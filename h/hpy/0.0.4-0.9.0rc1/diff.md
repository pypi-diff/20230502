# Comparing `tmp/hpy-0.0.4.tar.gz` & `tmp/hpy-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hpy-0.0.4.tar", last modified: Thu Jun  2 06:40:07 2022, max compression
+gzip compressed data, was "hpy-0.9.0rc1.tar", last modified: Tue May  2 19:38:32 2023, max compression
```

## Comparing `hpy-0.0.4.tar` & `hpy-0.9.0rc1.tar`

### file list

```diff
@@ -1,232 +1,324 @@
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.212427 hpy-0.0.4/
--rw-rw-r--   0 fa        (1000) fa        (1000)       37 2021-06-28 09:21:45.000000 hpy-0.0.4/.gitattributes
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.180428 hpy-0.0.4/.github/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.184428 hpy-0.0.4/.github/workflows/
--rw-rw-r--   0 fa        (1000) fa        (1000)     9943 2022-06-02 06:24:11.000000 hpy-0.0.4/.github/workflows/ci.yml
--rw-rw-r--   0 fa        (1000) fa        (1000)     2108 2022-02-09 08:35:11.000000 hpy-0.0.4/.github/workflows/release-pypi.yml
--rw-rw-r--   0 fa        (1000) fa        (1000)     1057 2022-02-09 08:35:11.000000 hpy-0.0.4/.gitignore
--rw-rw-r--   0 fa        (1000) fa        (1000)      171 2021-06-28 09:21:45.000000 hpy-0.0.4/.readthedocs.yml
--rw-rw-r--   0 fa        (1000) fa        (1000)     1370 2021-06-28 09:21:45.000000 hpy-0.0.4/CONTRIBUTING.md
--rw-rw-r--   0 fa        (1000) fa        (1000)     1065 2020-01-14 12:25:57.000000 hpy-0.0.4/LICENSE
--rw-rw-r--   0 fa        (1000) fa        (1000)       40 2021-06-28 09:21:45.000000 hpy-0.0.4/MANIFEST.in
--rw-rw-r--   0 fa        (1000) fa        (1000)     2017 2022-06-02 06:24:11.000000 hpy-0.0.4/Makefile
--rw-rw-r--   0 fa        (1000) fa        (1000)     5889 2022-06-02 06:40:07.716879 hpy-0.0.4/PKG-INFO
--rw-rw-r--   0 fa        (1000) fa        (1000)     5724 2021-06-28 09:21:45.000000 hpy-0.0.4/README-gdb.md
--rw-rw-r--   0 fa        (1000) fa        (1000)     4734 2022-02-09 08:35:11.000000 hpy-0.0.4/README.md
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.184428 hpy-0.0.4/c_test/
--rw-rw-r--   0 fa        (1000) fa        (1000)      449 2022-06-02 06:24:11.000000 hpy-0.0.4/c_test/Makefile
--rw-rw-r--   0 fa        (1000) fa        (1000)    60088 2021-11-15 16:41:49.000000 hpy-0.0.4/c_test/acutest.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     2240 2021-11-15 16:41:49.000000 hpy-0.0.4/c_test/test_debug_handles.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      465 2022-06-02 06:24:11.000000 hpy-0.0.4/c_test/test_stacktrace.c
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/
--rw-rw-r--   0 fa        (1000) fa        (1000)      767 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/Makefile
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/_static/
--rw-rw-r--   0 fa        (1000) fa        (1000)       43 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/_static/README.txt
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/_templates/
--rw-rw-r--   0 fa        (1000) fa        (1000)       45 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/_templates/README.txt
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/api-reference/
--rw-rw-r--   0 fa        (1000) fa        (1000)       84 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/api-reference/argument-parsing.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)      119 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api-reference/build-value.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)       81 2021-11-15 16:41:49.000000 hpy-0.0.4/docs/api-reference/helpers.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)       99 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api-reference/hpy-field.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)      174 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api-reference/hpy-gil.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)      103 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api-reference/hpy-global.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)      282 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api-reference/index.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     7138 2020-01-14 12:25:57.000000 hpy-0.0.4/docs/api.md
--rw-rw-r--   0 fa        (1000) fa        (1000)    12451 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/api.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     1056 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/changelog.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     3930 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/conf.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     6777 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/debug-mode.rst
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/examples/
--rw-rw-r--   0 fa        (1000) fa        (1000)      257 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/examples/debug-example.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/examples/mixed-example/
--rw-rw-r--   0 fa        (1000) fa        (1000)     1336 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/mixed-example/mixed.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      241 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/mixed-example/setup.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.188428 hpy-0.0.4/docs/examples/simple-example/
--rw-rw-r--   0 fa        (1000) fa        (1000)      244 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/simple-example/setup.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1001 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/simple-example/simple.c
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.192427 hpy-0.0.4/docs/examples/snippets/
--rw-rw-r--   0 fa        (1000) fa        (1000)     1463 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/snippets/hpyvarargs.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      336 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/examples/snippets/setup.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2135 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/examples/snippets/snippets.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     2256 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/examples/tests.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1632 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/index.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     8429 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/leysin-2020-design-decisions.md
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.192427 hpy-0.0.4/docs/misc/
--rw-rw-r--   0 fa        (1000) fa        (1000)       72 2021-11-15 16:41:49.000000 hpy-0.0.4/docs/misc/index.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)    20113 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/misc/str-builder-api.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     1128 2021-06-28 09:21:45.000000 hpy-0.0.4/docs/module-state.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)    16554 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/overview.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)     9767 2022-06-02 06:24:11.000000 hpy-0.0.4/docs/porting-guide.rst
--rw-rw-r--   0 fa        (1000) fa        (1000)      213 2022-02-09 08:35:11.000000 hpy-0.0.4/docs/requirements.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)     3261 2020-01-14 12:25:57.000000 hpy-0.0.4/docs/xxx-unsorted-notes.txt
--rwxrwxr-x   0 fa        (1000) fa        (1000)       69 2021-06-28 09:21:45.000000 hpy-0.0.4/gdb-py.test
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.184428 hpy-0.0.4/hpy/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.192427 hpy-0.0.4/hpy/debug/
--rw-rw-r--   0 fa        (1000) fa        (1000)      315 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/__init__.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1065 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/debug/leakdetector.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1096 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/debug/pytest.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.192427 hpy-0.0.4/hpy/debug/src/
--rw-rw-r--   0 fa        (1000) fa        (1000)    14205 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/_debugmod.c
--rw-rw-r--   0 fa        (1000) fa        (1000)    11313 2022-02-15 07:39:52.000000 hpy-0.0.4/hpy/debug/src/autogen_debug_ctx_call.i
--rw-rw-r--   0 fa        (1000) fa        (1000)    24403 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/autogen_debug_ctx_init.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    23153 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/autogen_debug_wrappers.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     7902 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/debug_ctx.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     7240 2022-02-15 07:39:52.000000 hpy-0.0.4/hpy/debug/src/debug_ctx_cpython.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      664 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/debug/src/debug_ctx_not_cpython.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     7254 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/debug_handles.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     9263 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/debug_internal.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     2708 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/debug/src/dhqueue.c
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.192427 hpy-0.0.4/hpy/debug/src/include/
--rw-rw-r--   0 fa        (1000) fa        (1000)     2294 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/include/hpy_debug.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1696 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/debug/src/memprotect.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     2582 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/debug/src/stacktrace.c
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:40:07.708879 hpy-0.0.4/hpy/devel/
--rw-rw-r--   0 fa        (1000) fa        (1000)    12111 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/__init__.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.196427 hpy-0.0.4/hpy/devel/include/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:40:07.708879 hpy-0.0.4/hpy/devel/include/hpy/
--rw-rw-r--   0 fa        (1000) fa        (1000)     6118 2022-02-10 09:06:57.000000 hpy-0.0.4/hpy/devel/include/hpy/autogen_hpyfunc_declare.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     4946 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/autogen_hpyslot.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      752 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/cpy_types.h
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.196427 hpy-0.0.4/hpy/devel/include/hpy/cpython/
--rw-rw-r--   0 fa        (1000) fa        (1000)    14335 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/cpython/autogen_api_impl.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     9144 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     6125 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    13140 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/cpython/misc.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     8911 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/hpydef.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     3808 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/include/hpy/hpyfunc.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     2060 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/hpymodule.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     4471 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/hpytype.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      982 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/inline_helpers.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     3029 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/macros.h
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.196427 hpy-0.0.4/hpy/devel/include/hpy/runtime/
--rw-rw-r--   0 fa        (1000) fa        (1000)      503 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/runtime/argparse.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      218 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/include/hpy/runtime/buildvalue.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     3025 2022-06-02 06:03:57.000000 hpy-0.0.4/hpy/devel/include/hpy/runtime/ctx_funcs.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1910 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/include/hpy/runtime/ctx_type.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      311 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/include/hpy/runtime/helpers.h
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.196427 hpy-0.0.4/hpy/devel/include/hpy/universal/
--rw-rw-r--   0 fa        (1000) fa        (1000)    12476 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_ctx.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    11924 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    19422 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     6454 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1418 2022-06-02 06:03:57.000000 hpy-0.0.4/hpy/devel/include/hpy/universal/misc_trampolines.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      120 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy/devel/include/hpy/version.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     5381 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/include/hpy.h
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.180428 hpy-0.0.4/hpy/devel/src/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.200427 hpy-0.0.4/hpy/devel/src/runtime/
--rw-rw-r--   0 fa        (1000) fa        (1000)    22684 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/src/runtime/argparse.c
--rw-rw-r--   0 fa        (1000) fa        (1000)    13886 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/src/runtime/buildvalue.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      833 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_bytes.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1210 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_call.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      246 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_err.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1528 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_listbuilder.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1083 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_module.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     2482 2022-06-02 06:03:57.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_object.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     4324 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_tracker.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      454 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_tuple.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1978 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_tuplebuilder.c
--rw-rw-r--   0 fa        (1000) fa        (1000)    30701 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/devel/src/runtime/ctx_type.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1808 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/devel/src/runtime/helpers.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      107 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy/devel/version.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.200427 hpy-0.0.4/hpy/tools/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/hpy/tools/autogen/
--rw-rw-r--   0 fa        (1000) fa        (1000)     1808 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/tools/autogen/__main__.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      876 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/autogen/autogenfile.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     4117 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/conf.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2434 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/ctx.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     5774 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/debug.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     7302 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/hpyfunc.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      547 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/tools/autogen/hpyslot.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     6228 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/parse.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    25671 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/public_api.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1395 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/autogen/pypy.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/hpy/tools/autogen/testing/
--rw-rw-r--   0 fa        (1000) fa        (1000)        0 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/autogen/testing/__init__.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     6221 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/tools/autogen/testing/test_autogen.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     5712 2021-11-15 16:41:49.000000 hpy-0.0.4/hpy/tools/autogen/testing/test_hpyfunc.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     4607 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/tools/autogen/trampolines.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      128 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/include_path.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/hpy/tools/valgrind/
--rw-rw-r--   0 fa        (1000) fa        (1000)      586 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/valgrind/hpy.supp
--rw-rw-r--   0 fa        (1000) fa        (1000)     6813 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/tools/valgrind/python.supp
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.184428 hpy-0.0.4/hpy/universal/
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/hpy/universal/src/
--rw-rw-r--   0 fa        (1000) fa        (1000)      355 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/universal/src/api.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     6631 2022-02-10 09:06:57.000000 hpy-0.0.4/hpy/universal/src/autogen_ctx_call.i
--rw-rw-r--   0 fa        (1000) fa        (1000)     7196 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/autogen_ctx_def.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    14315 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/autogen_ctx_impl.h
--rw-rw-r--   0 fa        (1000) fa        (1000)      212 2022-02-09 08:35:11.000000 hpy-0.0.4/hpy/universal/src/ctx.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     4326 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/ctx_meth.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      192 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/ctx_meth.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1471 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/ctx_misc.c
--rw-rw-r--   0 fa        (1000) fa        (1000)      821 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/ctx_misc.h
--rw-rw-r--   0 fa        (1000) fa        (1000)     1221 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/handles.h
--rw-rw-r--   0 fa        (1000) fa        (1000)    10205 2022-06-02 06:24:11.000000 hpy-0.0.4/hpy/universal/src/hpymodule.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     1418 2021-06-28 09:21:45.000000 hpy-0.0.4/hpy/universal/src/misc_win32.h
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:40:07.708879 hpy-0.0.4/hpy.egg-info/
--rw-rw-r--   0 fa        (1000) fa        (1000)     5889 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/PKG-INFO
--rw-rw-r--   0 fa        (1000) fa        (1000)     5485 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/SOURCES.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)        1 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/dependency_links.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)       79 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/entry_points.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)       27 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/requires.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)        4 2022-06-02 06:40:07.000000 hpy-0.0.4/hpy.egg-info/top_level.txt
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/microbench/
--rw-rw-r--   0 fa        (1000) fa        (1000)      531 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/README.md
--rw-rw-r--   0 fa        (1000) fa        (1000)      551 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/_valgrind_build.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     3805 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/conftest.py
--rwxrwxr-x   0 fa        (1000) fa        (1000)       85 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/pytest_valgrind.sh
--rw-rw-r--   0 fa        (1000) fa        (1000)      464 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/setup.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.204427 hpy-0.0.4/microbench/src/
--rw-rw-r--   0 fa        (1000) fa        (1000)     4546 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/src/cpy_simple.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     3460 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/src/hpy_simple.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     5043 2022-02-09 14:23:56.000000 hpy-0.0.4/microbench/test_microbench.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.208427 hpy-0.0.4/proof-of-concept/
--rw-rw-r--   0 fa        (1000) fa        (1000)      552 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/Makefile
--rw-rw-r--   0 fa        (1000) fa        (1000)     2865 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/pof.c
--rw-rw-r--   0 fa        (1000) fa        (1000)     2950 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/pofcpp.cpp
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.208427 hpy-0.0.4/proof-of-concept/pofpackage/
--rw-rw-r--   0 fa        (1000) fa        (1000)      865 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/pofpackage/bar.cpp
--rw-rw-r--   0 fa        (1000) fa        (1000)      574 2022-02-09 08:35:11.000000 hpy-0.0.4/proof-of-concept/pofpackage/foo.c
--rw-rw-r--   0 fa        (1000) fa        (1000)        4 2022-02-09 08:35:11.000000 hpy-0.0.4/proof-of-concept/requirements.txt
--rw-rw-r--   0 fa        (1000) fa        (1000)     1023 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/setup.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1097 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/test_pof.py
--rwxrwxr-x   0 fa        (1000) fa        (1000)     4843 2022-06-02 06:24:11.000000 hpy-0.0.4/proof-of-concept/test_pof.sh
--rw-rw-r--   0 fa        (1000) fa        (1000)      137 2022-06-02 06:24:11.000000 hpy-0.0.4/pyproject.toml
--rw-rw-r--   0 fa        (1000) fa        (1000)       38 2022-06-02 06:40:07.716879 hpy-0.0.4/setup.cfg
--rw-rw-r--   0 fa        (1000) fa        (1000)     6072 2022-06-02 06:24:11.000000 hpy-0.0.4/setup.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.212427 hpy-0.0.4/test/
--rw-rw-r--   0 fa        (1000) fa        (1000)        0 2020-01-14 12:25:57.000000 hpy-0.0.4/test/__init__.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2321 2022-02-09 08:35:11.000000 hpy-0.0.4/test/check_py27_compat.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2260 2022-02-15 07:39:52.000000 hpy-0.0.4/test/conftest.py
-drwxrwxr-x   0 fa        (1000) fa        (1000)        0 2022-06-02 06:36:10.212427 hpy-0.0.4/test/debug/
--rw-rw-r--   0 fa        (1000) fa        (1000)     8841 2022-02-09 08:35:11.000000 hpy-0.0.4/test/debug/test_charptr.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     5130 2022-02-15 07:39:52.000000 hpy-0.0.4/test/debug/test_handles_invalid.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     8809 2022-06-02 06:24:11.000000 hpy-0.0.4/test/debug/test_handles_leak.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    17465 2022-06-02 06:24:11.000000 hpy-0.0.4/test/support.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    15489 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_00_basic.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    22127 2022-02-09 08:35:11.000000 hpy-0.0.4/test/test_argparse.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     3885 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_call.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     6765 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_cpy_compat.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2221 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_helpers.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     9305 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpybuildvalue.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     4453 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_hpybytes.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2337 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_hpydict.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    29203 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpyerr.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    15078 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpyfield.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1172 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpyglobal.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      826 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_hpyimport.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2526 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_hpylist.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    12165 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpylong.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      855 2022-02-09 08:35:11.000000 hpy-0.0.4/test/test_hpymodule.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     2746 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_hpytuple.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    28186 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpytype.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     7580 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpytype_legacy.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     7035 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_hpyunicode.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     1764 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_importing.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     7638 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_number.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    17222 2022-06-02 06:03:57.000000 hpy-0.0.4/test/test_object.py
--rw-rw-r--   0 fa        (1000) fa        (1000)    26521 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_slots.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     7952 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_slots_legacy.py
--rw-rw-r--   0 fa        (1000) fa        (1000)      715 2022-06-02 06:24:11.000000 hpy-0.0.4/test/test_support.py
--rw-rw-r--   0 fa        (1000) fa        (1000)     4151 2021-11-15 16:41:49.000000 hpy-0.0.4/test/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.github/workflows/valgrind-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/README-gdb.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/c_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    60089 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/acutest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/test_debug_handles.c
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/c_test/test_stacktrace.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/_static/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.163920 hpy-0.9.0rc1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/_templates/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/argument-parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/build-value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/function-index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-call.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-ctx.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-dict.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-err.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-eval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-field.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-gil.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-global.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/hpy-type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/inline-helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/public-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api-reference/structseq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25010 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/debug-mode.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/debug-example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/hpytype-example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/builtin_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/simple_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/hpytype-example/simple_type.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/mixed-example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/mixed-example/mixed.c
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/mixed-example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.167920 hpy-0.9.0rc1/docs/examples/quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/quickstart/quickstart.c
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/quickstart/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/examples/simple-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/simple-example/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/simple-example/simple.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/examples/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpycall.c
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpyinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/hpyvarargs.c
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/legacyinit.c
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/snippets/snippets.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/examples/trace-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/leysin-2020-design-decisions.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/misc/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/module-state.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/porting-example/
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.171920 hpy-0.9.0rc1/docs/porting-example/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup00.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup01.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup02.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/setup03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_00_c_api.c
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_00_c_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_01_hpy_legacy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_01_hpy_legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_02_hpy_legacy.c
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_02_hpy_legacy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_03_hpy_final.c
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/step_03_hpy_final.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-example/steps/test_porting_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40482 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/porting-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/trace-mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/docs/xxx-unsorted-notes.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/gdb-py.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/leakdetector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    14954 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/_debugmod.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_call.i
+-rw-r--r--   0 runner    (1001) docker     (123)    29310 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    59317 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/autogen_debug_wrappers.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_ctx_not_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_handles.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13759 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/debug_internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/dhqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/debug/src/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/include/hpy_debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/memprotect.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/debug/src/stacktrace.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/devel/
+-rw-r--r--   0 runner    (1001) docker     (123)    18442 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/abitag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy/devel/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyfunc_declare.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyslot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpy_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_api_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_ctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/misc.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/forbid_python_h/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/forbid_python_h/Python.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpydef.h
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpyexports.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpyfunc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpymodule.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/hpytype.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/inline_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/macros.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/argparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/buildvalue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_funcs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_module.h
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/ctx_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/format.h
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/helpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/runtime/structseq.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.179920 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_ctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/universal/misc_trampolines.h
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy/devel/include/hpy/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/include/hpy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/devel/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/devel/src/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)    26604 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/argparse.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14606 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/buildvalue.c
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_bytes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_call.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_capsule.c
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_contextvar.c
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_err.c
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_eval.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_listbuilder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_long.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_module.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_object.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tracker.c
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuplebuilder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57318 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_type.c
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/format.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/helpers.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/devel/src/runtime/structseq.c
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy/devel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/autogen.h
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/autogenfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/hpyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/hpyslot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48452 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/public_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/pypy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/autogen/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/test_autogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/testing/test_hpyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/autogen/trampolines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/include_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/tools/valgrind/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/valgrind/hpy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/tools/valgrind/python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/_tracemod.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27287 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_ctx_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_func_table.c
+-rw-r--r--   0 runner    (1001) docker     (123)    78016 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/autogen_trace_wrappers.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.183920 hpy-0.9.0rc1/hpy/trace/src/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/include/hpy_trace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/trace_ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/trace/src/trace_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.159920 hpy-0.9.0rc1/hpy/universal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/hpy/universal/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_call.i
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_def.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_meth.c
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_meth.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_misc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/ctx_misc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/handles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24089 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/hpymodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/hpy/universal/src/misc_win32.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.175920 hpy-0.9.0rc1/hpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:38:32.000000 hpy-0.9.0rc1/hpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/microbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/_valgrind_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/pytest_valgrind.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/microbench/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/src/cpy_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/src/hpy_simple.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/microbench/test_microbench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/proof-of-concept/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pof.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofcpp.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.187920 hpy-0.9.0rc1/proof-of-concept/pofpackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofpackage/bar.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/pofpackage/foo.c
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/test_pof.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/proof-of-concept/test_pof.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/requirements-autogen.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.191920 hpy-0.9.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/check_py27_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_builder_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_charptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_context_reuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_handles_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_handles_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/debug/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/hpy_devel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/hpy_devel/test_abitag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/hpy_devel/test_distutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_00_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17094 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_capsule_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_contextvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_cpy_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpybuildvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpybytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpydict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29552 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyerr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyglobal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16027 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpylong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpymodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpystructseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60249 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpytype_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43142 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_hpyunicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_legacy_forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_slots_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:38:32.195921 hpy-0.9.0rc1/test/trace/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-02 19:38:25.000000 hpy-0.9.0rc1/test/trace/test_trace.py
```

### Comparing `hpy-0.0.4/.github/workflows/ci.yml` & `hpy-0.9.0rc1/.github/workflows/ci.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,130 +7,118 @@
   main_tests:
     name: Main tests ${{ matrix.os }} ${{ matrix.python-version }} ${{ matrix.compiler }}
     runs-on: ${{ matrix.os }}
     continue-on-error: true
     strategy:
       # Duplicate changes to this matrix to 'poc_tests'
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
+        os: [ubuntu-latest, macos-11, windows-latest]
         python-version: ['3.9', '3.10']
-        # Possible values: ['2.7', '3.6', '3.7', '3.8', '3.9', '3.10.0-rc.2', 'pypy-3.8']
         compiler: [""]
         include:
           - os: ubuntu-latest
-            python-version: '3.6'
-          - os: ubuntu-latest
-            python-version: '3.7'
-          - os: ubuntu-latest
             python-version: '3.8'
           - os: ubuntu-latest
-            python-version: '3.9'
+            python-version: '3.10'
             compiler: 'g++'
-          ## Expected failure
-          # - os: ubuntu-latest
-          #   python-version: '3.10.0-rc.2'
+          - os: ubuntu-latest
+            python-version: '3.11'
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       # - template: azure-templates/ccache.yml
       #   parameters:
       #     pythonVersion: $(python.version)
       # - template: azure-templates/python.yml
       #   parameters:
       #     pythonVersion: $(python.version)
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install/Upgrade Python dependencies
-        run: python -m pip install --upgrade pip wheel
+        run: python -m pip install --upgrade pip wheel 'setuptools>=60.2'
 
       - name: Build
-        run: python -m pip install .
+        run: |
+          make
+          python -m pip install .
 
       - if: ${{ matrix.compiler }}
         # Only set the compiler for the tests, not for the build
         run: echo "CC=${{ matrix.compiler }}" >> $GITHUB_ENV
 
       - name: Run tests
         run: |
-          python -m pip install pytest pytest-xdist
-          python -m pytest --durations=16 -n auto test/
+          python -m pip install pytest pytest-xdist filelock
+          python -m pytest --basetemp=.tmpdir --durations=16 -n auto test/
 
   main_tests_debug:
     name: Main tests on CPython debug builds
     runs-on: ${{ matrix.os }}
-    continue-on-error: true
     strategy:
       matrix:
         os: [ubuntu-latest]
-        python-version: ['3.10', '3.9', '3.8', '3.7']
-
-    env:
-      SETUPTOOLS_USE_DISTUTILS: stdlib
+        python-version: ['3.11', '3.10', '3.9', '3.8']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python from deadsnakes
         uses: deadsnakes/action@v2.1.1
         with:
           python-version: ${{ matrix.python-version }}
           debug: true
 
       - name: Check Python debug build
         run: python -c "import sys; print(hasattr(sys, 'gettotalrefcount'))"
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
 
       - name: Build
-        run: python -m pip install .
+        run: |
+          make
+          python -m pip install .
 
       - name: Run tests
         run: |
-          python -m pip install pytest pytest-xdist
+          python -m pip install pytest pytest-xdist filelock
           python -m pytest --durations=16 -n auto test/
 
   poc_tests:
     name: Proof of concept tests
     runs-on: ${{ matrix.os }}
-    continue-on-error: true
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.9']
+        os: [ubuntu-latest, macos-11, windows-latest]
+        python-version: ['3.10']
         include:
           - os: ubuntu-latest
-            python-version: '3.6'
-          - os: ubuntu-latest
-            python-version: '3.7'
-          - os: ubuntu-latest
             python-version: '3.8'
           - os: ubuntu-latest
-            python-version: '3.10'
-          ## Expected failure
-          # - os: ubuntu-latest
-          #   python-version: '3.10.0-rc.2'
+            python-version: '3.9'
+          - os: ubuntu-latest
+            python-version: '3.11'
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       # - template: azure-templates/ccache.yml
       #   parameters:
       #     pythonVersion: $(python.version)
       # - template: azure-templates/python.yml
       #   parameters:
       #     pythonVersion: $(python.version)
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
         shell: bash
 
@@ -155,127 +143,161 @@
         shell: bash
 
       - name: 'Test setup.py --hpy-abi=universal build_ext --inplace'
         run: proof-of-concept/test_pof.sh setup_py_build_ext_inplace universal
         shell: bash
 
 
-  valgrind_tests:
-    name: Valgrind tests
-    runs-on: 'ubuntu-latest'
-    steps:
-      - uses: actions/checkout@v2
+  porting_example_tests:
+    name: Porting example tests
+    runs-on: ${{ matrix.os }}
+    continue-on-error: true
+    strategy:
+      matrix:
+        os: [ubuntu-latest, macos-11, windows-latest]
+        python-version: ['3.9']
 
-    # - template: azure-templates/ccache.yml
-    # - template: azure-templates/python.yml
+    steps:
+      - uses: actions/checkout@v3
 
-      - name: Install / Upgrade system dependencies
-        run: sudo apt update && sudo apt install -y valgrind
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
 
-      - name: Install / Upgrade Python dependencies
+      - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
+        shell: bash
 
-      - name: Build
+      - name: Install HPy
         run: python -m pip install .
 
-      - name: Run tests
+      - name: Install pytest
         run: |
-          python -m pip install pytest pytest-valgrind
-          make valgrind
+          python -m pip install pytest
+
+      - name: Run tests
+        run: make porting-example-tests
+        shell: bash
+
+      - name: Run tests of completed port in debug mode
+        env:
+          HPY_DEBUG: "1"
+          TEST_ARGS: "-s -k hpy_final"
+        run: make porting-example-tests
+        shell: bash
+
+
+  valgrind_tests_1:
+    name: 'Valgrind tests (1/3)'
+    uses: ./.github/workflows/valgrind-tests.yml
+    with:
+      portion: '1/3'
+
+
+  valgrind_tests_2:
+    name: 'Valgrind tests (2/3)'
+    uses: ./.github/workflows/valgrind-tests.yml
+    with:
+      portion: '2/3'
+
+
+  valgrind_tests_3:
+    name: 'Valgrind tests (3/3)'
+    uses: ./.github/workflows/valgrind-tests.yml
+    with:
+      portion: '3/3'
+
 
   docs_examples_tests:
     name: Documentation examples tests
     runs-on: ${{ matrix.os }}
-    continue-on-error: true
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ['3.9']
+        os: [ubuntu-latest, macos-11, windows-latest]
+        python-version: ['3.10']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
         shell: bash
 
       - name: Install HPy
         run: python -m pip install .
 
       - name: Install pytest
         run: |
-          python -m pip install pytest
+          python -m pip install pytest pytest-xdist filelock
       - name: Run tests
         run: make docs-examples-tests
         shell: bash
 
   build_docs:
     name: Build documentation
     runs-on: 'ubuntu-latest'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       # - template: azure-templates/python.yml
 
       - name: Install / Upgrade system requirements
-        run: sudo apt update && sudo apt install -y libclang-10-dev
+        run: sudo apt update && sudo apt install -y libclang-11-dev
 
       - name: Install / Upgrade Python requirements
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r docs/requirements.txt
 
       - name: Build docs
         run: |
           cd docs;
           python -m sphinx -T -W -E -b html -d _build/doctrees -D language=en . _build/html
 
       - name: Upload built HTML files
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: hpy_html_docs
           path: docs/_build/html/*
           if-no-files-found: error
           retention-days: 5
 
   c_tests:
     name: C tests
     runs-on: 'ubuntu-latest'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - run: make -C c_test
 
 
   check_autogen:
     name: Check autogen
     runs-on: 'ubuntu-latest'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
     # - template: azure-templates/python.yml
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.x'
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
 
-      - name: Install dependencies
-        run: |
-          pip install pycparser==2.20
-          pip install py==1.8.0
-          pip install packaging==19.2
-          pip install attrs==19.3.0
+      - name: Install autogen dependencies
+        run: pip install -r requirements-autogen.txt
+
       - name: make autogen
         run: |
           make autogen
           if [ -z "$(git status --porcelain)" ]; then
               # clean working copy
               echo "Working copy is clean, everything ok"
           else
@@ -288,73 +310,104 @@
               git diff
               exit 1
           fi
 
 
   check_py27_compat:
     name: Check Python 2.7 compatibility
-    runs-on: 'ubuntu-latest'
+    runs-on: 'ubuntu-20.04'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
     # - template: azure-templates/python.yml
     #   parameters:
     #     pythonVersion: "2.7"
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '2.7'
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
 
       - name: check_py27_compat.py
         run: |
-          python -m pip install pytest pathlib
+          python -m pip install pytest pytest-xdist filelock pathlib
           python test/check_py27_compat.py
 
 
   cpp_check:
     name: Cppcheck static analysis
-    runs-on: 'ubuntu-latest'
+    runs-on: 'ubuntu-22.04'
+    continue-on-error: true
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: '3.x'
+          python-version: '3.10'
 
       - name: Install Cppcheck
-        run: sudo apt-get -qq -y install cppcheck
+        run: sudo apt-get -qq -y install cppcheck=2.7-1
 
       - name: Run Cppcheck
         run: make cppcheck
 
 
   infer:
     name: Infer static analysis
     runs-on: 'ubuntu-latest'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       # - template: azure-templates/python.yml
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: '3.x'
+          python-version: '3.10'
 
       - name: Install/Upgrade Python dependencies
         run: python -m pip install --upgrade pip wheel
 
       - name: Install Infer
         run: |
           python -m pip install compiledb wheel;
           VERSION=1.1.0; \
           curl -sSL "https://github.com/facebook/infer/releases/download/v$VERSION/infer-linux64-v$VERSION.tar.xz" \
           | sudo tar -C /opt -xJ && \
           echo "/opt/infer-linux64-v$VERSION/bin" >> $GITHUB_PATH
 
       - name: Run Infer
         run: make infer
+
+  check_microbench:
+    name: Check micro benchmarks
+    runs-on: 'ubuntu-latest'
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.x'
+
+      - name: Install / Upgrade system dependencies
+        run: sudo apt update && sudo apt install -y valgrind
+
+      - name: Install / Upgrade Python requirements
+        run: |
+          python -m pip install --upgrade pip wheel 'setuptools>=60.2'
+          python -m pip install pytest cffi
+
+      - name: Build and install HPy
+        run: |
+          make
+          python -m pip install .
+
+      - name: Run microbenchmarks
+        run: |
+          cd microbench
+          python setup.py build_ext -i
+          python -m pytest -v
```

### Comparing `hpy-0.0.4/.gitignore` & `hpy-0.9.0rc1/.gitignore`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 proof-of-concept/pofpackage/foo.py
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
-# C extensions
+# C extensions and static libs
 *.so
 *.o
+*.a
+*.lib
 vc140.pdb
 c_test/test_debug_handles
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
@@ -55,14 +57,15 @@
 nosetests.xml
 coverage.xml
 test-output.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
+.hpy.lock
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
 # IPython
 profile_default/
 ipython_config.py
@@ -80,7 +83,10 @@
 venv.bak/
 
 # cppcheck
 .cppcheck
 
 # Sphinx
 docs/_build/
+
+# vscode
+.vscode
```

### Comparing `hpy-0.0.4/CONTRIBUTING.md` & `hpy-0.9.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/LICENSE` & `hpy-0.9.0rc1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 pyhandle
+Copyright (c) 2019 The HPy Authors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hpy-0.0.4/Makefile` & `hpy-0.9.0rc1/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .PHONY: all
 all: hpy.universal
 
 .PHONY: hpy.universal
 hpy.universal:
-	python3 setup.py build_ext -if
+	python3 setup.py build_clib -f build_ext -if
 
 .PHONY: dist-info
 dist-info:
 	python3 setup.py dist_info
 
 debug:
 	HPY_DEBUG_BUILD=1 make all
@@ -18,42 +18,69 @@
 cppcheck-build-dir:
 	mkdir -p $(or ${CPPCHECK_BUILD_DIR}, .cppcheck)
 
 .PHONY: cppcheck
 cppcheck: cppcheck-build-dir
 	# azure pipelines doesn't show stderr, so we write the errors to a file and cat it later :(
 	$(eval PYTHON_INC = $(shell python3 -q -c "from sysconfig import get_paths as gp; print(gp()['include'])"))
+	$(eval PYTHON_PLATINC = $(shell python3 -q -c "from sysconfig import get_paths as gp; print(gp()['platinclude'])"))
 	cppcheck --version
 	cppcheck \
 		-v \
 		--error-exitcode=1 \
 		--cppcheck-build-dir=$(or ${CPPCHECK_BUILD_DIR}, .cppcheck) \
-		--output-file=$(or ${CPPCHECK_BUILD_DIR}, .cppcheck)/output.txt \
 		--enable=warning,performance,portability,information,missingInclude \
 		--inline-suppr \
-		--suppress=allocaCalled \
-		-I /usr/local/include \
+		--suppress=syntaxError \
+		-I /usr/local/include/ \
+		-I /usr/include/ \
 		-I ${PYTHON_INC} \
+		-I ${PYTHON_PLATINC} \
+		-I . \
 		-I hpy/devel/include/ \
 		-I hpy/devel/include/hpy/ \
 		-I hpy/devel/include/hpy/cpython/ \
 		-I hpy/devel/include/hpy/universal/ \
 		-I hpy/devel/include/hpy/runtime/ \
 		-I hpy/universal/src/ \
 		-I hpy/debug/src/ \
+		-I hpy/debug/src/include \
+		-I hpy/trace/src/ \
+		-I hpy/trace/src/include \
 		--force \
 		-D NULL=0 \
-		. || (cat $(or ${CPPCHECK_BUILD_DIR}, .cppcheck)/output.txt && false)
+		-D HPY_ABI_CPYTHON \
+		-D __linux__=1 \
+		-D __x86_64__=1 \
+		-D __LP64__=1 \
+		.
 
 infer:
 	python3 setup.py build_ext -if -U NDEBUG | compiledb
 	# see commit cd8cd6e for why we need to ignore debug_ctx.c
 	@infer --fail-on-issue --compilation-database compile_commands.json --report-blacklist-path-regex "hpy/debug/src/debug_ctx.c"
 
+valgrind_args = --suppressions=hpy/tools/valgrind/python.supp --suppressions=hpy/tools/valgrind/hpy.supp --leak-check=full --show-leak-kinds=definite,indirect --log-file=/tmp/valgrind-output
+python_args = -m pytest --valgrind --valgrind-log=/tmp/valgrind-output
+
+.PHONY: valgrind
 valgrind:
-	PYTHONMALLOC=malloc valgrind --suppressions=hpy/tools/valgrind/python.supp --suppressions=hpy/tools/valgrind/hpy.supp --leak-check=full --show-leak-kinds=definite,indirect --log-file=/tmp/valgrind-output python -m pytest --valgrind --valgrind-log=/tmp/valgrind-output test/
+ifeq ($(HPY_TEST_PORTION),)
+	PYTHONMALLOC=malloc valgrind $(valgrind_args) python3 $(python_args) test/
+else
+	PYTHONMALLOC=malloc valgrind $(valgrind_args) python3 $(python_args) --portion $(HPY_TEST_PORTION) test/
+endif
+
+porting-example-tests:
+	cd docs/porting-example/steps && python3 setup00.py build_ext -i
+	cd docs/porting-example/steps && python3 setup01.py build_ext -i
+	cd docs/porting-example/steps && python3 setup02.py build_ext -i
+	cd docs/porting-example/steps && python3 setup03.py --hpy-abi=universal build_ext -i
+	python3 -m pytest docs/porting-example/steps/ ${TEST_ARGS}
 
 docs-examples-tests:
-	python docs/examples/simple-example/setup.py --hpy-abi=universal install
-	python docs/examples/mixed-example/setup.py install
-	python docs/examples/snippets/setup.py --hpy-abi=universal install
-	pytest docs/examples/tests.py
+	cd docs/examples/simple-example  && python3 setup.py --hpy-abi=universal install
+	cd docs/examples/mixed-example   && python3 setup.py install
+	cd docs/examples/snippets        && python3 setup.py --hpy-abi=universal install
+	cd docs/examples/quickstart      && python3 setup.py --hpy-abi=universal install
+	cd docs/examples/hpytype-example && python3 setup.py --hpy-abi=universal install
+	python3 -m pytest docs/examples/tests.py ${TEST_ARGS}
```

### Comparing `hpy-0.0.4/README-gdb.md` & `hpy-0.9.0rc1/README-gdb.md`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/c_test/acutest.h` & `hpy-0.9.0rc1/c_test/acutest.h`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
  * You may define another limit prior including "acutest.h"
  */
 #ifndef TEST_DUMP_MAXSIZE
     #define TEST_DUMP_MAXSIZE   1024
 #endif
 
 
-/* Common test initialiation/clean-up
+/* Common test initialization/clean-up
  *
  * In some test suites, it may be needed to perform some sort of the same
  * initialization and/or clean-up in all the tests.
  *
  * Such test suites may use macros TEST_INIT and/or TEST_FINI prior including
  * this header. The expansion of the macro is then used as a body of helper
  * function called just before executing every single (TEST_INIT) or just after
```

### Comparing `hpy-0.0.4/docs/Makefile` & `hpy-0.9.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/docs/conf.py` & `hpy-0.9.0rc1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
+import sys
 import os
 import re
+import datetime
 
 # -- Project information -----------------------------------------------------
 
 project = "HPy"
-copyright = "2019-2020, HPy Collective"
+copyright = "2019-{}, HPy Collective".format(datetime.date.today().year)
 author = "HPy Collective"
 
 # The full version, including alpha/beta/rc tags
-release = "0.0.1"
+release = "0.9"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -45,28 +47,38 @@
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
+# -- autodoc -----------------------------------------------------------------
+
+autodoc_member_order = "bysource"
+
 # -- sphinx_c_autodoc --------------------------------------------------------
 
 c_autodoc_roots = [
     "../hpy/devel/include",
     "../hpy/devel/src",
     "../hpy/tools",
 ]
 
 
 def pre_process(app, filename, contents, *args):
+    # FIXME: the missing typedef for 'HPy' causes the file formatting to fail
+    if filename.endswith('public_api.h'):
+        contents[0] = '#include "../../devel/include/hpy.h"\n' + contents[0]
+    if filename.endswith('autogen_ctx.h'):
+        contents[0] = 'typedef int HPy;' + contents[0]
+
     # remove HPyAPI_HELPER so that the sphinx-c-autodoc and clang
     # find and render the API functions
     contents[:] = [
-        re.sub(r"^HPyAPI_HELPER ", r"", part, flags=re.MULTILINE)
+        re.sub(r"^(HPyAPI_HELPER|HPyAPI_INLINE_HELPER|HPy_ID\(\d+\))", r"", part, flags=re.MULTILINE)
         for part in contents
     ]
 
 
 def setup(app):
     app.connect("c-autodoc-pre-process", pre_process)
 
@@ -94,14 +106,18 @@
     if 'READTHEDOCS' in os.environ:
         # TODO: Hopefully we can remove this setting of the libclang path once
         #       readthedocs updates its docker image to Ubuntu 20.04 which
         #       supports clang-10 and clang-11.
         cindex.Config.set_library_file(
             "/usr/lib/x86_64-linux-gnu/libclang-6.0.so.1"
         )
+    elif sys.platform == "darwin":
+        cindex.Config.set_library_file(
+            "/Library/Developer/CommandLineTools/usr/lib/libclang.dylib"
+        )
 
 
 setup_clang()
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
```

### Comparing `hpy-0.0.4/docs/debug-mode.rst` & `hpy-0.9.0rc1/docs/debug-mode.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,94 +1,106 @@
 Debug Mode
 ==========
 
-HPy includes a debug mode which includes a lot of useful run-time checks to
-ensure that C extensions use the API correctly. The major points of the debug mode are:
+HPy includes a debug mode which does useful run-time checks to ensure that C
+extensions use the API correctly. Its features include:
 
-    1. no special compilation flags are required: it is enough to compile the extension 
-       with the Universal ABI.
-    
-    2. The debug mode can be activated at *import time*, and it can be activated
+    1. No special compilation flags are required: it is enough to compile the
+       extension with the Universal ABI.
+
+    2. Debug mode can be activated at *import time*, and it can be activated
        per-extension.
-    
-    3. You pay the overhead of the debug mode only if you use it. Extensions loaded 
+
+    3. You pay the overhead of debug mode only if you use it. Extensions loaded
        without the debug mode run at full speed.
 
-This is possible because the whole of the HPy API is provided
-as part of the HPy context, so debug mode can pass in a special debugging
-context (that wraps the normal context) without affecting the performance of
-the regular context at all.
+This is possible because the whole of the HPy API is provided as part of the HPy
+context, so debug mode can pass in a special debugging context without affecting
+the performance of the regular context at all.
+
+.. note:: The debug mode is only available if the module (you want to use it
+    for) was built for :term:`HPy Universal ABI`.
 
 The debugging context can already check for:
 
 * Leaked handles.
 * Handles used after they are closed.
+* Tuple and list builder used after they were *closed* (i.e. cancelled or the
+  tuple/list was built).
 * Reading from a memory which is no longer guaranteed to be still valid,
-  for example, the buffer returned by ``HPyUnicode_AsUTF8AndSize`` after the
+  for example, the buffer returned by :c:func:`HPyUnicode_AsUTF8AndSize`,
+  :c:func:`HPyBytes_AsString`, and :c:func:`HPyBytes_AS_STRING`, after the
   corresponding ``HPy`` handle was closed.
-* Writing to a memory which should be read-only, for example,
-  the buffer returned by ``HPyUnicode_AsUTF8AndSize``.
+* Writing to memory which should be read-only, for example the buffer
+  returned by :c:func:`HPyUnicode_AsUTF8AndSize`, :c:func:`HPyBytes_AsString`,
+  and :c:func:`HPyBytes_AS_STRING`
 
 
 Activating Debug Mode
 ---------------------
 
-The debug mode works only for extensions built with HPy universal ABI.
+Debug mode works *only* for extensions built with HPy universal ABI.
 
-To enable the debug mode, use environment variable ``HPY_DEBUG``.
-If ``HPY_DEBUG=1``, then all HPy modules are loaded with debug context.
-Alternatively ``HPY_DEBUG`` can be set to a comma separated list of names
-of the modules that should be loaded in the debug mode.
-
-In order to verify that your extension is being loaded in the HPy debug mode,
-use environment variable ``HPY_LOG``. If this variable is set, then all HPy
-extensions built in universal ABI mode print a message, such as:
+To enable debug mode, use environment variable ``HPY``. If ``HPY=debug``, then
+all HPy modules are loaded with the trace context. Alternatively, it is also
+possible to specify the mode per module like this:
+``HPY=modA:debug,modB:debug``.
+
+In order to verify that your extension is being loaded in debug mode, use
+environment variable ``HPY_LOG``. If this variable is set, then all HPy
+extensions built in universal ABI mode print a message when loaded, such as:
 
 .. code-block:: console
 
     > import snippets
     Loading 'snippets' in HPy universal mode with a debug context
 
 .. Note: the output above is tested in test_leak_detector_with_traces_output
 
-If the extension is built in CPython ABI mode, then the ``HPY_LOG``
-environment variable has no effect.
+If the extension is built in CPython ABI mode, then the ``HPY_LOG`` environment
+variable has no effect.
 
-An HPy extension module may be also explicitly loaded in debug mode using::
+An HPy extension module may be also explicitly loaded in debug mode using:
 
-  mod = hpy.universal.load(module_name, so_filename, debug=True)
+.. code-block:: python
+
+   from hpy.universal import load, MODE_DEBUG
+   mod = load(module_name, so_filename, mode=MODE_DEBUG)
 
 When loading HPy extensions explicitly, environment variables ``HPY_LOG``
-and ``HPY_DEBUG`` have no effect for that extension.
+and ``HPY`` have no effect for that extension.
 
 
 Using Debug Mode
 ----------------
 
-The HPy debug module exposes ``LeakDetector`` class for detection of
-leaked handles. ``LeakDetector`` can be used to check that some code does
-not leave behind unclosed ``HPy`` handles. For example:
+By default, when debug mode detects an error it will either abort the process
+(using :c:func:`HPy_FatalError`) or raise a fatal exception. This may sound very
+strict but in general, it is not safe to continue the execution.
+
+When testing, aborting the process is unwanted. Module ``hpy.debug`` exposes the
+``LeakDetector`` class to detect leaked ``HPy`` handles. For example:
 
 .. literalinclude:: examples/tests.py
   :language: python
   :start-at: def test_leak_detector
   :end-before: # END: test_leak_detector
 
-Additionally, the debug module also exposes pytest fixture ``hpy_debug`` that
-, for the time being, enables the ``LeakDetector``, but may also enable other
-useful debugging facilities.
+Additionally, the debug module also provides a pytest fixture, ``hpy_debug``,
+that for the time being, enables the ``LeakDetector``. In the future, it
+may also enable other useful debugging facilities.
 
 .. literalinclude:: examples/tests.py
   :language: python
   :start-at: from hpy.debug.pytest import hpy_debug
   :end-at: # Run some HPy extension code
 
-**ATTENTION**: the usage of ``LeakDetector`` or ``hpy_debug`` by itself does not
-enable the HPy debug mode! If the debug mode is not enabled for any extension,
-then those features do nothing useful (but also nothing harmful).
+.. warning:: The usage of ``LeakDetector`` or ``hpy_debug`` by itself does not
+    enable HPy debug mode! If debug mode is not enabled for any extension, then
+    those features have no effect.
 
 When dealing with handle leaks, it is useful to get a stack trace of the
 allocation of the leaked handle. This feature has large memory requirements
 and is therefore opt-in. It can be activated by:
 
 .. literalinclude:: examples/tests.py
   :language: python
@@ -98,19 +110,20 @@
 and disabled by:
 
 .. literalinclude:: examples/tests.py
   :language: python
   :start-at: hpy.debug.disable_handle_stack_traces
   :end-at: hpy.debug.disable_handle_stack_traces
 
-.. Note: the following output is tested in test_leak_detector_with_traces_output
 
 Example
 -------
 
+.. note: The following output is tested in test_leak_detector_with_traces_output
+
 Following HPy function leaks a handle:
 
 .. literalinclude:: examples/snippets/snippets.c
   :start-after: // BEGIN: test_leak_stacktrace
   :end-before: // END: test_leak_stacktrace
 
 When this script is executed in debug mode:
```

### Comparing `hpy-0.0.4/docs/examples/mixed-example/mixed.c` & `hpy-0.9.0rc1/docs/examples/mixed-example/mixed.c`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
  * At the moment, this code is not referenced from the documentation, but it is
  * tested nonetheless.
  */
 
 #include "hpy.h"
 
 /* a HPy style function */
-HPyDef_METH(add_ints, "add_ints", add_ints_impl, HPyFunc_VARARGS)
-static HPy add_ints_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(add_ints, "add_ints", HPyFunc_VARARGS)
+static HPy add_ints_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     long a, b;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 
@@ -35,24 +35,15 @@
 
 static PyMethodDef py_defines[] = {
     {"add_ints_legacy", add_ints2, METH_VARARGS, "add two ints"},
     {NULL, NULL, 0, NULL}    /* Sentinel */
 };
 
 static HPyModuleDef moduledef = {
-    .name = "mixed",
     .doc = "HPy Example of mixing CPython API and HPy API",
-    .size = -1,
+    .size = 0,
     .defines = hpy_defines,
     .legacy_methods = py_defines
 };
 
 
-HPy_MODINIT(mixed)
-static HPy init_mixed_impl(HPyContext *ctx)
-{
-    HPy m;
-    m = HPyModule_Create(ctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-    return m;
-}
+HPy_MODINIT(mixed, moduledef)
```

### Comparing `hpy-0.0.4/docs/examples/simple-example/simple.c` & `hpy-0.9.0rc1/docs/examples/simple-example/simple.c`

 * *Files 20% similar despite different names*

```diff
@@ -4,35 +4,40 @@
  * initialization, the module definition, and the setup.py script, so there is
  * no room left for mixing these code snippets with other code snippets.
  */
 
 // BEGIN: myabs
 #include "hpy.h"
 
-HPyDef_METH(myabs, "myabs", myabs_impl, HPyFunc_O)
+HPyDef_METH(myabs, "myabs", HPyFunc_O)
 static HPy myabs_impl(HPyContext *ctx, HPy self, HPy arg)
 {
     return HPy_Absolute(ctx, arg);
 }
 // END: myabs
 
+// BEGIN: double
+HPyDef_METH_IMPL(double_num, "double", double_impl, HPyFunc_O)
+static HPy double_impl(HPyContext *ctx, HPy self, HPy arg)
+{
+    return HPy_Add(ctx, arg, arg);
+}
+// END: double
+
 // BEGIN: methodsdef
 static HPyDef *SimpleMethods[] = {
         &myabs,
+        &double_num,
         NULL,
 };
 
 static HPyModuleDef simple = {
-        .name = "simple",
         .doc = "HPy Example",
-        .size = -1,
+        .size = 0,
         .defines = SimpleMethods,
         .legacy_methods = NULL
 };
 // END: methodsdef
 
 // BEGIN: moduledef
-HPy_MODINIT(simple)
-HPy init_simple_impl(HPyContext *ctx) {
-    return HPyModule_Create(ctx, &simple);
-}
+HPy_MODINIT(simple, simple)
 // END: moduledef
```

### Comparing `hpy-0.0.4/docs/examples/snippets/hpyvarargs.c` & `hpy-0.9.0rc1/docs/examples/snippets/hpyvarargs.c`

 * *Files 23% similar despite different names*

```diff
@@ -7,23 +7,23 @@
  * want to show the source code including the HPyDef array initialization, so
  * there is no room left for adding other entry points for other code snippets.
  */
 
 #include "hpy.h"
 
 // This is here to make the module look like an incremental change to simple-example
-HPyDef_METH(myabs, "myabs", myabs_impl, HPyFunc_O)
+HPyDef_METH(myabs, "myabs", HPyFunc_O)
 static HPy myabs_impl(HPyContext *ctx, HPy self, HPy arg)
 {
     return HPy_Absolute(ctx, arg);
 }
 
 // BEGIN: add_ints
-HPyDef_METH(add_ints, "add_ints", add_ints_impl, HPyFunc_VARARGS)
-static HPy add_ints_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(add_ints, "add_ints", HPyFunc_VARARGS)
+static HPy add_ints_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     long a, b;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 // END: add_ints
@@ -32,18 +32,14 @@
 static HPyDef *SimpleMethods[] = {
         &myabs,
         &add_ints,
         NULL,
 };
 // END: methodsdef
 
-static HPyModuleDef simple = {
-        .name = "hpyvarargs",
+static HPyModuleDef def = {
         .doc = "HPy Example of varargs calling convention",
-        .size = -1,
+        .size = 0,
         .defines = SimpleMethods
 };
 
-HPy_MODINIT(hpyvarargs)
-HPy init_hpyvarargs_impl(HPyContext *ctx) {
-    return HPyModule_Create(ctx, &simple);
-}
+HPy_MODINIT(hpyvarargs, def)
```

### Comparing `hpy-0.0.4/docs/examples/snippets/snippets.c` & `hpy-0.9.0rc1/docs/examples/snippets/snippets.c`

 * *Files 10% similar despite different names*

```diff
@@ -25,50 +25,57 @@
 {
     // return x == y; // compilation error!
     return HPy_Is(ctx, x, y);
 }
 // END: is_same_object
 
 // dummy entry point so that we can test the snippets:
-HPyDef_METH(test_foo_and_is_same_object, "test_foo_and_is_same_object",
-            test_foo_and_is_same_object_impl, HPyFunc_VARARGS)
+HPyDef_METH(test_foo_and_is_same_object, "test_foo_and_is_same_object", HPyFunc_VARARGS)
 static HPy test_foo_and_is_same_object_impl(HPyContext *ctx, HPy self,
-                                            HPy *args, HPy_ssize_t nargs)
+                                            const HPy *args, size_t nargs)
 {
     foo(ctx);   // not much we can test here
     return HPyLong_FromLong(ctx, is_same_object(ctx, args[0], args[1]));
 }
 
 // BEGIN: test_leak_stacktrace
-HPyDef_METH(test_leak_stacktrace, "test_leak_stacktrace",
-            test_leak_stacktrace_impl, HPyFunc_NOARGS)
+HPyDef_METH(test_leak_stacktrace, "test_leak_stacktrace", HPyFunc_NOARGS)
 static HPy test_leak_stacktrace_impl(HPyContext *ctx, HPy self)
 {
     HPy num = HPyLong_FromLong(ctx, 42);
     if (HPy_IsNull(num)) {
         return HPy_NULL;
     }
     // No HPy_Close(ctx, num);
     return HPy_Dup(ctx, ctx->h_None);
 }
 // END: test_leak_stacktrace
 
+// BEGIN: add
+HPyDef_METH(add, "add", HPyFunc_VARARGS)
+static HPy add_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
+{
+    if (nargs != 2) {
+        HPyErr_SetString(ctx, ctx->h_TypeError, "expected exactly two args");
+        return HPy_NULL;
+    }
+    return HPy_Add(ctx, args[0], args[1]);
+}
+// END: add
+
 // ------------------------------------
 // Dummy module definition, so that we can test the snippets
 
 static HPyDef *Methods[] = {
         &test_foo_and_is_same_object,
         &test_leak_stacktrace,
+        &add,
         NULL,
 };
 
 static HPyModuleDef snippets = {
-        .name = "snippets",
         .doc = "Various HPy code snippets for the docs",
-        .size = -1,
+        .size = 0,
         .defines = Methods
 };
 
-HPy_MODINIT(snippets)
-HPy init_snippets_impl(HPyContext *ctx) {
-    return HPyModule_Create(ctx, &snippets);
-}
+HPy_MODINIT(snippets, snippets)
```

### Comparing `hpy-0.0.4/docs/index.rst` & `hpy-0.9.0rc1/docs/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -4,48 +4,74 @@
    contain the root `toctree` directive.
 
 HPy: a better API for Python
 ===============================
 
 HPy provides a new API for extending Python in C.
 
-The official `Python/C API <https://docs.python.org/3/c-api/index.html>`_ is
+There are several advantages to writing C extensions in HPy:
+
+  - **Speed**: it runs much faster on PyPy, GraalPy, and at native speed on CPython
+
+  - **Deployment**: it is possible to compile a single binary which runs unmodified on all
+    supported Python implementations and versions -- think "stable ABI" on steroids
+
+  - **Simplicity**: it is simpler and more manageable than the ``Python.h`` API, both for
+    the users and the Pythons implementing it
+
+  - **Debugging**: it provides an improved debugging experience. Debug mode can be turned
+    on at runtime without the need to recompile the extension or the Python running it.
+    HPy design is more suitable for automated checks.
+
+The official `Python/C API <https://docs.python.org/3/c-api/index.html>`_,
+also informally known as ``#include <Python.h>``, is
 specific to the current implementation of CPython: it exposes a lot of
-internal details which makes it hard:
+internal details which makes it hard to:
+
+  - implement it for other Python implementations (e.g. PyPy, GraalPy,
+    Jython, ...)
+
+  - experiment with new approaches inside CPython itself, for example:
 
-  - to implement it for other Python implementations (e.g. PyPy, GraalPython,
-    Jython, IronPython, etc.)
+    - use a tracing garbage collection instead of reference counting
+    - remove the global interpreter lock (GIL) to take full advantage of multicore architectures
+    - use tagged pointers to reduce memory footprint
 
-  - to experiment with new things inside CPython itself: e.g. using a GC
-    instead of refcounting, or to remove the GIL.
+Where to go next:
+-----------------
 
-There are several advantages to write your C extension in HPy:
+  - Show me the code:
 
-  - it runs much faster on PyPy, GraalPython, and at native speed on CPython
+      - :doc:`Quickstart<quickstart>`
+      - :ref:`Simple documented HPy extension example<simple example>`
+      - :doc:`Tutorial: porting Python/C API extension to HPy<porting-example/index>`
 
-  - it is possible to compile a single binary which runs unmodified on all
-    supported Python implementations and versions
+  - Details:
 
-  - it is simpler and more manageable than the Python/C API
+      - :doc:`HPy overview: motivation, goals, current status<overview>`
+      - :doc:`HPy API concepts introduction<api>`
+      - :doc:`Python/C API to HPy Porting guide<porting-guide>`
+      - :doc:`HPy API reference<api-reference/index>`
 
-  - it provides an improved debugging experience: in "debug mode", HPy
-    actively checks for many common mistakes such as reference leaks and
-    invalid usage of objects after they have been deleted. It is possible to
-    turn the "debug mode" on at startup time, without needing to recompile
-    Python or the extension itself
 
+Full table of contents:
+-----------------------
 
 .. toctree::
    :maxdepth: 2
 
+   quickstart
    overview
    api
    porting-guide
+   porting-example/index
    debug-mode
+   trace-mode
    api-reference/index
+   contributing/index
    misc/index
    changelog
 
 
 Indices and tables
 ==================
```

### Comparing `hpy-0.0.4/docs/leysin-2020-design-decisions.md` & `hpy-0.9.0rc1/docs/leysin-2020-design-decisions.md`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/docs/module-state.txt` & `hpy-0.9.0rc1/docs/module-state.txt`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/docs/overview.rst` & `hpy-0.9.0rc1/docs/overview.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,72 @@
-HPy overview
-=============
+HPy Overview
+============
 
 Motivation and goals
 ---------------------
 
-The biggest quality of the Python ecosystem is to have a huge number of high
-quality libraries for all kind of jobs. Many of them, especially in the
-scientific community, are written in C and exposed to Python using the
-`Python/C API <https://docs.python.org/3/c-api/index.html>`_.  However, the
-Python/C API exposes a number of CPython's implementation details and
-low-level data structure layouts. This has two important consequences:
-
-  1. any alternative implementation which wants to support C extensions needs
-     to either follow the same low-level layout or to provide a compatibility
-     layer.
+The superpower of the Python ecosystem is its libraries, which are developed by
+users. Over time, these libraries have grown in number, quality, and
+applicability. While it is possible to write python libraries entirely in
+python, many of them, especially in the scientific community, are written in C
+and exposed to Python using the `Python.h API
+<https://docs.python.org/3/c-api/index.html>`_. The existence of these C
+extensions using the ``Python.h`` API leads to some issues:
+
+  1. Usually, alternative implementation of the Python programming language
+     want to support C extensions. To do so, they must implement the same
+     ``Python.h`` API or provide a compatibility layer.
 
   2. CPython developers cannot experiment with new designs or refactoring
      without breaking compatibility with existing extensions.
 
-Over the years, it has become evident that emulating the Python/C
-API in an efficient way is `challenging, if not impossible
+Over the years, it has become evident that emulating ``Python.h`` in an
+efficient way is `challenging, if not impossible
 <https://www.pypy.org/posts/2018/09/inside-cpyext-why-emulating-cpython-c-8083064623681286567.html>`_.
-The main goal of HPy is provide a **C API which is possible to implement in an
-efficient way on a number of very diverse implementations**.  The following is
-a list of sub-goals.
+To summarize, it is mainly due to leaking of implementation details of CPython
+into the C/API - which makes it difficult to make different design choices than
+those made by CPython. As such - the main goal of HPy is to provide a **C API
+which makes as few assumptions as possible about the design decisions of any
+implementation of Python, allowing diverse implementations to support it
+efficiently and without compromise**. In particular, **reference counting is not
+part of the API**: we want a more generic way of managing resources that is
+possible to implement with different strategies, including the existing
+reference counting and/or with a moving *Garbage Collector* (like the ones used
+by PyPy, GraalPy or Java, for example). Moreover, each implementation can
+experiment with new memory layout of objects, add optimizations, etc. The
+following is a list of sub-goals.
+
 
 Performance on CPython
   HPy is usable on CPython from day 1 with no performance impact compared to
-  the existing Python/C API.
+  the existing ``Python.h`` API.
 
 
 Incremental adoption
   It is possible to port existing C extensions piece by piece and to use
   the old and the new API side-by-side during the transition.
 
 
 Easy migration
   It should be easy to migrate existing C extensions to HPy. Thanks to an
   appropriate and regular naming convention it should be obvious what the
-  HPy equivalent of any existing Python/C API is. When a perfect replacement
+  HPy equivalent of any existing ``Python.h`` API is. When a perfect replacement
   does not exist, the documentation explains what the alternative options are.
 
 
 Better debugging
   In debug mode, you get early and precise errors and warnings when you make
   some specific kind of mistakes and/or violate the API rules and
   assumptions. For example, you get an error if you try to use a handle
   (see :ref:`api:handles`) which has already been closed. It is possible to
   turn on the debug mode at startup time, *without needing to recompile*.
 
-
-Hide internal details
-  The API is designed to allow a lot of flexibility for Python
-  implementations, allowing the possibility to explore different choices to
-  the ones used by CPython.  In particular, **reference counting is not part
-  of the API**: we want a more generic way of managing resources which is
-  possible to implement with different strategies, including the existing
-  reference counting and/or with a moving *Garbage Collector* (like the ones
-  used by PyPy, GraalPython or Java, for example).
-
-  Moreover, we want to avoid exposing internal details of a specific
-  implementation, so that each implementation can experiment with new memory
-  layout of objects, add optimizations, etc.
-
-
 Simplicity
   The HPy API aims to be smaller and easier to study/use/manage than the
-  existing Python/C API. Sometimes there is a trade-off between this goal and
+  existing ``Python.h`` API. Sometimes there is a trade-off between this goal and
   the others above, in particular *Performance on CPython* and *Easy migration*.
   The general approach is to have an API which is "as simple as possible" while
   not violating the other goals.
 
 
 Universal binaries
   It is possible to compile extensions to a single binary which is
@@ -102,68 +98,107 @@
     operating system it defines things like the set of exported symbols, the
     precise memory layout of objects, the size of types, etc.
 
 In general it is possible to compile the same source into multiple compiled
 libraries, each one targeting a different ABI. :pep:`3149` states that the
 filename of the compiled extension should contain the *ABI tag* to specify
 what the target ABI is. For example, if you compile an extension called
-``simple.c`` on CPython 3.7, you get a DLL called
-``simple.cpython-37m-x86_64-linux-gnu.so``:
+``simple.c`` on CPython 3.8, you get a DLL called
+``simple.cpython-38-x86_64-linux-gnu.so``:
 
-  - ``cpython-37m`` is the ABI tag, in this case CPython 3.7
+  - ``cpython-38`` is the ABI tag, in this case CPython 3.8
 
   - ``x86_64`` is the CPU architecture
 
   - ``linux-gnu`` is the operating system
 
 The same source code compiled on PyPy3.6 7.2.0 results in a file called
-``simple.pypy3-72-x86_64-linux-gnu.so``:
+``simple.pypy38-pp73-x86_64-linux-gnu.so``:
 
-  - ``pypy3-72`` is the ABI tag, in this case "PyPy3.x", version "7.2.x"
+  - ``pypy38-pp73`` is the ABI tag, in this case "PyPy3.8", version "7.3.x"
 
 The HPy C API is exposed to the user by including ``hpy.h`` and it is
 explained in its own section of the documentation.
 
 
+Legacy and compatibility features
+---------------------------------
+
+To allow an incremental transition to HPy, it is possible to use both
+``hpy.h`` and ``Python.h`` API calls in the same extension.  Using *HPy legacy
+features* you can:
+
+  - mix ``Python.h`` and HPy method defs in the same HPy module
+
+  - mix ``Python.h`` and HPy method defs and slots in the same HPy type
+
+  - convert ``HPy`` handles to and from ``PyObject *`` using
+    ``HPy_AsPyObject()`` and ``HPy_FromPyObject()``
+
+
+Thanks to this, you can port your code to HPy one method and one type at a
+time, while keeping the extension fully functional during the transition
+period. See the :ref:`porting-guide:Porting guide` for a concrete example.
+
+Legacy features are available only if you target the CPython or HPy Hybrid
+ABIs, as explained in the next section.
+
+
 .. _hpy-target-abis:
 
 Target ABIs
 -----------
 
-Depending on the compilation options, and HPy extension can target three
+Depending on the compilation options, an HPy extension can target three
 different ABIs:
 
 .. glossary::
 
     CPython ABI
       In this mode, HPy is implemented as a set of C macros and ``static inline``
       functions which translate the HPy API into the CPython API at compile
       time. The result is a compiled extension which is indistinguishable from a
       "normal" one and can be distributed using all the standard tools and will
-      run at the very same speed. The ABI tag is defined by the version of CPython
-      which is used to compile it (e.g., ``cpython-37m``),
+      run at the very same speed.
+
+      *Legacy features* are available.
+
+      The output filename is e.g. ``simple.cpython-38-x86_64-linux-gnu.so``.
+
 
     HPy Universal ABI
       As the name suggests, the HPy Universal ABI is designed to be loaded and
       executed by a variety of different Python implementations. Compiled
-      extensions can be loaded unmodified on all the interpreters which supports
-      it.  PyPy and GraalPython support it natively.  CPython supports it by using the
-      ``hpy.universal`` package, and there is a small speed penalty compared to
-      the CPython ABI.  The ABI tag has not been formally defined yet.
+      extensions can be loaded unmodified on all the interpreters which support
+      it. PyPy and GraalPy support it natively. CPython supports it by using the
+      ``hpy.universal`` package, and there is a small speed penalty [#f1]_ compared to
+      the CPython ABI.
+
+      *Legacy features* are **not** available and it is forbidden to ``#include <Python.h>``.
+
+      The resulting filename is e.g. ``simple.hpy0.so``.
 
     HPy Hybrid ABI
-      To allow an incremental transition to HPy, it is possible to use both HPy
-      and Python/C API calls in the same extension. In this case, it is not
-      possible to target the Universal ABI because the resulting compiled library
-      also needs to be compatible with a specific CPython version. The ABI tag
-      will be something like ``hpy-1_cpython-37m``. Note: the tag is not implemented
-      yet. Currently, the approach to use HPy in hybrid mode is to build the extension
-      in HPy universal mode, which, for now, still allows mixing the HPy and CPython APIs.
-      Extensions mixing the HPy and CPython APIs will not work on Pythons that do not
-      support the hybrid ABI.
+
+      The HPy Hybrid ABI is essentially the same as the Universal ABI, with
+      the big difference that it allows to ``#include <Python.h>``, to use the
+      legacy features and thus to allow incremental porting.
+
+      At the ABI level the resulting binary depends on *both* HPy and the
+      specific Python implementation which was used to compile the extension.
+      As the name suggests, this means that the binary is not "universal",
+      thus negating some of the benefits of HPy.  The main benefit of using
+      the HPy Hybrid ABI instead of the CPython ABI is being able to use the
+      :ref:`debug-mode:Debug mode` on the HPy parts, and faster speed on
+      alternative implementations.
+
+      *Legacy features* are available.
+
+      The resulting filename is e.g. ``simple.hpy0-cp38.so``.
+
 
 Moreover, each alternative Python implementation could decide to implement its
 own non-universal ABI if it makes sense for them. For example, a hypothetical
 project *DummyPython* could decide to ship its own ``hpy.h`` which implements
 the HPy API but generates a DLL which targets the DummyPython ABI.
 
 This means that to compile an extension for CPython, you can choose whether to
@@ -177,39 +212,48 @@
 
 From the user point of view, extensions compiled for the CPython ABI can be
 distributed and installed as usual, while those compiled for the HPy Universal
 or HPy Hybrid ABIs require installing the ``hpy.universal`` package on
 CPython and have no further requirements on Pythons that support HPy natively.
 
 
-C extensions
-------------
+Benefits for the Python ecosystem
+---------------------------------
 
-If you are writing a Python extension in C, you are a consumer of the HPy
-API. There are three big advantages in using HPy instead of the old Python/C
-API:
-
-  - Speed on PyPy, GraalPython and other alternative implementations: according
-    to early :ref:`benchmarks`, an extension written in HPy can be ~3x faster
-    than the equivalent extension written in Python/C.
+The HPy project offers some benefits to the python ecosystem, both to Python
+users and to library developers.
 
+  - C extensions can achieve much better speed on alternative implementions,
+    including PyPy and GraalPy: according to early :ref:`benchmarks`, an
+    extension written in HPy can be ~3x faster than the equivalent extension
+    written using ``Python.h``.
   - Improved debugging: when you load extensions in :ref:`debug-mode:debug mode`,
     many common mistakes are checked and reported automatically.
-
-  - Universal binaries: you can choose to distribute only Universal ABI
-    binaries. This comes with a small speed penalty on CPython, but for
+  - Universal binaries: libraries can choose to distribute only Universal ABI
+    binaries. By doing so, they can support all Python implementations and
+    version of CPython (like PyPy, GraalPy, CPython 3.10, CPython 3.11, etc)
+    for which an HPy loader exists, including those that do not yet exist! This
+    currently comes with a small speed penalty on CPython, but for
     non-performance critical libraries it might still be a good tradeoff.
+  - Python environments: With general availability of universal ABI binaries for
+    popular packages, users can create equivalent python environments that
+    target different Python implementations. Thus, Python users can try their
+    workload against different implementations and pick the one best suited for
+    their usage.
+  - In a situation where most or all popular Python extensions target the
+    universal ABI, it will be more feasible for CPython to make breaking changes
+    to its C/API for performance or maintainability reasons.
 
 
 Cython extensions
 -----------------
 
 If you use Cython, you can't use HPy directly. There is a
 `work in progress <https://github.com/cython/cython/pull/4490>`_ to
-add Cython backend which emits HPy code instead of Python/C code: once this is
+add Cython backend which emits HPy code instead of using ``Python.h`` code: once this is
 done, you will get the benefits of HPy automatically.
 
 
 Extensions in other languages
 -----------------------------
 
 On the API side, HPy is designed with C in mind, so it is not directly useful
@@ -222,83 +266,91 @@
 <https://github.com/pyhandle/rust-hpy>`_.
 
 
 Benefits for alternative Python implementations
 -----------------------------------------------
 
 If you are writing an alternative Python implementation, there is a good
-chance that you already know how painful it is to support the Python/C
-API. HPy is designed to be both faster and easier to implement!
+chance that you already know how painful it is to support the ``Python.h`` API.
+HPy is designed to be both faster and easier to implement!
 
 You have two choices:
 
   - support the Universal ABI: in this case, you just need to export the
     needed functions and to add a hook to ``dlopen()`` the desired libraries
 
   - use a custom ABI: in this case, you have to write your own replacement for
     ``hpy.h`` and recompile the C extensions with it.
 
 
 Current status and roadmap
 --------------------------
 
-HPy is still in the early stages of development, but many big pieces are
-already in place. As on April 2022, the following milestones have been reached:
+HPy left the early stages of development and already provides a noticeable set
+of features. As on April 2023, the following milestones have been reached:
 
-  - some real-world Python packages have been ported to HPy API.
-    The ports will be published soon.
+  - some prominent real-world Python packages have been ported to HPy API. There
+    is a list of HPy-compatible packages we know about on the HPy website
+    `hpyproject.org <https://hpyproject.org/>`_.
 
   - one can write extensions which expose module-level functions, with all
     the various kinds of calling conventions.
 
   - there is support for argument parsing (i.e., the equivalents of
-    `PyArg_ParseTuple` and `PyArg_ParseTupleAndKeywords`), and a
-    convenient complex value building (i.e., the equivalent `Py_BuildValue`).
+    ``PyArg_ParseTuple`` and ``PyArg_ParseTupleAndKeywords``), and a
+    convenient complex value building (i.e., the equivalent ``Py_BuildValue``).
 
   - one can implement custom types, whose struct may contain references to other
-    Python objects using `HPyField`.
+    Python objects using ``HPyField``.
 
-  - there is a support for globally accessible Python object handles: `HPyGlobal`,
+  - there is a support for globally accessible Python object handles: ``HPyGlobal``,
     which can still provide isolation for subinterpreters if needed.
 
   - there is support for raising and catching exceptions.
 
   - debug mode has been implemented and can be activated at run-time without
     recompiling. It can detect leaked handles or handles used after
     being closed.
 
-  - wheels can be build for HPy extensions with `python setup.py bdist_wheel`
-    and can be installed with `pip install`.
+  - trace mode has been implemented and can be activated just like the debug
+    mode. It helps analyzing the API usage (in particular wrt. performance).
+
+  - wheels can be built for HPy extensions with ``python setup.py bdist_wheel``
+    and can be installed with ``pip install``.
 
   - it is possible to choose between the :term:`CPython ABI` and the
     :term:`HPy Universal ABI` when compiling an extension module.
 
   - extensions compiled with the CPython ABI work out of the box on
     CPython.
 
   - it is possible to load HPy Universal extensions on CPython, thanks to the
     ``hpy.universal`` package.
 
   - it is possible to load HPy Universal extensions on
     PyPy (using the PyPy `hpy branch <https://foss.heptapod.net/pypy/pypy/tree/branch/hpy>`_).
 
-  - it is possible to load HPy Universal extensions on `GraalPython
+  - it is possible to load HPy Universal extensions on `GraalPy
     <https://github.com/graalvm/graalpython>`_.
 
+  - there is support for multi-phase module initialization.
+
+  - support for metaclasses has been added.
+
 
 However, there is still a long road before HPy is usable for the general
 public. In particular, the following features are on our roadmap but have not
 been implemented yet:
 
-  - many of the original Python/C functions have not been ported to
+  - many of the original ``Python.h`` functions have not been ported to
     HPy yet. Porting most of them is straightforward, so for now the priority
     is to test HPy with real-world Python packages and primarily resolve the
     "hard" features to prove that the HPy approach works.
 
-  - add C-level module state to complement the `HPyGlobal` approach. While `HPyGlobal`
+  - add C-level module state to complement the ``HPyGlobal`` approach. While ``HPyGlobal``
     is easier to use, it will make the migration simpler for existing extensions that
     use CPython module state.
 
   - the integration with Cython is work in progress
 
   - it is not clear yet how to approach pybind11 and similar C++ bindings. They serve two use-cases:
 
@@ -342,44 +394,51 @@
     even bigger speedups eventually.
 
 
 Projects involved
 -----------------
 
 HPy was born during EuroPython 2019, were a small group of people started to
-discuss the problems of the Python/C API and how it would be nice to
+discuss the problems of the ``Python.h`` API and how it would be nice to
 have a way to fix them.  Since then, it has gathered the attention and interest
 of people who are involved in many projects within the Python ecosystem.  The
 following is a (probably incomplete) list of projects whose core developers
 are involved in HPy, in one way or the other.  The mere presence in this list
 does not mean that the project as a whole endorse or recognize HPy in any way,
 just that some of the people involved contributed to the
 code/design/discussions of HPy:
 
   - PyPy
 
   - CPython
 
   - Cython
 
-  - GraalPython
+  - GraalPy
 
   - RustPython
 
   - rust-hpy (fork of the `cpython crate <https://crates.io/crates/cpython>`_)
 
 
-
-
 Related work
 -------------
 
-A partial list of alternative implementations which offer a Python/C
+A partial list of alternative implementations which offer a ``Python.h``
 compatibility layer include:
 
   - `PyPy <https://doc.pypy.org/en/latest/faq.html#do-cpython-extension-modules-work-with-pypy>`_
 
   - `Jython <https://www.jyni.org/>`_
 
   - `IronPython <https://github.com/IronLanguages/ironclad>`_
 
-  - `GraalPython <https://github.com/graalvm/graalpython>`_
+  - `GraalPy <https://github.com/graalvm/graalpython>`_
+
+.. rubric:: Footnotes
+
+.. [#f1] The reason for this minor performance penalty is a layer of pointer
+  indirection. For instance, ``ctx->HPyLong_FromLong`` is called from the
+  CPython extension, which in universal mode simply forwards the call to
+  ``PyLong_FromLong``. It is technically possible to implement a CPython
+  universal module loader which edits the program's executable code at runtime
+  to replace that call. Note that this is not at all trivial.
```

### Comparing `hpy-0.0.4/docs/xxx-unsorted-notes.txt` & `hpy-0.9.0rc1/docs/xxx-unsorted-notes.txt`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/debug/leakdetector.py` & `hpy-0.9.0rc1/hpy/debug/leakdetector.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/debug/pytest.py` & `hpy-0.9.0rc1/hpy/debug/pytest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/debug/src/_debugmod.c` & `hpy-0.9.0rc1/hpy/debug/src/_debugmod.c`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 #include "hpy.h"
 #include "debug_internal.h"
 
 static UHPy new_DebugHandleObj(HPyContext *uctx, UHPy u_DebugHandleType,
                                DebugHandle *handle);
 
+HPY_MOD_EMBEDDABLE(_trace)
 
-HPyDef_METH(new_generation, "new_generation", new_generation_impl, HPyFunc_NOARGS)
+HPyDef_METH(new_generation, "new_generation", HPyFunc_NOARGS)
 static UHPy new_generation_impl(HPyContext *uctx, UHPy self)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     info->current_generation++;
     return HPyLong_FromLong(uctx, info->current_generation);
 }
 
 static UHPy build_list_of_handles(HPyContext *uctx, UHPy u_self, DHQueue *q,
                                   long gen)
@@ -31,59 +34,63 @@
     if (HPy_IsNull(u_DebugHandleType))
         goto error;
 
     u_result = HPyList_New(uctx, 0);
     if (HPy_IsNull(u_result))
         goto error;
 
-    DebugHandle *dh = q->head;
-    while(dh != NULL) {
+    DHQueueNode *node = q->head;
+    while(node != NULL) {
+        DebugHandle *dh = (DebugHandle *)node;
         if (dh->generation >= gen) {
             UHPy u_item = new_DebugHandleObj(uctx, u_DebugHandleType, dh);
             if (HPy_IsNull(u_item))
                 goto error;
             if (HPyList_Append(uctx, u_result, u_item) == -1)
                 goto error;
             HPy_Close(uctx, u_item);
         }
-        dh = dh->next;
+        node = node->next;
     }
 
     HPy_Close(uctx, u_DebugHandleType);
     return u_result;
 
  error:
     HPy_Close(uctx, u_DebugHandleType);
     HPy_Close(uctx, u_result);
     HPy_Close(uctx, u_item);
     return HPy_NULL;
 }
 
 
-HPyDef_METH(get_open_handles, "get_open_handles", get_open_handles_impl, HPyFunc_O, .doc=
+HPyDef_METH(get_open_handles, "get_open_handles", HPyFunc_O, .doc=
             "Return a list containing all the open handles whose generation is >= "
             "of the given arg")
 static UHPy get_open_handles_impl(HPyContext *uctx, UHPy u_self, UHPy u_gen)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
 
     long gen = HPyLong_AsLong(uctx, u_gen);
     if (HPyErr_Occurred(uctx))
         return HPy_NULL;
 
     return build_list_of_handles(uctx, u_self, &info->open_handles, gen);
 }
 
-HPyDef_METH(get_closed_handles, "get_closed_handles", get_closed_handles_impl,
-            HPyFunc_VARARGS, .doc=
-            "Return a list of all the closed handle in the cache")
-static UHPy get_closed_handles_impl(HPyContext *uctx, UHPy u_self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(get_closed_handles, "get_closed_handles", HPyFunc_VARARGS,
+            .doc="Return a list of all the closed handle in the cache")
+static UHPy get_closed_handles_impl(HPyContext *uctx, UHPy u_self, const HPy *args, size_t nargs)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     long gen = 0;
     if (nargs > 0) {
         if (nargs != 1) {
             HPyErr_SetString(uctx, uctx->h_TypeError,
                              "get_closed_handles expects no arguments or exactly one argument");
             return HPy_NULL;
@@ -91,84 +98,107 @@
         gen = HPyLong_AsLong(uctx, args[0]);
         if (HPyErr_Occurred(uctx))
             return HPy_NULL;
     }
     return build_list_of_handles(uctx, u_self, &info->closed_handles, gen);
 }
 
-HPyDef_METH(get_closed_handles_queue_max_size, "get_closed_handles_queue_max_size",
-            get_closed_handles_queue_max_size_impl, HPyFunc_NOARGS, .doc=
-            "Return the maximum size of the closed handles queue")
+HPyDef_METH(get_closed_handles_queue_max_size, "get_closed_handles_queue_max_size", HPyFunc_NOARGS,
+            .doc="Return the maximum size of the closed handles queue")
 static UHPy get_closed_handles_queue_max_size_impl(HPyContext *uctx, UHPy u_self)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     return HPyLong_FromSsize_t(uctx, info->closed_handles_queue_max_size);
 }
 
-HPyDef_METH(set_closed_handles_queue_max_size, "set_closed_handles_queue_max_size",
-            set_closed_handles_queue_max_size_impl, HPyFunc_O, .doc=
-            "Set the maximum size of the closed handles queue")
+HPyDef_METH(set_closed_handles_queue_max_size, "set_closed_handles_queue_max_size", HPyFunc_O,
+            .doc="Set the maximum size of the closed handles queue")
 static UHPy set_closed_handles_queue_max_size_impl(HPyContext *uctx, UHPy u_self, UHPy u_size)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     HPy_ssize_t size = HPyLong_AsSize_t(uctx, u_size);
     if (HPyErr_Occurred(uctx))
         return HPy_NULL;
     info->closed_handles_queue_max_size = size;
     return HPy_Dup(uctx, uctx->h_None);
 }
 
-HPyDef_METH(get_protected_raw_data_max_size, "get_protected_raw_data_max_size",
-get_protected_raw_data_max_size_impl, HPyFunc_NOARGS, .doc=
-"Return the maximum size of the retained raw memory associated with closed handles")
+HPyDef_METH(get_protected_raw_data_max_size, "get_protected_raw_data_max_size", HPyFunc_NOARGS,
+            .doc="Return the maximum size of the retained raw memory associated with closed handles")
 static UHPy get_protected_raw_data_max_size_impl(HPyContext *uctx, UHPy u_self)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     return HPyLong_FromSsize_t(uctx, info->protected_raw_data_max_size);
 }
 
-HPyDef_METH(set_protected_raw_data_max_size, "set_protected_raw_data_max_size",
-set_protected_raw_data_max_size_impl, HPyFunc_O, .doc=
-"Set the maximum size of the retained raw memory associated with closed handles")
+HPyDef_METH(set_protected_raw_data_max_size, "set_protected_raw_data_max_size", HPyFunc_O,
+            .doc="Set the maximum size of the retained raw memory associated with closed handles")
 static UHPy set_protected_raw_data_max_size_impl(HPyContext *uctx, UHPy u_self, UHPy u_size)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     HPy_ssize_t size = HPyLong_AsSize_t(uctx, u_size);
     if (HPyErr_Occurred(uctx))
         return HPy_NULL;
     info->protected_raw_data_max_size = size;
     return HPy_Dup(uctx, uctx->h_None);
 }
 
-HPyDef_METH(set_on_invalid_handle, "set_on_invalid_handle", set_on_invalid_handle_impl,
-            HPyFunc_O, .doc=
-            "Set the function to call when we detect the usage of an invalid handle")
+HPyDef_METH(set_on_invalid_handle, "set_on_invalid_handle", HPyFunc_O,
+            .doc="Set the function to call when we detect the usage of an invalid handle")
 static UHPy set_on_invalid_handle_impl(HPyContext *uctx, UHPy u_self, UHPy u_arg)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPyDebugInfo *info = get_info(dctx);
     if (HPy_Is(uctx, u_arg, uctx->h_None)) {
         info->uh_on_invalid_handle = HPy_NULL;
     } else if (!HPyCallable_Check(uctx, u_arg)) {
         HPyErr_SetString(uctx, uctx->h_TypeError, "Expected a callable object");
         return HPy_NULL;
     } else {
         info->uh_on_invalid_handle = HPy_Dup(uctx, u_arg);
     }
     return HPy_Dup(uctx, uctx->h_None);
 }
 
-HPyDef_METH(set_handle_stack_trace_limit, "set_handle_stack_trace_limit",
-            set_handle_stack_trace_limit_impl, HPyFunc_O, .doc=
-                    "Set the limit to captured HPy handles allocations stack traces. "
-                    "None means do not capture the stack traces.")
+HPyDef_METH(set_on_invalid_builder_handle, "set_on_invalid_builder_handle", HPyFunc_O,
+            .doc="Set the function to call when we detect the usage of an invalid builder handle")
+static UHPy set_on_invalid_builder_handle_impl(HPyContext *uctx, UHPy u_self, UHPy u_arg)
+{
+    HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
+    HPyDebugInfo *info = get_info(dctx);
+    if (HPy_Is(uctx, u_arg, uctx->h_None)) {
+        info->uh_on_invalid_builder_handle = HPy_NULL;
+    } else if (!HPyCallable_Check(uctx, u_arg)) {
+        HPyErr_SetString(uctx, uctx->h_TypeError, "Expected a callable object");
+        return HPy_NULL;
+    } else {
+        info->uh_on_invalid_builder_handle = HPy_Dup(uctx, u_arg);
+    }
+    return HPy_Dup(uctx, uctx->h_None);
+}
+
+HPyDef_METH(set_handle_stack_trace_limit, "set_handle_stack_trace_limit", HPyFunc_O,
+            .doc="Set the limit to captured HPy handles allocations stack traces. "
+                "None means do not capture the stack traces.")
 static UHPy set_handle_stack_trace_limit_impl(HPyContext *uctx, UHPy u_self, UHPy u_arg)
 {
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
     HPyDebugInfo *info = get_info(dctx);
     if (HPy_Is(uctx, u_arg, uctx->h_None)) {
         info->handle_alloc_stacktrace_limit = 0;
     } else {
@@ -207,70 +237,69 @@
 
 typedef struct {
     DebugHandle *handle;
 } DebugHandleObject;
 
 HPyType_HELPERS(DebugHandleObject)
 
-HPyDef_GET(DebugHandle_obj, "obj", DebugHandle_obj_get,
-           .doc="The object which the handle points to")
+HPyDef_GET(DebugHandle_obj, "obj", .doc="The object which the handle points to")
 static UHPy DebugHandle_obj_get(HPyContext *uctx, UHPy self, void *closure)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
     return HPy_Dup(uctx, dh->handle->uh);
 }
 
-HPyDef_GET(DebugHandle_id, "id", DebugHandle_id_get,
+HPyDef_GET(DebugHandle_id, "id",
            .doc="A numeric identifier representing the underlying universal handle")
 static UHPy DebugHandle_id_get(HPyContext *uctx, UHPy self, void *closure)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
     return HPyLong_FromSsize_t(uctx, (HPy_ssize_t)dh->handle);
 }
 
-HPyDef_GET(DebugHandle_is_closed, "is_closed", DebugHandle_is_closed_get,
+HPyDef_GET(DebugHandle_is_closed, "is_closed",
            .doc="Self-explanatory")
 static UHPy DebugHandle_is_closed_get(HPyContext *uctx, UHPy self, void *closure)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
-    return HPyBool_FromLong(uctx, dh->handle->is_closed);
+    return HPyBool_FromBool(uctx, dh->handle->is_closed);
 }
 
-HPyDef_GET(DebugHandle_raw_data_size, "raw_data_size", DebugHandle_raw_data_size_get,
+HPyDef_GET(DebugHandle_raw_data_size, "raw_data_size",
 .doc="Size of retained raw memory. FOR TESTS ONLY.")
 static UHPy DebugHandle_raw_data_size_get(HPyContext *uctx, UHPy self, void *closure)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
     if (dh->handle->associated_data) {
         return HPyLong_FromSsize_t(uctx, dh->handle->associated_data_size);
     } else {
         return HPyLong_FromLong(uctx, -1);
     }
 }
 
-HPyDef_SLOT(DebugHandle_cmp, DebugHandle_cmp_impl, HPy_tp_richcompare)
+HPyDef_SLOT(DebugHandle_cmp, HPy_tp_richcompare)
 static UHPy DebugHandle_cmp_impl(HPyContext *uctx, UHPy self, UHPy o, HPy_RichCmpOp op)
 {
     UHPy T = HPy_Type(uctx, self);
     if (!HPy_TypeCheck(uctx, o, T))
         return HPy_Dup(uctx, uctx->h_NotImplemented);
     DebugHandleObject *dh_self = DebugHandleObject_AsStruct(uctx, self);
     DebugHandleObject *dh_o = DebugHandleObject_AsStruct(uctx, o);
 
     switch(op) {
     case HPy_EQ:
-        return HPyBool_FromLong(uctx, dh_self->handle == dh_o->handle);
+        return HPyBool_FromBool(uctx, dh_self->handle == dh_o->handle);
     case HPy_NE:
-        return HPyBool_FromLong(uctx, dh_self->handle != dh_o->handle);
+        return HPyBool_FromBool(uctx, dh_self->handle != dh_o->handle);
     default:
         return HPy_Dup(uctx, uctx->h_NotImplemented);
     }
 }
 
-HPyDef_SLOT(DebugHandle_repr, DebugHandle_repr_impl, HPy_tp_repr)
+HPyDef_SLOT(DebugHandle_repr, HPy_tp_repr)
 static UHPy DebugHandle_repr_impl(HPyContext *uctx, UHPy self)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
     UHPy uh_fmt = HPy_NULL;
     UHPy uh_id = HPy_NULL;
     UHPy uh_args = HPy_NULL;
     UHPy uh_result = HPy_NULL;
@@ -321,20 +350,22 @@
     HPy_Close(uctx, uh_args);
     HPy_Close(uctx, h_trace);
     HPy_Close(uctx, h_trace_header);
     return uh_result;
 }
 
 
-HPyDef_METH(DebugHandle__force_close, "_force_close", DebugHandle__force_close_impl,
-            HPyFunc_NOARGS, .doc="Close the underyling handle. FOR TESTS ONLY.")
+HPyDef_METH(DebugHandle__force_close, "_force_close",
+            HPyFunc_NOARGS, .doc="Close the underlying handle. FOR TESTS ONLY.")
 static UHPy DebugHandle__force_close_impl(HPyContext *uctx, UHPy self)
 {
     DebugHandleObject *dh = DebugHandleObject_AsStruct(uctx, self);
     HPyContext *dctx = hpy_debug_get_ctx(uctx);
+    if (dctx == NULL)
+        return HPy_NULL;
     HPy_Close(dctx, as_DHPy(dh->handle));
     return HPy_Dup(uctx, uctx->h_None);
 }
 
 static HPyDef *DebugHandleType_defs[] = {
     &DebugHandle_obj,
     &DebugHandle_id,
@@ -362,42 +393,40 @@
     dhobj->handle = handle;
     return u_result;
 }
 
 
 /* ~~~~~~ definition of the module hpy.debug._debug ~~~~~~~ */
 
+HPyDef_SLOT(module_exec, HPy_mod_exec)
+static int module_exec_impl(HPyContext *uctx, HPy m)
+{
+    UHPy h_DebugHandleType = HPyType_FromSpec(uctx, &DebugHandleType_spec, NULL);
+    if (HPy_IsNull(h_DebugHandleType))
+        return -1;
+    HPy_SetAttr_s(uctx, m, "DebugHandle", h_DebugHandleType);
+    HPy_Close(uctx, h_DebugHandleType);
+    return 0;
+}
+
 static HPyDef *module_defines[] = {
     &new_generation,
     &get_open_handles,
     &get_closed_handles,
     &get_closed_handles_queue_max_size,
     &set_closed_handles_queue_max_size,
     &get_protected_raw_data_max_size,
     &set_protected_raw_data_max_size,
     &set_on_invalid_handle,
+    &set_on_invalid_builder_handle,
     &set_handle_stack_trace_limit,
+    &module_exec,
     NULL
 };
 
 static HPyModuleDef moduledef = {
-    .name = "hpy.debug._debug",
     .doc = "HPy debug mode",
-    .size = -1,
+    .size = 0,
     .defines = module_defines
 };
 
-
-HPy_MODINIT(_debug)
-static UHPy init__debug_impl(HPyContext *uctx)
-{
-    UHPy m = HPyModule_Create(uctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-
-    UHPy h_DebugHandleType = HPyType_FromSpec(uctx, &DebugHandleType_spec, NULL);
-    if (HPy_IsNull(h_DebugHandleType))
-        return HPy_NULL;
-    HPy_SetAttr_s(uctx, m, "DebugHandle", h_DebugHandleType);
-    HPy_Close(uctx, h_DebugHandleType);
-    return m;
-}
+HPy_MODINIT(_debug, moduledef)
```

### Comparing `hpy-0.0.4/hpy/debug/src/autogen_debug_ctx_init.h` & `hpy-0.9.0rc1/hpy/debug/src/autogen_debug_ctx_init.h`

 * *Files 15% similar despite different names*

```diff
@@ -6,36 +6,35 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
-DHPy debug_ctx_Module_Create(HPyContext *dctx, HPyModuleDef *def);
 DHPy debug_ctx_Dup(HPyContext *dctx, DHPy h);
 void debug_ctx_Close(HPyContext *dctx, DHPy h);
-DHPy debug_ctx_Long_FromLong(HPyContext *dctx, long value);
-DHPy debug_ctx_Long_FromUnsignedLong(HPyContext *dctx, unsigned long value);
-DHPy debug_ctx_Long_FromLongLong(HPyContext *dctx, long long v);
-DHPy debug_ctx_Long_FromUnsignedLongLong(HPyContext *dctx, unsigned long long v);
+DHPy debug_ctx_Long_FromInt32_t(HPyContext *dctx, int32_t value);
+DHPy debug_ctx_Long_FromUInt32_t(HPyContext *dctx, uint32_t value);
+DHPy debug_ctx_Long_FromInt64_t(HPyContext *dctx, int64_t v);
+DHPy debug_ctx_Long_FromUInt64_t(HPyContext *dctx, uint64_t v);
 DHPy debug_ctx_Long_FromSize_t(HPyContext *dctx, size_t value);
 DHPy debug_ctx_Long_FromSsize_t(HPyContext *dctx, HPy_ssize_t value);
-long debug_ctx_Long_AsLong(HPyContext *dctx, DHPy h);
-unsigned long debug_ctx_Long_AsUnsignedLong(HPyContext *dctx, DHPy h);
-unsigned long debug_ctx_Long_AsUnsignedLongMask(HPyContext *dctx, DHPy h);
-long long debug_ctx_Long_AsLongLong(HPyContext *dctx, DHPy h);
-unsigned long long debug_ctx_Long_AsUnsignedLongLong(HPyContext *dctx, DHPy h);
-unsigned long long debug_ctx_Long_AsUnsignedLongLongMask(HPyContext *dctx, DHPy h);
+int32_t debug_ctx_Long_AsInt32_t(HPyContext *dctx, DHPy h);
+uint32_t debug_ctx_Long_AsUInt32_t(HPyContext *dctx, DHPy h);
+uint32_t debug_ctx_Long_AsUInt32_tMask(HPyContext *dctx, DHPy h);
+int64_t debug_ctx_Long_AsInt64_t(HPyContext *dctx, DHPy h);
+uint64_t debug_ctx_Long_AsUInt64_t(HPyContext *dctx, DHPy h);
+uint64_t debug_ctx_Long_AsUInt64_tMask(HPyContext *dctx, DHPy h);
 size_t debug_ctx_Long_AsSize_t(HPyContext *dctx, DHPy h);
 HPy_ssize_t debug_ctx_Long_AsSsize_t(HPyContext *dctx, DHPy h);
 void *debug_ctx_Long_AsVoidPtr(HPyContext *dctx, DHPy h);
 double debug_ctx_Long_AsDouble(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Float_FromDouble(HPyContext *dctx, double v);
 double debug_ctx_Float_AsDouble(HPyContext *dctx, DHPy h);
-DHPy debug_ctx_Bool_FromLong(HPyContext *dctx, long v);
+DHPy debug_ctx_Bool_FromBool(HPyContext *dctx, bool v);
 HPy_ssize_t debug_ctx_Length(HPyContext *dctx, DHPy h);
 int debug_ctx_Number_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Add(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_Subtract(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_Multiply(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_MatrixMultiply(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_FloorDivide(HPyContext *dctx, DHPy h1, DHPy h2);
@@ -66,208 +65,242 @@
 DHPy debug_ctx_InPlaceLshift(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_InPlaceRshift(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_InPlaceAnd(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_InPlaceXor(HPyContext *dctx, DHPy h1, DHPy h2);
 DHPy debug_ctx_InPlaceOr(HPyContext *dctx, DHPy h1, DHPy h2);
 int debug_ctx_Callable_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_CallTupleDict(HPyContext *dctx, DHPy callable, DHPy args, DHPy kw);
+DHPy debug_ctx_Call(HPyContext *dctx, DHPy callable, const DHPy *args, size_t nargs, DHPy kwnames);
+DHPy debug_ctx_CallMethod(HPyContext *dctx, DHPy name, const DHPy *args, size_t nargs, DHPy kwnames);
 void debug_ctx_FatalError(HPyContext *dctx, const char *message);
-void debug_ctx_Err_SetString(HPyContext *dctx, DHPy h_type, const char *message);
+void debug_ctx_Err_SetString(HPyContext *dctx, DHPy h_type, const char *utf8_message);
 void debug_ctx_Err_SetObject(HPyContext *dctx, DHPy h_type, DHPy h_value);
 DHPy debug_ctx_Err_SetFromErrnoWithFilename(HPyContext *dctx, DHPy h_type, const char *filename_fsencoded);
 void debug_ctx_Err_SetFromErrnoWithFilenameObjects(HPyContext *dctx, DHPy h_type, DHPy filename1, DHPy filename2);
 int debug_ctx_Err_Occurred(HPyContext *dctx);
 int debug_ctx_Err_ExceptionMatches(HPyContext *dctx, DHPy exc);
 void debug_ctx_Err_NoMemory(HPyContext *dctx);
 void debug_ctx_Err_Clear(HPyContext *dctx);
-DHPy debug_ctx_Err_NewException(HPyContext *dctx, const char *name, DHPy base, DHPy dict);
-DHPy debug_ctx_Err_NewExceptionWithDoc(HPyContext *dctx, const char *name, const char *doc, DHPy base, DHPy dict);
-int debug_ctx_Err_WarnEx(HPyContext *dctx, DHPy category, const char *message, HPy_ssize_t stack_level);
+DHPy debug_ctx_Err_NewException(HPyContext *dctx, const char *utf8_name, DHPy base, DHPy dict);
+DHPy debug_ctx_Err_NewExceptionWithDoc(HPyContext *dctx, const char *utf8_name, const char *utf8_doc, DHPy base, DHPy dict);
+int debug_ctx_Err_WarnEx(HPyContext *dctx, DHPy category, const char *utf8_message, HPy_ssize_t stack_level);
 void debug_ctx_Err_WriteUnraisable(HPyContext *dctx, DHPy obj);
 int debug_ctx_IsTrue(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Type_FromSpec(HPyContext *dctx, HPyType_Spec *spec, HPyType_SpecParam *params);
-DHPy debug_ctx_Type_GenericNew(HPyContext *dctx, DHPy type, DHPy *args, HPy_ssize_t nargs, DHPy kw);
+DHPy debug_ctx_Type_GenericNew(HPyContext *dctx, DHPy type, const DHPy *args, HPy_ssize_t nargs, DHPy kw);
 DHPy debug_ctx_GetAttr(HPyContext *dctx, DHPy obj, DHPy name);
-DHPy debug_ctx_GetAttr_s(HPyContext *dctx, DHPy obj, const char *name);
+DHPy debug_ctx_GetAttr_s(HPyContext *dctx, DHPy obj, const char *utf8_name);
 int debug_ctx_HasAttr(HPyContext *dctx, DHPy obj, DHPy name);
-int debug_ctx_HasAttr_s(HPyContext *dctx, DHPy obj, const char *name);
+int debug_ctx_HasAttr_s(HPyContext *dctx, DHPy obj, const char *utf8_name);
 int debug_ctx_SetAttr(HPyContext *dctx, DHPy obj, DHPy name, DHPy value);
-int debug_ctx_SetAttr_s(HPyContext *dctx, DHPy obj, const char *name, DHPy value);
+int debug_ctx_SetAttr_s(HPyContext *dctx, DHPy obj, const char *utf8_name, DHPy value);
 DHPy debug_ctx_GetItem(HPyContext *dctx, DHPy obj, DHPy key);
 DHPy debug_ctx_GetItem_i(HPyContext *dctx, DHPy obj, HPy_ssize_t idx);
-DHPy debug_ctx_GetItem_s(HPyContext *dctx, DHPy obj, const char *key);
+DHPy debug_ctx_GetItem_s(HPyContext *dctx, DHPy obj, const char *utf8_key);
 int debug_ctx_Contains(HPyContext *dctx, DHPy container, DHPy key);
 int debug_ctx_SetItem(HPyContext *dctx, DHPy obj, DHPy key, DHPy value);
 int debug_ctx_SetItem_i(HPyContext *dctx, DHPy obj, HPy_ssize_t idx, DHPy value);
-int debug_ctx_SetItem_s(HPyContext *dctx, DHPy obj, const char *key, DHPy value);
+int debug_ctx_SetItem_s(HPyContext *dctx, DHPy obj, const char *utf8_key, DHPy value);
+int debug_ctx_DelItem(HPyContext *dctx, DHPy obj, DHPy key);
+int debug_ctx_DelItem_i(HPyContext *dctx, DHPy obj, HPy_ssize_t idx);
+int debug_ctx_DelItem_s(HPyContext *dctx, DHPy obj, const char *utf8_key);
 DHPy debug_ctx_Type(HPyContext *dctx, DHPy obj);
 int debug_ctx_TypeCheck(HPyContext *dctx, DHPy obj, DHPy type);
+const char *debug_ctx_Type_GetName(HPyContext *dctx, DHPy type);
+int debug_ctx_Type_IsSubtype(HPyContext *dctx, DHPy sub, DHPy type);
 int debug_ctx_Is(HPyContext *dctx, DHPy obj, DHPy other);
-void *debug_ctx_AsStruct(HPyContext *dctx, DHPy h);
-void *debug_ctx_AsStructLegacy(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Object(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Legacy(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Type(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Long(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Float(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Unicode(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_Tuple(HPyContext *dctx, DHPy h);
+void *debug_ctx_AsStruct_List(HPyContext *dctx, DHPy h);
+HPyType_BuiltinShape debug_ctx_Type_GetBuiltinShape(HPyContext *dctx, DHPy h_type);
 DHPy debug_ctx_New(HPyContext *dctx, DHPy h_type, void **data);
 DHPy debug_ctx_Repr(HPyContext *dctx, DHPy obj);
 DHPy debug_ctx_Str(HPyContext *dctx, DHPy obj);
 DHPy debug_ctx_ASCII(HPyContext *dctx, DHPy obj);
 DHPy debug_ctx_Bytes(HPyContext *dctx, DHPy obj);
 DHPy debug_ctx_RichCompare(HPyContext *dctx, DHPy v, DHPy w, int op);
 int debug_ctx_RichCompareBool(HPyContext *dctx, DHPy v, DHPy w, int op);
 HPy_hash_t debug_ctx_Hash(HPyContext *dctx, DHPy obj);
 int debug_ctx_Bytes_Check(HPyContext *dctx, DHPy h);
 HPy_ssize_t debug_ctx_Bytes_Size(HPyContext *dctx, DHPy h);
 HPy_ssize_t debug_ctx_Bytes_GET_SIZE(HPyContext *dctx, DHPy h);
-char *debug_ctx_Bytes_AsString(HPyContext *dctx, DHPy h);
-char *debug_ctx_Bytes_AS_STRING(HPyContext *dctx, DHPy h);
-DHPy debug_ctx_Bytes_FromString(HPyContext *dctx, const char *v);
-DHPy debug_ctx_Bytes_FromStringAndSize(HPyContext *dctx, const char *v, HPy_ssize_t len);
+const char *debug_ctx_Bytes_AsString(HPyContext *dctx, DHPy h);
+const char *debug_ctx_Bytes_AS_STRING(HPyContext *dctx, DHPy h);
+DHPy debug_ctx_Bytes_FromString(HPyContext *dctx, const char *bytes);
+DHPy debug_ctx_Bytes_FromStringAndSize(HPyContext *dctx, const char *bytes, HPy_ssize_t len);
 DHPy debug_ctx_Unicode_FromString(HPyContext *dctx, const char *utf8);
 int debug_ctx_Unicode_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Unicode_AsASCIIString(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Unicode_AsLatin1String(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Unicode_AsUTF8String(HPyContext *dctx, DHPy h);
 const char *debug_ctx_Unicode_AsUTF8AndSize(HPyContext *dctx, DHPy h, HPy_ssize_t *size);
 DHPy debug_ctx_Unicode_FromWideChar(HPyContext *dctx, const wchar_t *w, HPy_ssize_t size);
 DHPy debug_ctx_Unicode_DecodeFSDefault(HPyContext *dctx, const char *v);
 DHPy debug_ctx_Unicode_DecodeFSDefaultAndSize(HPyContext *dctx, const char *v, HPy_ssize_t size);
 DHPy debug_ctx_Unicode_EncodeFSDefault(HPyContext *dctx, DHPy h);
 HPy_UCS4 debug_ctx_Unicode_ReadChar(HPyContext *dctx, DHPy h, HPy_ssize_t index);
-DHPy debug_ctx_Unicode_DecodeASCII(HPyContext *dctx, const char *s, HPy_ssize_t size, const char *errors);
-DHPy debug_ctx_Unicode_DecodeLatin1(HPyContext *dctx, const char *s, HPy_ssize_t size, const char *errors);
+DHPy debug_ctx_Unicode_DecodeASCII(HPyContext *dctx, const char *ascii, HPy_ssize_t size, const char *errors);
+DHPy debug_ctx_Unicode_DecodeLatin1(HPyContext *dctx, const char *latin1, HPy_ssize_t size, const char *errors);
+DHPy debug_ctx_Unicode_FromEncodedObject(HPyContext *dctx, DHPy obj, const char *encoding, const char *errors);
+DHPy debug_ctx_Unicode_Substring(HPyContext *dctx, DHPy str, HPy_ssize_t start, HPy_ssize_t end);
 int debug_ctx_List_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_List_New(HPyContext *dctx, HPy_ssize_t len);
 int debug_ctx_List_Append(HPyContext *dctx, DHPy h_list, DHPy h_item);
 int debug_ctx_Dict_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Dict_New(HPyContext *dctx);
+DHPy debug_ctx_Dict_Keys(HPyContext *dctx, DHPy h);
+DHPy debug_ctx_Dict_Copy(HPyContext *dctx, DHPy h);
 int debug_ctx_Tuple_Check(HPyContext *dctx, DHPy h);
 DHPy debug_ctx_Tuple_FromArray(HPyContext *dctx, DHPy items[], HPy_ssize_t n);
-DHPy debug_ctx_Import_ImportModule(HPyContext *dctx, const char *name);
+int debug_ctx_Slice_Unpack(HPyContext *dctx, DHPy slice, HPy_ssize_t *start, HPy_ssize_t *stop, HPy_ssize_t *step);
+DHPy debug_ctx_Import_ImportModule(HPyContext *dctx, const char *utf8_name);
+DHPy debug_ctx_Capsule_New(HPyContext *dctx, void *pointer, const char *utf8_name, HPyCapsule_Destructor *destructor);
+void *debug_ctx_Capsule_Get(HPyContext *dctx, DHPy capsule, _HPyCapsule_key key, const char *utf8_name);
+int debug_ctx_Capsule_IsValid(HPyContext *dctx, DHPy capsule, const char *utf8_name);
+int debug_ctx_Capsule_Set(HPyContext *dctx, DHPy capsule, _HPyCapsule_key key, void *value);
 DHPy debug_ctx_FromPyObject(HPyContext *dctx, cpy_PyObject *obj);
 cpy_PyObject *debug_ctx_AsPyObject(HPyContext *dctx, DHPy h);
 void debug_ctx_CallRealFunctionFromTrampoline(HPyContext *dctx, HPyFunc_Signature sig, HPyCFunction func, void *args);
-HPyListBuilder debug_ctx_ListBuilder_New(HPyContext *dctx, HPy_ssize_t initial_size);
+HPyListBuilder debug_ctx_ListBuilder_New(HPyContext *dctx, HPy_ssize_t size);
 void debug_ctx_ListBuilder_Set(HPyContext *dctx, HPyListBuilder builder, HPy_ssize_t index, DHPy h_item);
 DHPy debug_ctx_ListBuilder_Build(HPyContext *dctx, HPyListBuilder builder);
 void debug_ctx_ListBuilder_Cancel(HPyContext *dctx, HPyListBuilder builder);
-HPyTupleBuilder debug_ctx_TupleBuilder_New(HPyContext *dctx, HPy_ssize_t initial_size);
+HPyTupleBuilder debug_ctx_TupleBuilder_New(HPyContext *dctx, HPy_ssize_t size);
 void debug_ctx_TupleBuilder_Set(HPyContext *dctx, HPyTupleBuilder builder, HPy_ssize_t index, DHPy h_item);
 DHPy debug_ctx_TupleBuilder_Build(HPyContext *dctx, HPyTupleBuilder builder);
 void debug_ctx_TupleBuilder_Cancel(HPyContext *dctx, HPyTupleBuilder builder);
 HPyTracker debug_ctx_Tracker_New(HPyContext *dctx, HPy_ssize_t size);
 int debug_ctx_Tracker_Add(HPyContext *dctx, HPyTracker ht, DHPy h);
 void debug_ctx_Tracker_ForgetAll(HPyContext *dctx, HPyTracker ht);
 void debug_ctx_Tracker_Close(HPyContext *dctx, HPyTracker ht);
 void debug_ctx_Field_Store(HPyContext *dctx, DHPy target_object, HPyField *target_field, DHPy h);
 DHPy debug_ctx_Field_Load(HPyContext *dctx, DHPy source_object, HPyField source_field);
 void debug_ctx_ReenterPythonExecution(HPyContext *dctx, HPyThreadState state);
 HPyThreadState debug_ctx_LeavePythonExecution(HPyContext *dctx);
 void debug_ctx_Global_Store(HPyContext *dctx, HPyGlobal *global, DHPy h);
 DHPy debug_ctx_Global_Load(HPyContext *dctx, HPyGlobal global);
 void debug_ctx_Dump(HPyContext *dctx, DHPy h);
+DHPy debug_ctx_Compile_s(HPyContext *dctx, const char *utf8_source, const char *utf8_filename, HPy_SourceKind kind);
+DHPy debug_ctx_EvalCode(HPyContext *dctx, DHPy code, DHPy globals, DHPy locals);
+DHPy debug_ctx_ContextVar_New(HPyContext *dctx, const char *name, DHPy default_value);
+int32_t debug_ctx_ContextVar_Get(HPyContext *dctx, DHPy context_var, DHPy default_value, DHPy *result);
+DHPy debug_ctx_ContextVar_Set(HPyContext *dctx, DHPy context_var, DHPy value);
+int debug_ctx_SetCallFunction(HPyContext *dctx, DHPy h, HPyCallFunction *func);
 
 static inline void debug_ctx_init_fields(HPyContext *dctx, HPyContext *uctx)
 {
-    dctx->h_None = DHPy_open(dctx, uctx->h_None);
-    dctx->h_True = DHPy_open(dctx, uctx->h_True);
-    dctx->h_False = DHPy_open(dctx, uctx->h_False);
-    dctx->h_NotImplemented = DHPy_open(dctx, uctx->h_NotImplemented);
-    dctx->h_Ellipsis = DHPy_open(dctx, uctx->h_Ellipsis);
-    dctx->h_BaseException = DHPy_open(dctx, uctx->h_BaseException);
-    dctx->h_Exception = DHPy_open(dctx, uctx->h_Exception);
-    dctx->h_StopAsyncIteration = DHPy_open(dctx, uctx->h_StopAsyncIteration);
-    dctx->h_StopIteration = DHPy_open(dctx, uctx->h_StopIteration);
-    dctx->h_GeneratorExit = DHPy_open(dctx, uctx->h_GeneratorExit);
-    dctx->h_ArithmeticError = DHPy_open(dctx, uctx->h_ArithmeticError);
-    dctx->h_LookupError = DHPy_open(dctx, uctx->h_LookupError);
-    dctx->h_AssertionError = DHPy_open(dctx, uctx->h_AssertionError);
-    dctx->h_AttributeError = DHPy_open(dctx, uctx->h_AttributeError);
-    dctx->h_BufferError = DHPy_open(dctx, uctx->h_BufferError);
-    dctx->h_EOFError = DHPy_open(dctx, uctx->h_EOFError);
-    dctx->h_FloatingPointError = DHPy_open(dctx, uctx->h_FloatingPointError);
-    dctx->h_OSError = DHPy_open(dctx, uctx->h_OSError);
-    dctx->h_ImportError = DHPy_open(dctx, uctx->h_ImportError);
-    dctx->h_ModuleNotFoundError = DHPy_open(dctx, uctx->h_ModuleNotFoundError);
-    dctx->h_IndexError = DHPy_open(dctx, uctx->h_IndexError);
-    dctx->h_KeyError = DHPy_open(dctx, uctx->h_KeyError);
-    dctx->h_KeyboardInterrupt = DHPy_open(dctx, uctx->h_KeyboardInterrupt);
-    dctx->h_MemoryError = DHPy_open(dctx, uctx->h_MemoryError);
-    dctx->h_NameError = DHPy_open(dctx, uctx->h_NameError);
-    dctx->h_OverflowError = DHPy_open(dctx, uctx->h_OverflowError);
-    dctx->h_RuntimeError = DHPy_open(dctx, uctx->h_RuntimeError);
-    dctx->h_RecursionError = DHPy_open(dctx, uctx->h_RecursionError);
-    dctx->h_NotImplementedError = DHPy_open(dctx, uctx->h_NotImplementedError);
-    dctx->h_SyntaxError = DHPy_open(dctx, uctx->h_SyntaxError);
-    dctx->h_IndentationError = DHPy_open(dctx, uctx->h_IndentationError);
-    dctx->h_TabError = DHPy_open(dctx, uctx->h_TabError);
-    dctx->h_ReferenceError = DHPy_open(dctx, uctx->h_ReferenceError);
-    dctx->h_SystemError = DHPy_open(dctx, uctx->h_SystemError);
-    dctx->h_SystemExit = DHPy_open(dctx, uctx->h_SystemExit);
-    dctx->h_TypeError = DHPy_open(dctx, uctx->h_TypeError);
-    dctx->h_UnboundLocalError = DHPy_open(dctx, uctx->h_UnboundLocalError);
-    dctx->h_UnicodeError = DHPy_open(dctx, uctx->h_UnicodeError);
-    dctx->h_UnicodeEncodeError = DHPy_open(dctx, uctx->h_UnicodeEncodeError);
-    dctx->h_UnicodeDecodeError = DHPy_open(dctx, uctx->h_UnicodeDecodeError);
-    dctx->h_UnicodeTranslateError = DHPy_open(dctx, uctx->h_UnicodeTranslateError);
-    dctx->h_ValueError = DHPy_open(dctx, uctx->h_ValueError);
-    dctx->h_ZeroDivisionError = DHPy_open(dctx, uctx->h_ZeroDivisionError);
-    dctx->h_BlockingIOError = DHPy_open(dctx, uctx->h_BlockingIOError);
-    dctx->h_BrokenPipeError = DHPy_open(dctx, uctx->h_BrokenPipeError);
-    dctx->h_ChildProcessError = DHPy_open(dctx, uctx->h_ChildProcessError);
-    dctx->h_ConnectionError = DHPy_open(dctx, uctx->h_ConnectionError);
-    dctx->h_ConnectionAbortedError = DHPy_open(dctx, uctx->h_ConnectionAbortedError);
-    dctx->h_ConnectionRefusedError = DHPy_open(dctx, uctx->h_ConnectionRefusedError);
-    dctx->h_ConnectionResetError = DHPy_open(dctx, uctx->h_ConnectionResetError);
-    dctx->h_FileExistsError = DHPy_open(dctx, uctx->h_FileExistsError);
-    dctx->h_FileNotFoundError = DHPy_open(dctx, uctx->h_FileNotFoundError);
-    dctx->h_InterruptedError = DHPy_open(dctx, uctx->h_InterruptedError);
-    dctx->h_IsADirectoryError = DHPy_open(dctx, uctx->h_IsADirectoryError);
-    dctx->h_NotADirectoryError = DHPy_open(dctx, uctx->h_NotADirectoryError);
-    dctx->h_PermissionError = DHPy_open(dctx, uctx->h_PermissionError);
-    dctx->h_ProcessLookupError = DHPy_open(dctx, uctx->h_ProcessLookupError);
-    dctx->h_TimeoutError = DHPy_open(dctx, uctx->h_TimeoutError);
-    dctx->h_Warning = DHPy_open(dctx, uctx->h_Warning);
-    dctx->h_UserWarning = DHPy_open(dctx, uctx->h_UserWarning);
-    dctx->h_DeprecationWarning = DHPy_open(dctx, uctx->h_DeprecationWarning);
-    dctx->h_PendingDeprecationWarning = DHPy_open(dctx, uctx->h_PendingDeprecationWarning);
-    dctx->h_SyntaxWarning = DHPy_open(dctx, uctx->h_SyntaxWarning);
-    dctx->h_RuntimeWarning = DHPy_open(dctx, uctx->h_RuntimeWarning);
-    dctx->h_FutureWarning = DHPy_open(dctx, uctx->h_FutureWarning);
-    dctx->h_ImportWarning = DHPy_open(dctx, uctx->h_ImportWarning);
-    dctx->h_UnicodeWarning = DHPy_open(dctx, uctx->h_UnicodeWarning);
-    dctx->h_BytesWarning = DHPy_open(dctx, uctx->h_BytesWarning);
-    dctx->h_ResourceWarning = DHPy_open(dctx, uctx->h_ResourceWarning);
-    dctx->h_BaseObjectType = DHPy_open(dctx, uctx->h_BaseObjectType);
-    dctx->h_TypeType = DHPy_open(dctx, uctx->h_TypeType);
-    dctx->h_BoolType = DHPy_open(dctx, uctx->h_BoolType);
-    dctx->h_LongType = DHPy_open(dctx, uctx->h_LongType);
-    dctx->h_FloatType = DHPy_open(dctx, uctx->h_FloatType);
-    dctx->h_UnicodeType = DHPy_open(dctx, uctx->h_UnicodeType);
-    dctx->h_TupleType = DHPy_open(dctx, uctx->h_TupleType);
-    dctx->h_ListType = DHPy_open(dctx, uctx->h_ListType);
-    dctx->ctx_Module_Create = &debug_ctx_Module_Create;
+    dctx->h_None = DHPy_open_immortal(dctx, uctx->h_None);
+    dctx->h_True = DHPy_open_immortal(dctx, uctx->h_True);
+    dctx->h_False = DHPy_open_immortal(dctx, uctx->h_False);
+    dctx->h_NotImplemented = DHPy_open_immortal(dctx, uctx->h_NotImplemented);
+    dctx->h_Ellipsis = DHPy_open_immortal(dctx, uctx->h_Ellipsis);
+    dctx->h_BaseException = DHPy_open_immortal(dctx, uctx->h_BaseException);
+    dctx->h_Exception = DHPy_open_immortal(dctx, uctx->h_Exception);
+    dctx->h_StopAsyncIteration = DHPy_open_immortal(dctx, uctx->h_StopAsyncIteration);
+    dctx->h_StopIteration = DHPy_open_immortal(dctx, uctx->h_StopIteration);
+    dctx->h_GeneratorExit = DHPy_open_immortal(dctx, uctx->h_GeneratorExit);
+    dctx->h_ArithmeticError = DHPy_open_immortal(dctx, uctx->h_ArithmeticError);
+    dctx->h_LookupError = DHPy_open_immortal(dctx, uctx->h_LookupError);
+    dctx->h_AssertionError = DHPy_open_immortal(dctx, uctx->h_AssertionError);
+    dctx->h_AttributeError = DHPy_open_immortal(dctx, uctx->h_AttributeError);
+    dctx->h_BufferError = DHPy_open_immortal(dctx, uctx->h_BufferError);
+    dctx->h_EOFError = DHPy_open_immortal(dctx, uctx->h_EOFError);
+    dctx->h_FloatingPointError = DHPy_open_immortal(dctx, uctx->h_FloatingPointError);
+    dctx->h_OSError = DHPy_open_immortal(dctx, uctx->h_OSError);
+    dctx->h_ImportError = DHPy_open_immortal(dctx, uctx->h_ImportError);
+    dctx->h_ModuleNotFoundError = DHPy_open_immortal(dctx, uctx->h_ModuleNotFoundError);
+    dctx->h_IndexError = DHPy_open_immortal(dctx, uctx->h_IndexError);
+    dctx->h_KeyError = DHPy_open_immortal(dctx, uctx->h_KeyError);
+    dctx->h_KeyboardInterrupt = DHPy_open_immortal(dctx, uctx->h_KeyboardInterrupt);
+    dctx->h_MemoryError = DHPy_open_immortal(dctx, uctx->h_MemoryError);
+    dctx->h_NameError = DHPy_open_immortal(dctx, uctx->h_NameError);
+    dctx->h_OverflowError = DHPy_open_immortal(dctx, uctx->h_OverflowError);
+    dctx->h_RuntimeError = DHPy_open_immortal(dctx, uctx->h_RuntimeError);
+    dctx->h_RecursionError = DHPy_open_immortal(dctx, uctx->h_RecursionError);
+    dctx->h_NotImplementedError = DHPy_open_immortal(dctx, uctx->h_NotImplementedError);
+    dctx->h_SyntaxError = DHPy_open_immortal(dctx, uctx->h_SyntaxError);
+    dctx->h_IndentationError = DHPy_open_immortal(dctx, uctx->h_IndentationError);
+    dctx->h_TabError = DHPy_open_immortal(dctx, uctx->h_TabError);
+    dctx->h_ReferenceError = DHPy_open_immortal(dctx, uctx->h_ReferenceError);
+    dctx->h_SystemError = DHPy_open_immortal(dctx, uctx->h_SystemError);
+    dctx->h_SystemExit = DHPy_open_immortal(dctx, uctx->h_SystemExit);
+    dctx->h_TypeError = DHPy_open_immortal(dctx, uctx->h_TypeError);
+    dctx->h_UnboundLocalError = DHPy_open_immortal(dctx, uctx->h_UnboundLocalError);
+    dctx->h_UnicodeError = DHPy_open_immortal(dctx, uctx->h_UnicodeError);
+    dctx->h_UnicodeEncodeError = DHPy_open_immortal(dctx, uctx->h_UnicodeEncodeError);
+    dctx->h_UnicodeDecodeError = DHPy_open_immortal(dctx, uctx->h_UnicodeDecodeError);
+    dctx->h_UnicodeTranslateError = DHPy_open_immortal(dctx, uctx->h_UnicodeTranslateError);
+    dctx->h_ValueError = DHPy_open_immortal(dctx, uctx->h_ValueError);
+    dctx->h_ZeroDivisionError = DHPy_open_immortal(dctx, uctx->h_ZeroDivisionError);
+    dctx->h_BlockingIOError = DHPy_open_immortal(dctx, uctx->h_BlockingIOError);
+    dctx->h_BrokenPipeError = DHPy_open_immortal(dctx, uctx->h_BrokenPipeError);
+    dctx->h_ChildProcessError = DHPy_open_immortal(dctx, uctx->h_ChildProcessError);
+    dctx->h_ConnectionError = DHPy_open_immortal(dctx, uctx->h_ConnectionError);
+    dctx->h_ConnectionAbortedError = DHPy_open_immortal(dctx, uctx->h_ConnectionAbortedError);
+    dctx->h_ConnectionRefusedError = DHPy_open_immortal(dctx, uctx->h_ConnectionRefusedError);
+    dctx->h_ConnectionResetError = DHPy_open_immortal(dctx, uctx->h_ConnectionResetError);
+    dctx->h_FileExistsError = DHPy_open_immortal(dctx, uctx->h_FileExistsError);
+    dctx->h_FileNotFoundError = DHPy_open_immortal(dctx, uctx->h_FileNotFoundError);
+    dctx->h_InterruptedError = DHPy_open_immortal(dctx, uctx->h_InterruptedError);
+    dctx->h_IsADirectoryError = DHPy_open_immortal(dctx, uctx->h_IsADirectoryError);
+    dctx->h_NotADirectoryError = DHPy_open_immortal(dctx, uctx->h_NotADirectoryError);
+    dctx->h_PermissionError = DHPy_open_immortal(dctx, uctx->h_PermissionError);
+    dctx->h_ProcessLookupError = DHPy_open_immortal(dctx, uctx->h_ProcessLookupError);
+    dctx->h_TimeoutError = DHPy_open_immortal(dctx, uctx->h_TimeoutError);
+    dctx->h_Warning = DHPy_open_immortal(dctx, uctx->h_Warning);
+    dctx->h_UserWarning = DHPy_open_immortal(dctx, uctx->h_UserWarning);
+    dctx->h_DeprecationWarning = DHPy_open_immortal(dctx, uctx->h_DeprecationWarning);
+    dctx->h_PendingDeprecationWarning = DHPy_open_immortal(dctx, uctx->h_PendingDeprecationWarning);
+    dctx->h_SyntaxWarning = DHPy_open_immortal(dctx, uctx->h_SyntaxWarning);
+    dctx->h_RuntimeWarning = DHPy_open_immortal(dctx, uctx->h_RuntimeWarning);
+    dctx->h_FutureWarning = DHPy_open_immortal(dctx, uctx->h_FutureWarning);
+    dctx->h_ImportWarning = DHPy_open_immortal(dctx, uctx->h_ImportWarning);
+    dctx->h_UnicodeWarning = DHPy_open_immortal(dctx, uctx->h_UnicodeWarning);
+    dctx->h_BytesWarning = DHPy_open_immortal(dctx, uctx->h_BytesWarning);
+    dctx->h_ResourceWarning = DHPy_open_immortal(dctx, uctx->h_ResourceWarning);
+    dctx->h_BaseObjectType = DHPy_open_immortal(dctx, uctx->h_BaseObjectType);
+    dctx->h_TypeType = DHPy_open_immortal(dctx, uctx->h_TypeType);
+    dctx->h_BoolType = DHPy_open_immortal(dctx, uctx->h_BoolType);
+    dctx->h_LongType = DHPy_open_immortal(dctx, uctx->h_LongType);
+    dctx->h_FloatType = DHPy_open_immortal(dctx, uctx->h_FloatType);
+    dctx->h_UnicodeType = DHPy_open_immortal(dctx, uctx->h_UnicodeType);
+    dctx->h_TupleType = DHPy_open_immortal(dctx, uctx->h_TupleType);
+    dctx->h_ListType = DHPy_open_immortal(dctx, uctx->h_ListType);
+    dctx->h_ComplexType = DHPy_open_immortal(dctx, uctx->h_ComplexType);
+    dctx->h_BytesType = DHPy_open_immortal(dctx, uctx->h_BytesType);
+    dctx->h_MemoryViewType = DHPy_open_immortal(dctx, uctx->h_MemoryViewType);
+    dctx->h_CapsuleType = DHPy_open_immortal(dctx, uctx->h_CapsuleType);
+    dctx->h_SliceType = DHPy_open_immortal(dctx, uctx->h_SliceType);
+    dctx->h_Builtins = DHPy_open_immortal(dctx, uctx->h_Builtins);
     dctx->ctx_Dup = &debug_ctx_Dup;
     dctx->ctx_Close = &debug_ctx_Close;
-    dctx->ctx_Long_FromLong = &debug_ctx_Long_FromLong;
-    dctx->ctx_Long_FromUnsignedLong = &debug_ctx_Long_FromUnsignedLong;
-    dctx->ctx_Long_FromLongLong = &debug_ctx_Long_FromLongLong;
-    dctx->ctx_Long_FromUnsignedLongLong = &debug_ctx_Long_FromUnsignedLongLong;
+    dctx->ctx_Long_FromInt32_t = &debug_ctx_Long_FromInt32_t;
+    dctx->ctx_Long_FromUInt32_t = &debug_ctx_Long_FromUInt32_t;
+    dctx->ctx_Long_FromInt64_t = &debug_ctx_Long_FromInt64_t;
+    dctx->ctx_Long_FromUInt64_t = &debug_ctx_Long_FromUInt64_t;
     dctx->ctx_Long_FromSize_t = &debug_ctx_Long_FromSize_t;
     dctx->ctx_Long_FromSsize_t = &debug_ctx_Long_FromSsize_t;
-    dctx->ctx_Long_AsLong = &debug_ctx_Long_AsLong;
-    dctx->ctx_Long_AsUnsignedLong = &debug_ctx_Long_AsUnsignedLong;
-    dctx->ctx_Long_AsUnsignedLongMask = &debug_ctx_Long_AsUnsignedLongMask;
-    dctx->ctx_Long_AsLongLong = &debug_ctx_Long_AsLongLong;
-    dctx->ctx_Long_AsUnsignedLongLong = &debug_ctx_Long_AsUnsignedLongLong;
-    dctx->ctx_Long_AsUnsignedLongLongMask = &debug_ctx_Long_AsUnsignedLongLongMask;
+    dctx->ctx_Long_AsInt32_t = &debug_ctx_Long_AsInt32_t;
+    dctx->ctx_Long_AsUInt32_t = &debug_ctx_Long_AsUInt32_t;
+    dctx->ctx_Long_AsUInt32_tMask = &debug_ctx_Long_AsUInt32_tMask;
+    dctx->ctx_Long_AsInt64_t = &debug_ctx_Long_AsInt64_t;
+    dctx->ctx_Long_AsUInt64_t = &debug_ctx_Long_AsUInt64_t;
+    dctx->ctx_Long_AsUInt64_tMask = &debug_ctx_Long_AsUInt64_tMask;
     dctx->ctx_Long_AsSize_t = &debug_ctx_Long_AsSize_t;
     dctx->ctx_Long_AsSsize_t = &debug_ctx_Long_AsSsize_t;
     dctx->ctx_Long_AsVoidPtr = &debug_ctx_Long_AsVoidPtr;
     dctx->ctx_Long_AsDouble = &debug_ctx_Long_AsDouble;
     dctx->ctx_Float_FromDouble = &debug_ctx_Float_FromDouble;
     dctx->ctx_Float_AsDouble = &debug_ctx_Float_AsDouble;
-    dctx->ctx_Bool_FromLong = &debug_ctx_Bool_FromLong;
+    dctx->ctx_Bool_FromBool = &debug_ctx_Bool_FromBool;
     dctx->ctx_Length = &debug_ctx_Length;
     dctx->ctx_Number_Check = &debug_ctx_Number_Check;
     dctx->ctx_Add = &debug_ctx_Add;
     dctx->ctx_Subtract = &debug_ctx_Subtract;
     dctx->ctx_Multiply = &debug_ctx_Multiply;
     dctx->ctx_MatrixMultiply = &debug_ctx_MatrixMultiply;
     dctx->ctx_FloorDivide = &debug_ctx_FloorDivide;
@@ -298,14 +331,16 @@
     dctx->ctx_InPlaceLshift = &debug_ctx_InPlaceLshift;
     dctx->ctx_InPlaceRshift = &debug_ctx_InPlaceRshift;
     dctx->ctx_InPlaceAnd = &debug_ctx_InPlaceAnd;
     dctx->ctx_InPlaceXor = &debug_ctx_InPlaceXor;
     dctx->ctx_InPlaceOr = &debug_ctx_InPlaceOr;
     dctx->ctx_Callable_Check = &debug_ctx_Callable_Check;
     dctx->ctx_CallTupleDict = &debug_ctx_CallTupleDict;
+    dctx->ctx_Call = &debug_ctx_Call;
+    dctx->ctx_CallMethod = &debug_ctx_CallMethod;
     dctx->ctx_FatalError = &debug_ctx_FatalError;
     dctx->ctx_Err_SetString = &debug_ctx_Err_SetString;
     dctx->ctx_Err_SetObject = &debug_ctx_Err_SetObject;
     dctx->ctx_Err_SetFromErrnoWithFilename = &debug_ctx_Err_SetFromErrnoWithFilename;
     dctx->ctx_Err_SetFromErrnoWithFilenameObjects = &debug_ctx_Err_SetFromErrnoWithFilenameObjects;
     dctx->ctx_Err_Occurred = &debug_ctx_Err_Occurred;
     dctx->ctx_Err_ExceptionMatches = &debug_ctx_Err_ExceptionMatches;
@@ -327,19 +362,31 @@
     dctx->ctx_GetItem = &debug_ctx_GetItem;
     dctx->ctx_GetItem_i = &debug_ctx_GetItem_i;
     dctx->ctx_GetItem_s = &debug_ctx_GetItem_s;
     dctx->ctx_Contains = &debug_ctx_Contains;
     dctx->ctx_SetItem = &debug_ctx_SetItem;
     dctx->ctx_SetItem_i = &debug_ctx_SetItem_i;
     dctx->ctx_SetItem_s = &debug_ctx_SetItem_s;
+    dctx->ctx_DelItem = &debug_ctx_DelItem;
+    dctx->ctx_DelItem_i = &debug_ctx_DelItem_i;
+    dctx->ctx_DelItem_s = &debug_ctx_DelItem_s;
     dctx->ctx_Type = &debug_ctx_Type;
     dctx->ctx_TypeCheck = &debug_ctx_TypeCheck;
+    dctx->ctx_Type_GetName = &debug_ctx_Type_GetName;
+    dctx->ctx_Type_IsSubtype = &debug_ctx_Type_IsSubtype;
     dctx->ctx_Is = &debug_ctx_Is;
-    dctx->ctx_AsStruct = &debug_ctx_AsStruct;
-    dctx->ctx_AsStructLegacy = &debug_ctx_AsStructLegacy;
+    dctx->ctx_AsStruct_Object = &debug_ctx_AsStruct_Object;
+    dctx->ctx_AsStruct_Legacy = &debug_ctx_AsStruct_Legacy;
+    dctx->ctx_AsStruct_Type = &debug_ctx_AsStruct_Type;
+    dctx->ctx_AsStruct_Long = &debug_ctx_AsStruct_Long;
+    dctx->ctx_AsStruct_Float = &debug_ctx_AsStruct_Float;
+    dctx->ctx_AsStruct_Unicode = &debug_ctx_AsStruct_Unicode;
+    dctx->ctx_AsStruct_Tuple = &debug_ctx_AsStruct_Tuple;
+    dctx->ctx_AsStruct_List = &debug_ctx_AsStruct_List;
+    dctx->ctx_Type_GetBuiltinShape = &debug_ctx_Type_GetBuiltinShape;
     dctx->ctx_New = &debug_ctx_New;
     dctx->ctx_Repr = &debug_ctx_Repr;
     dctx->ctx_Str = &debug_ctx_Str;
     dctx->ctx_ASCII = &debug_ctx_ASCII;
     dctx->ctx_Bytes = &debug_ctx_Bytes;
     dctx->ctx_RichCompare = &debug_ctx_RichCompare;
     dctx->ctx_RichCompareBool = &debug_ctx_RichCompareBool;
@@ -360,22 +407,31 @@
     dctx->ctx_Unicode_FromWideChar = &debug_ctx_Unicode_FromWideChar;
     dctx->ctx_Unicode_DecodeFSDefault = &debug_ctx_Unicode_DecodeFSDefault;
     dctx->ctx_Unicode_DecodeFSDefaultAndSize = &debug_ctx_Unicode_DecodeFSDefaultAndSize;
     dctx->ctx_Unicode_EncodeFSDefault = &debug_ctx_Unicode_EncodeFSDefault;
     dctx->ctx_Unicode_ReadChar = &debug_ctx_Unicode_ReadChar;
     dctx->ctx_Unicode_DecodeASCII = &debug_ctx_Unicode_DecodeASCII;
     dctx->ctx_Unicode_DecodeLatin1 = &debug_ctx_Unicode_DecodeLatin1;
+    dctx->ctx_Unicode_FromEncodedObject = &debug_ctx_Unicode_FromEncodedObject;
+    dctx->ctx_Unicode_Substring = &debug_ctx_Unicode_Substring;
     dctx->ctx_List_Check = &debug_ctx_List_Check;
     dctx->ctx_List_New = &debug_ctx_List_New;
     dctx->ctx_List_Append = &debug_ctx_List_Append;
     dctx->ctx_Dict_Check = &debug_ctx_Dict_Check;
     dctx->ctx_Dict_New = &debug_ctx_Dict_New;
+    dctx->ctx_Dict_Keys = &debug_ctx_Dict_Keys;
+    dctx->ctx_Dict_Copy = &debug_ctx_Dict_Copy;
     dctx->ctx_Tuple_Check = &debug_ctx_Tuple_Check;
     dctx->ctx_Tuple_FromArray = &debug_ctx_Tuple_FromArray;
+    dctx->ctx_Slice_Unpack = &debug_ctx_Slice_Unpack;
     dctx->ctx_Import_ImportModule = &debug_ctx_Import_ImportModule;
+    dctx->ctx_Capsule_New = &debug_ctx_Capsule_New;
+    dctx->ctx_Capsule_Get = &debug_ctx_Capsule_Get;
+    dctx->ctx_Capsule_IsValid = &debug_ctx_Capsule_IsValid;
+    dctx->ctx_Capsule_Set = &debug_ctx_Capsule_Set;
     dctx->ctx_FromPyObject = &debug_ctx_FromPyObject;
     dctx->ctx_AsPyObject = &debug_ctx_AsPyObject;
     dctx->ctx_CallRealFunctionFromTrampoline = &debug_ctx_CallRealFunctionFromTrampoline;
     dctx->ctx_ListBuilder_New = &debug_ctx_ListBuilder_New;
     dctx->ctx_ListBuilder_Set = &debug_ctx_ListBuilder_Set;
     dctx->ctx_ListBuilder_Build = &debug_ctx_ListBuilder_Build;
     dctx->ctx_ListBuilder_Cancel = &debug_ctx_ListBuilder_Cancel;
@@ -390,8 +446,14 @@
     dctx->ctx_Field_Store = &debug_ctx_Field_Store;
     dctx->ctx_Field_Load = &debug_ctx_Field_Load;
     dctx->ctx_ReenterPythonExecution = &debug_ctx_ReenterPythonExecution;
     dctx->ctx_LeavePythonExecution = &debug_ctx_LeavePythonExecution;
     dctx->ctx_Global_Store = &debug_ctx_Global_Store;
     dctx->ctx_Global_Load = &debug_ctx_Global_Load;
     dctx->ctx_Dump = &debug_ctx_Dump;
+    dctx->ctx_Compile_s = &debug_ctx_Compile_s;
+    dctx->ctx_EvalCode = &debug_ctx_EvalCode;
+    dctx->ctx_ContextVar_New = &debug_ctx_ContextVar_New;
+    dctx->ctx_ContextVar_Get = &debug_ctx_ContextVar_Get;
+    dctx->ctx_ContextVar_Set = &debug_ctx_ContextVar_Set;
+    dctx->ctx_SetCallFunction = &debug_ctx_SetCallFunction;
 }
```

### Comparing `hpy-0.0.4/hpy/debug/src/debug_ctx_not_cpython.c` & `hpy-0.9.0rc1/hpy/debug/src/debug_ctx_not_cpython.c`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/debug/src/debug_internal.h` & `hpy-0.9.0rc1/hpy/debug/src/debug_internal.h`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,42 @@
 #ifndef HPY_DEBUG_INTERNAL_H
 #define HPY_DEBUG_INTERNAL_H
 
 #include <assert.h>
 #include "hpy.h"
 #include "hpy_debug.h"
 
-#define HPY_DEBUG_MAGIC 0xDEB00FF
+#define HPY_DEBUG_INFO_MAGIC     0xDEB00FF
+#define HPY_DEBUG_CTX_INFO_MAGIC 0xDDA003F
+
+/* === DHQueue === */
+
+/**
+ * This struct is meant to be embedded in the actual payload struct to avoid
+ * a separate allocation of the queue node.
+ */
+typedef struct _DHQueueNode_s {
+    struct _DHQueueNode_s *next;
+    struct _DHQueueNode_s *prev;
+    HPy_ssize_t size;
+} DHQueueNode;
+
+typedef struct {
+    DHQueueNode *head;
+    DHQueueNode *tail;
+    HPy_ssize_t size;
+} DHQueue;
+
+void DHQueue_init(DHQueue *q);
+void DHQueue_append(DHQueue *q, DHQueueNode *h);
+DHQueueNode *DHQueue_popfront(DHQueue *q);
+void DHQueue_remove(DHQueue *q, DHQueueNode *h);
+void DHQueue_sanity_check(DHQueue *q);
+
+/* === DHQueue === */
 
 /* The Debug context is a wrapper around an underlying context, which we will
    call Universal. Inside the debug mode we manipulate handles which belongs
    to both contexts, so to make things easier we create two typedefs to make
    it clear what kind of handle we expect: UHPy and DHPy:
 
      * UHPy are opaque from our point of view.
@@ -100,14 +127,33 @@
    different configuration of the limits. For the sake of keeping the
    implementation reasonably simple and portable, we choose to ignore this
    for the time being.
 */
 
 typedef HPy UHPy;
 typedef HPy DHPy;
+typedef HPyTupleBuilder UHPyTupleBuilder;
+typedef HPyTupleBuilder DHPyTupleBuilder;
+typedef HPyListBuilder UHPyListBuilder;
+typedef HPyListBuilder DHPyListBuilder;
+
+#define DHPyTupleBuilder_IsNull(h) ((h)._tup == 0)
+#define DHPyListBuilder_IsNull(h) ((h)._lst == 0)
+
+#if defined(_MSC_VER) && defined(__cplusplus) // MSVC C4576
+#  define UHPyListBuilder_NULL {0}
+#  define UHPyTupleBuilder_NULL {0}
+#  define DHPyListBuilder_NULL UHPyListBuilder_NULL
+#  define DHPyTupleBuilder_NULL UHPyTupleBuilder_NULL
+#else
+#  define UHPyListBuilder_NULL ((UHPyListBuilder){0})
+#  define UHPyTupleBuilder_NULL ((UHPyTupleBuilder){0})
+#  define DHPyListBuilder_NULL ((DHPyListBuilder){0})
+#  define DHPyTupleBuilder_NULL ((DHPyTupleBuilder){0})
+#endif
 
 /* Under CPython:
      - UHPy always end with 1 (see hpy.universal's _py2h and _h2py)
      - DHPy are pointers, so they always end with 0
 
    DHPy_sanity_check is a minimal check to ensure that we are not treating a
    UHPy as a DHPy. Note that DHPy_sanity_check works fine also on HPy_NULL.
@@ -131,102 +177,182 @@
 
 // NOTE: having a "generation" field is the easiest way to know when a handle
 // was created, but we waste 8 bytes per handle. Since all handles of the same
 // generation are stored sequentially in the open_handles list, a possible
 // alternative implementation is to put special placeholders inside the list
 // to mark the creation of a new generation
 typedef struct DebugHandle {
+    DHQueueNode node;
     UHPy uh;
     long generation;
-    bool is_closed;
+    bool is_closed:1;
+    bool is_immortal:1;
     // pointer to and size of any raw data associated with
     // the lifetime of the handle:
     void *associated_data;
     // allocation_stacktrace information if available
     char *allocation_stacktrace;
     HPy_ssize_t associated_data_size;
-    struct DebugHandle *prev;
-    struct DebugHandle *next;
 } DebugHandle;
 
+/** A debug handle for a tuple or list builder. */
+typedef struct DebugBuilderHandle {
+    DHQueueNode node;
+    union {
+        UHPyTupleBuilder tuple_builder;
+        UHPyListBuilder list_builder;
+    } uh;
+
+    /**
+     * ``true`` if the builder was consumed by the build function or cancelled.
+     */
+    bool is_closed:1;
+} DebugBuilderHandle;
+
 static inline DebugHandle * as_DebugHandle(DHPy dh) {
     DHPy_sanity_check(dh);
     return (DebugHandle *)dh._i;
 }
 
 static inline DHPy as_DHPy(DebugHandle *handle) {
     return (DHPy){(HPy_ssize_t)handle};
 }
 
+static inline DebugBuilderHandle * DHPyTupleBuilder_as_DebugBuilderHandle(DHPyTupleBuilder dh) {
+    if (DHPyTupleBuilder_IsNull(dh))
+        return NULL;
+    return (DebugBuilderHandle *)dh._tup;
+}
+
+static inline DHPyTupleBuilder as_DHPyTupleBuilder(DebugBuilderHandle *handle) {
+    return (DHPyTupleBuilder){(HPy_ssize_t)handle};
+}
+
+static inline DebugBuilderHandle * DHPyListBuilder_as_DebugBuilderHandle(DHPyListBuilder dh) {
+    if (DHPyListBuilder_IsNull(dh))
+        return NULL;
+    return (DebugBuilderHandle *)dh._lst;
+}
+
+static inline DHPyListBuilder as_DHPyListBuilder(DebugBuilderHandle *handle) {
+    return (DHPyListBuilder){(HPy_ssize_t)handle};
+}
+
 DHPy DHPy_open(HPyContext *dctx, UHPy uh);
+DHPy DHPy_open_immortal(HPyContext *dctx, UHPy uh);
 void DHPy_close(HPyContext *dctx, DHPy dh);
 void DHPy_close_and_check(HPyContext *dctx, DHPy dh);
 void DHPy_free(HPyContext *dctx, DHPy dh);
 void DHPy_invalid_handle(HPyContext *dctx, DHPy dh);
+DHPyTupleBuilder DHPyTupleBuilder_open(HPyContext *dctx, UHPyTupleBuilder uh);
+DHPyListBuilder DHPyListBuilder_open(HPyContext *dctx, UHPyListBuilder uh);
+void DHPy_invalid_builder_handle(HPyContext *dctx);
+void DHPy_builder_handle_close(HPyContext *dctx, DebugBuilderHandle *handle);
 
 static inline UHPy DHPy_unwrap(HPyContext *dctx, DHPy dh)
 {
     if (HPy_IsNull(dh))
         return HPy_NULL;
     DebugHandle *handle = as_DebugHandle(dh);
     if (handle->is_closed)
         DHPy_invalid_handle(dctx, dh);
     return handle->uh;
 }
 
-/* === DHQueue === */
-
-typedef struct {
-    DebugHandle *head;
-    DebugHandle *tail;
-    HPy_ssize_t size;
-} DHQueue;
+#define BUILDER_UNWRAP(TYPE, ACCESS) \
+    static inline U##TYPE D##TYPE##_unwrap(HPyContext *dctx, D##TYPE dh) \
+    { \
+        DebugBuilderHandle *handle = D##TYPE##_as_DebugBuilderHandle(dh); \
+        if (handle == NULL) \
+            return U##TYPE##_NULL; \
+        if (handle->is_closed) { \
+            DHPy_invalid_builder_handle(dctx); \
+            return U##TYPE##_NULL; \
+        } \
+        return handle->uh.ACCESS; \
+    }
 
-void DHQueue_init(DHQueue *q);
-void DHQueue_append(DHQueue *q, DebugHandle *h);
-DebugHandle *DHQueue_popfront(DHQueue *q);
-void DHQueue_remove(DHQueue *q, DebugHandle *h);
-void DHQueue_sanity_check(DHQueue *q);
+BUILDER_UNWRAP(HPyTupleBuilder, tuple_builder)
+BUILDER_UNWRAP(HPyListBuilder, list_builder)
 
 /* === HPyDebugInfo === */
 
 static const HPy_ssize_t DEFAULT_CLOSED_HANDLES_QUEUE_MAX_SIZE = 1024;
 static const HPy_ssize_t DEFAULT_PROTECTED_RAW_DATA_MAX_SIZE = 1024 * 1024 * 10;
+static const HPy_ssize_t HPY_DEBUG_DEFAULT_STACKTRACE_LIMIT = 16;
+#define HPY_DEBUG_CTX_CACHE_SIZE 16 // Keep in sync with test_context_reuse.py
+
+// We intentionally create multiple HPyContext instances to check that
+// the extension is not relying on the HPyContext identity. Before bouncing
+// to HPy function in the CallRealFunctionFromTrampoline, we take next debug
+// context copy from a circular buffer and mark the current one as invalid.
+//
+// HPyDebugInfo: represents meta-data shared between all the copies of the
+// debug context.
+//
+// HPyDebugCtxInfo represents meta-data specific to each debug context
+// instance. At this point it is main flag is_valid that is checked by all
+// the context functions as the first thing.
 
 typedef struct {
     long magic_number; // used just for sanity checks
     HPyContext *uctx;
     long current_generation;
 
+    // Array of cached debug contexts used as a circular buffer
+    HPyContext *dctx_cache[HPY_DEBUG_CTX_CACHE_SIZE];
+    size_t dctx_cache_current_index;
+
     // the following should be an HPyField, but it's complicate:
     // HPyFields should be used only on memory which is known by the GC, which
     // happens automatically if you use e.g. HPy_New, but currently
     // HPy_DebugInfo is malloced(). We need either:
     //   1. a generic HPy_GcMalloc() OR
     //   2. HPy_{Un}TrackMemory(), so that we can add manually allocated
     //      memory as a GC root
+    // Alternative is to put it into a module state or to put it into HPyGlobal
+    // once those features are implemented
     UHPy uh_on_invalid_handle;
+    UHPy uh_on_invalid_builder_handle;
     HPy_ssize_t closed_handles_queue_max_size; // configurable by the user
     HPy_ssize_t protected_raw_data_max_size;
     HPy_ssize_t protected_raw_data_size;
     // Limit for the stack traces captured for allocated handles
     // Value 0 implies that stack traces should not be captured
     HPy_ssize_t handle_alloc_stacktrace_limit;
     DHQueue open_handles;
     DHQueue closed_handles;
+    DHQueue closed_builder;
 } HPyDebugInfo;
 
+typedef struct {
+    long magic_number; // used just for sanity checks
+    bool is_valid;
+    HPyDebugInfo *info;
+} HPyDebugCtxInfo;
+
+static inline HPyDebugCtxInfo *get_ctx_info(HPyContext *dctx)
+{
+    HPyDebugCtxInfo *info = (HPyDebugCtxInfo*)dctx->_private;
+    assert(info->magic_number == HPY_DEBUG_CTX_INFO_MAGIC); // sanity check
+    return info;
+}
+
 static inline HPyDebugInfo *get_info(HPyContext *dctx)
 {
-    HPyDebugInfo *info = (HPyDebugInfo*)dctx->_private;
-    assert(info->magic_number == HPY_DEBUG_MAGIC); // sanity check
+    HPyDebugInfo *info = get_ctx_info(dctx)->info;
+    assert(info->magic_number == HPY_DEBUG_INFO_MAGIC); // sanity check
     return info;
 }
 
 
+HPyContext* hpy_debug_get_next_dctx_from_cache(HPyContext *dctx);
+
+void report_invalid_debug_context();
+
 void *raw_data_copy(const void* data, HPy_ssize_t size, bool write_protect);
 void raw_data_protect(void* data, HPy_ssize_t size);
 /* Return value: 0 indicates success, any different value indicates an error */
 int raw_data_free(void *data, HPy_ssize_t size);
 
 void create_stacktrace(char **target, HPy_ssize_t max_frames_count);
```

### Comparing `hpy-0.0.4/hpy/debug/src/dhqueue.c` & `hpy-0.9.0rc1/hpy/debug/src/dhqueue.c`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 // context in multiple threads
 void DHQueue_init(DHQueue *q) {
     q->head = NULL;
     q->tail = NULL;
     q->size = 0;
 }
 
-void DHQueue_append(DHQueue *q, DebugHandle *h) {
+void DHQueue_append(DHQueue *q, DHQueueNode *h) {
     if (q->head == NULL) {
         h->prev = NULL;
         h->next = NULL;
         q->head = h;
         q->tail = h;
     } else {
         h->next = NULL;
         h->prev = q->tail;
         q->tail->next = h;
         q->tail = h;
     }
     q->size++;
 }
 
-DebugHandle *DHQueue_popfront(DHQueue *q)
+DHQueueNode *DHQueue_popfront(DHQueue *q)
 {
     assert(q->size > 0);
     assert(q->head != NULL);
-    DebugHandle *head = q->head;
+    DHQueueNode *head = q->head;
     if (q->size == 1) {
         q->head = NULL;
         q->tail = NULL;
         q->size = 0;
     }
     else {
         q->head = head->next;
@@ -41,19 +41,19 @@
     // the following is not strictly necessary, but it makes thing much easier
     // to debug in case of bugs
     head->next = NULL;
     head->prev = NULL;
     return head;
 }
 
-void DHQueue_remove(DHQueue *q, DebugHandle *h)
+void DHQueue_remove(DHQueue *q, DHQueueNode *h)
 {
 #ifndef NDEBUG
     // if we are debugging, let's check that h is effectively in the queue
-    DebugHandle *it = q->head;
+    DHQueueNode *it = q->head;
     bool found = false;
     while(it != NULL) {
         if (it == h) {
             found = true;
             break;
         }
         it = it->next;
@@ -79,15 +79,15 @@
     q->size--;
     h->next = NULL;
     h->prev = NULL;
 }
 
 
 #ifndef NDEBUG
-static void linked_item_sanity_check(DebugHandle *h)
+static void linked_item_sanity_check(DHQueueNode *h)
 {
     if (h == NULL)
         return;
     if (h->next != NULL)
         assert(h->next->prev == h);
     if (h->prev != NULL)
         assert(h->prev->next == h);
@@ -102,15 +102,15 @@
         assert(q->tail == NULL);
         assert(q->size == 0);
     }
     else {
         assert(q->head->prev == NULL);
         assert(q->tail->next == NULL);
         assert(q->size > 0);
-        DebugHandle *h = q->head;
+        DHQueueNode *h = q->head;
         HPy_ssize_t size = 0;
         while(h != NULL) {
             linked_item_sanity_check(h);
             if (h->next == NULL)
                 assert(h == q->tail);
             h = h->next;
             size++;
```

### Comparing `hpy-0.0.4/hpy/debug/src/include/hpy_debug.h` & `hpy-0.9.0rc1/hpy/debug/src/include/hpy_debug.h`

 * *Files 18% similar despite different names*

```diff
@@ -38,22 +38,20 @@
 
 // this is the HPy init function created by HPy_MODINIT. In CPython's version
 // of hpy.universal the code is embedded inside the extension, so we can call
 // this function directly instead of dlopen it. This is similar to what
 // CPython does for its own built-in modules. But we must use the same
 // signature as HPy_MODINIT
 
-// Copied from Python's exports.h, pyport.h
-#ifndef Py_EXPORTED_SYMBOL
-    #if defined(_WIN32) || defined(__CYGWIN__)
-        #define Py_EXPORTED_SYMBOL __declspec(dllexport)
-    #else
-        #define Py_EXPORTED_SYMBOL __attribute__ ((visibility ("default")))
-    #endif
+#ifdef ___cplusplus
+extern "C"
 #endif
+HPy_EXPORTED_SYMBOL
+HPyModuleDef* HPyInit__debug();
+
 #ifdef ___cplusplus
 extern "C"
 #endif
-Py_EXPORTED_SYMBOL
-HPy HPyInit__debug(HPyContext *uctx);
+HPy_EXPORTED_SYMBOL
+void HPyInitGlobalContext__debug(HPyContext *ctx);
 
 #endif /* HPY_DEBUG_H */
```

### Comparing `hpy-0.0.4/hpy/debug/src/memprotect.c` & `hpy-0.9.0rc1/hpy/debug/src/memprotect.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #include "debug_internal.h"
 
 // Implements OS dependent abstraction of memory protection
 
 #ifdef _HPY_DEBUG_MEM_PROTECT_USEMMAP
 
+#ifndef _WIN32
+
 // On UNIX systems we use mmap and mprotect
-// On Windows this should be eventually extended to use
-// VirtualAlloc and VirtualProtect
 
 #include <sys/mman.h>
 #include <string.h>
 
 void *raw_data_copy(const void* data, HPy_ssize_t size, bool write_protect) {
-    void* new_ptr = mmap(NULL, size, PROT_READ | PROT_WRITE, MAP_PRIVATE | MAP_ANONYMOUS, -1, 0);
+    void* new_ptr;
+    new_ptr = mmap(NULL, size, PROT_READ | PROT_WRITE, MAP_PRIVATE | MAP_ANONYMOUS, -1, 0);
+    if (new_ptr == NULL)
+        return NULL;
     memcpy(new_ptr, data, size);
     if (write_protect) {
         mprotect(new_ptr, size, PROT_READ);
     }
     return new_ptr;
 }
 
@@ -26,14 +29,45 @@
 
 int raw_data_free(void *data, HPy_ssize_t size) {
     return munmap(data, size);
 }
 
 #else
 
+// On Windows systems we use VirtualAlloc and VirtualProtect
+
+#include <windows.h>
+#include <memoryapi.h>
+
+void *raw_data_copy(const void* data, HPy_ssize_t size, bool write_protect) {
+    void* new_ptr;
+    DWORD old;
+    new_ptr = VirtualAlloc(NULL, size, MEM_COMMIT | MEM_RESERVE, PAGE_READWRITE);
+    if (new_ptr == NULL)
+        return NULL;
+    memcpy(new_ptr, data, size);
+    if (write_protect) {
+        VirtualProtect(new_ptr, size, PAGE_READONLY, &old);
+    }
+    return new_ptr;
+}
+
+void raw_data_protect(void* data, HPy_ssize_t size) {
+    DWORD old;
+    VirtualProtect(data, size, PAGE_NOACCESS, &old);
+}
+
+int raw_data_free(void *data, HPy_ssize_t size) {
+    return !VirtualFree(data, 0, MEM_RELEASE);
+}
+
+#endif /* _WIN32 */
+
+#else
+
 // Generic fallback that should work for any OS with decent C compiler: copy
 // the memory and then override it with garbage to "protect" it from reading.
 
 #include <stdlib.h>
 #include <string.h>
 
 void *raw_data_copy(const void* data, HPy_ssize_t size, bool write_protect) {
@@ -53,8 +87,8 @@
 }
 
 int raw_data_free(void *data, HPy_ssize_t size) {
     free(data);
     return 0;
 }
 
-#endif
+#endif
```

### Comparing `hpy-0.0.4/hpy/debug/src/stacktrace.c` & `hpy-0.9.0rc1/hpy/debug/src/stacktrace.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #include "debug_internal.h"
 
-#if (__linux__ && __GNU_LIBRARY__)
+#if ((__linux__ && __GNU_LIBRARY__) || __APPLE__)
 
 // Basic implementation that uses backtrace from glibc
 
 #include <stdlib.h>
 #include <string.h>
 #include <execinfo.h>
 
@@ -81,13 +81,14 @@
 #else
 
 #include <string.h>
 
 void create_stacktrace(char **target, HPy_ssize_t max_frames_count) {
     const char msg[] =
             "Current HPy build does not support getting C stack traces.\n"
-            "At the moment this is only supported on Linux with glibc.";
+            "At the moment this is only supported on Linux with glibc"
+            " and macOS.";
     *target = malloc(sizeof(msg));
     memcpy(*target, msg, sizeof(msg));
 }
 
 #endif
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/autogen_hpyfunc_declare.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyfunc_declare.h`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
    Run this to regenerate:
        make autogen
 
 */
 
 #define _HPyFunc_DECLARE_HPyFunc_NOARGS(SYM) static HPy SYM(HPyContext *ctx, HPy self)
 #define _HPyFunc_DECLARE_HPyFunc_O(SYM) static HPy SYM(HPyContext *ctx, HPy self, HPy arg)
-#define _HPyFunc_DECLARE_HPyFunc_VARARGS(SYM) static HPy SYM(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
-#define _HPyFunc_DECLARE_HPyFunc_KEYWORDS(SYM) static HPy SYM(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs, HPy kw)
+#define _HPyFunc_DECLARE_HPyFunc_VARARGS(SYM) static HPy SYM(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
+#define _HPyFunc_DECLARE_HPyFunc_KEYWORDS(SYM) static HPy SYM(HPyContext *ctx, HPy self, const HPy *args, size_t nargs, HPy kwnames)
 #define _HPyFunc_DECLARE_HPyFunc_UNARYFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_BINARYFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_TERNARYFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_INQUIRY(SYM) static int SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_LENFUNC(SYM) static HPy_ssize_t SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_SSIZEARGFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy_ssize_t)
 #define _HPyFunc_DECLARE_HPyFunc_SSIZESSIZEARGFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy_ssize_t, HPy_ssize_t)
@@ -32,28 +32,30 @@
 #define _HPyFunc_DECLARE_HPyFunc_REPRFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_HASHFUNC(SYM) static HPy_hash_t SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_RICHCMPFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy, HPy_RichCmpOp)
 #define _HPyFunc_DECLARE_HPyFunc_GETITERFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_ITERNEXTFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_DESCRGETFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy, HPy, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_DESCRSETFUNC(SYM) static int SYM(HPyContext *ctx, HPy, HPy, HPy)
-#define _HPyFunc_DECLARE_HPyFunc_INITPROC(SYM) static int SYM(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs, HPy kw)
+#define _HPyFunc_DECLARE_HPyFunc_INITPROC(SYM) static int SYM(HPyContext *ctx, HPy self, const HPy *args, HPy_ssize_t nargs, HPy kw)
+#define _HPyFunc_DECLARE_HPyFunc_NEWFUNC(SYM) static HPy SYM(HPyContext *ctx, HPy type, const HPy *args, HPy_ssize_t nargs, HPy kw)
 #define _HPyFunc_DECLARE_HPyFunc_GETTER(SYM) static HPy SYM(HPyContext *ctx, HPy, void *)
 #define _HPyFunc_DECLARE_HPyFunc_SETTER(SYM) static int SYM(HPyContext *ctx, HPy, HPy, void *)
 #define _HPyFunc_DECLARE_HPyFunc_OBJOBJPROC(SYM) static int SYM(HPyContext *ctx, HPy, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_GETBUFFERPROC(SYM) static int SYM(HPyContext *ctx, HPy, HPy_buffer *, int)
 #define _HPyFunc_DECLARE_HPyFunc_RELEASEBUFFERPROC(SYM) static void SYM(HPyContext *ctx, HPy, HPy_buffer *)
 #define _HPyFunc_DECLARE_HPyFunc_TRAVERSEPROC(SYM) static int SYM(void *object, HPyFunc_visitproc visit, void *arg)
 #define _HPyFunc_DECLARE_HPyFunc_DESTRUCTOR(SYM) static void SYM(HPyContext *ctx, HPy)
 #define _HPyFunc_DECLARE_HPyFunc_DESTROYFUNC(SYM) static void SYM(void *)
+#define _HPyFunc_DECLARE_HPyFunc_MOD_CREATE(SYM) static HPy SYM(HPyContext *ctx, HPy)
 
 typedef HPy (*HPyFunc_noargs)(HPyContext *ctx, HPy self);
 typedef HPy (*HPyFunc_o)(HPyContext *ctx, HPy self, HPy arg);
-typedef HPy (*HPyFunc_varargs)(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs);
-typedef HPy (*HPyFunc_keywords)(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs, HPy kw);
+typedef HPy (*HPyFunc_varargs)(HPyContext *ctx, HPy self, const HPy *args, size_t nargs);
+typedef HPy (*HPyFunc_keywords)(HPyContext *ctx, HPy self, const HPy *args, size_t nargs, HPy kwnames);
 typedef HPy (*HPyFunc_unaryfunc)(HPyContext *ctx, HPy);
 typedef HPy (*HPyFunc_binaryfunc)(HPyContext *ctx, HPy, HPy);
 typedef HPy (*HPyFunc_ternaryfunc)(HPyContext *ctx, HPy, HPy, HPy);
 typedef int (*HPyFunc_inquiry)(HPyContext *ctx, HPy);
 typedef HPy_ssize_t (*HPyFunc_lenfunc)(HPyContext *ctx, HPy);
 typedef HPy (*HPyFunc_ssizeargfunc)(HPyContext *ctx, HPy, HPy_ssize_t);
 typedef HPy (*HPyFunc_ssizessizeargfunc)(HPyContext *ctx, HPy, HPy_ssize_t, HPy_ssize_t);
@@ -68,16 +70,18 @@
 typedef HPy (*HPyFunc_reprfunc)(HPyContext *ctx, HPy);
 typedef HPy_hash_t (*HPyFunc_hashfunc)(HPyContext *ctx, HPy);
 typedef HPy (*HPyFunc_richcmpfunc)(HPyContext *ctx, HPy, HPy, HPy_RichCmpOp);
 typedef HPy (*HPyFunc_getiterfunc)(HPyContext *ctx, HPy);
 typedef HPy (*HPyFunc_iternextfunc)(HPyContext *ctx, HPy);
 typedef HPy (*HPyFunc_descrgetfunc)(HPyContext *ctx, HPy, HPy, HPy);
 typedef int (*HPyFunc_descrsetfunc)(HPyContext *ctx, HPy, HPy, HPy);
-typedef int (*HPyFunc_initproc)(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs, HPy kw);
+typedef int (*HPyFunc_initproc)(HPyContext *ctx, HPy self, const HPy *args, HPy_ssize_t nargs, HPy kw);
+typedef HPy (*HPyFunc_newfunc)(HPyContext *ctx, HPy type, const HPy *args, HPy_ssize_t nargs, HPy kw);
 typedef HPy (*HPyFunc_getter)(HPyContext *ctx, HPy, void *);
 typedef int (*HPyFunc_setter)(HPyContext *ctx, HPy, HPy, void *);
 typedef int (*HPyFunc_objobjproc)(HPyContext *ctx, HPy, HPy);
 typedef int (*HPyFunc_getbufferproc)(HPyContext *ctx, HPy, HPy_buffer *, int);
 typedef void (*HPyFunc_releasebufferproc)(HPyContext *ctx, HPy, HPy_buffer *);
 typedef int (*HPyFunc_traverseproc)(void *object, HPyFunc_visitproc visit, void *arg);
 typedef void (*HPyFunc_destructor)(HPyContext *ctx, HPy);
 typedef void (*HPyFunc_destroyfunc)(void *);
+typedef HPy (*HPyFunc_mod_create)(HPyContext *ctx, HPy);
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/autogen_hpyslot.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/autogen_hpyslot.h`

 * *Files 9% similar despite different names*

```diff
@@ -53,23 +53,28 @@
     HPy_sq_concat = 40,
     HPy_sq_contains = 41,
     HPy_sq_inplace_concat = 42,
     HPy_sq_inplace_repeat = 43,
     HPy_sq_item = 44,
     HPy_sq_length = 45,
     HPy_sq_repeat = 46,
+    HPy_tp_call = 50,
+    HPy_tp_hash = 59,
     HPy_tp_init = 60,
     HPy_tp_new = 65,
     HPy_tp_repr = 66,
     HPy_tp_richcompare = 67,
+    HPy_tp_str = 70,
     HPy_tp_traverse = 71,
     HPy_nb_matrix_multiply = 75,
     HPy_nb_inplace_matrix_multiply = 76,
     HPy_tp_finalize = 80,
     HPy_tp_destroy = 1000,
+    HPy_mod_create = 2000,
+    HPy_mod_exec = 2001,
 } HPySlot_Slot;
 
 #define _HPySlot_SIG__HPy_bf_getbuffer HPyFunc_GETBUFFERPROC
 #define _HPySlot_SIG__HPy_bf_releasebuffer HPyFunc_RELEASEBUFFERPROC
 #define _HPySlot_SIG__HPy_mp_ass_subscript HPyFunc_OBJOBJARGPROC
 #define _HPySlot_SIG__HPy_mp_length HPyFunc_LENFUNC
 #define _HPySlot_SIG__HPy_mp_subscript HPyFunc_BINARYFUNC
@@ -110,16 +115,21 @@
 #define _HPySlot_SIG__HPy_sq_concat HPyFunc_BINARYFUNC
 #define _HPySlot_SIG__HPy_sq_contains HPyFunc_OBJOBJPROC
 #define _HPySlot_SIG__HPy_sq_inplace_concat HPyFunc_BINARYFUNC
 #define _HPySlot_SIG__HPy_sq_inplace_repeat HPyFunc_SSIZEARGFUNC
 #define _HPySlot_SIG__HPy_sq_item HPyFunc_SSIZEARGFUNC
 #define _HPySlot_SIG__HPy_sq_length HPyFunc_LENFUNC
 #define _HPySlot_SIG__HPy_sq_repeat HPyFunc_SSIZEARGFUNC
+#define _HPySlot_SIG__HPy_tp_call HPyFunc_KEYWORDS
+#define _HPySlot_SIG__HPy_tp_hash HPyFunc_HASHFUNC
 #define _HPySlot_SIG__HPy_tp_init HPyFunc_INITPROC
-#define _HPySlot_SIG__HPy_tp_new HPyFunc_KEYWORDS
+#define _HPySlot_SIG__HPy_tp_new HPyFunc_NEWFUNC
 #define _HPySlot_SIG__HPy_tp_repr HPyFunc_REPRFUNC
 #define _HPySlot_SIG__HPy_tp_richcompare HPyFunc_RICHCMPFUNC
+#define _HPySlot_SIG__HPy_tp_str HPyFunc_REPRFUNC
 #define _HPySlot_SIG__HPy_tp_traverse HPyFunc_TRAVERSEPROC
 #define _HPySlot_SIG__HPy_nb_matrix_multiply HPyFunc_BINARYFUNC
 #define _HPySlot_SIG__HPy_nb_inplace_matrix_multiply HPyFunc_BINARYFUNC
 #define _HPySlot_SIG__HPy_tp_finalize HPyFunc_DESTRUCTOR
 #define _HPySlot_SIG__HPy_tp_destroy HPyFunc_DESTROYFUNC
+#define _HPySlot_SIG__HPy_mod_create HPyFunc_MOD_CREATE
+#define _HPySlot_SIG__HPy_mod_exec HPyFunc_INQUIRY
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/cpython/autogen_api_impl.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_api_impl.h`

 * *Files 18% similar despite different names*

```diff
@@ -6,74 +6,24 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
-HPyAPI_FUNC HPy HPyLong_FromLong(HPyContext *ctx, long value)
-{
-    return _py2h(PyLong_FromLong(value));
-}
-
-HPyAPI_FUNC HPy HPyLong_FromUnsignedLong(HPyContext *ctx, unsigned long value)
-{
-    return _py2h(PyLong_FromUnsignedLong(value));
-}
-
-HPyAPI_FUNC HPy HPyLong_FromLongLong(HPyContext *ctx, long long v)
-{
-    return _py2h(PyLong_FromLongLong(v));
-}
-
-HPyAPI_FUNC HPy HPyLong_FromUnsignedLongLong(HPyContext *ctx, unsigned long long v)
-{
-    return _py2h(PyLong_FromUnsignedLongLong(v));
-}
-
 HPyAPI_FUNC HPy HPyLong_FromSize_t(HPyContext *ctx, size_t value)
 {
     return _py2h(PyLong_FromSize_t(value));
 }
 
 HPyAPI_FUNC HPy HPyLong_FromSsize_t(HPyContext *ctx, HPy_ssize_t value)
 {
     return _py2h(PyLong_FromSsize_t(value));
 }
 
-HPyAPI_FUNC long HPyLong_AsLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsLong(_h2py(h));
-}
-
-HPyAPI_FUNC unsigned long HPyLong_AsUnsignedLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLong(_h2py(h));
-}
-
-HPyAPI_FUNC unsigned long HPyLong_AsUnsignedLongMask(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongMask(_h2py(h));
-}
-
-HPyAPI_FUNC long long HPyLong_AsLongLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsLongLong(_h2py(h));
-}
-
-HPyAPI_FUNC unsigned long long HPyLong_AsUnsignedLongLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongLong(_h2py(h));
-}
-
-HPyAPI_FUNC unsigned long long HPyLong_AsUnsignedLongLongMask(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongLongMask(_h2py(h));
-}
-
 HPyAPI_FUNC size_t HPyLong_AsSize_t(HPyContext *ctx, HPy h)
 {
     return PyLong_AsSize_t(_h2py(h));
 }
 
 HPyAPI_FUNC HPy_ssize_t HPyLong_AsSsize_t(HPyContext *ctx, HPy h)
 {
@@ -96,15 +46,15 @@
 }
 
 HPyAPI_FUNC double HPyFloat_AsDouble(HPyContext *ctx, HPy h)
 {
     return PyFloat_AsDouble(_h2py(h));
 }
 
-HPyAPI_FUNC HPy HPyBool_FromLong(HPyContext *ctx, long v)
+HPyAPI_FUNC HPy HPyBool_FromBool(HPyContext *ctx, bool v)
 {
     return _py2h(PyBool_FromLong(v));
 }
 
 HPyAPI_FUNC HPy_ssize_t HPy_Length(HPyContext *ctx, HPy h)
 {
     return PyObject_Length(_h2py(h));
@@ -286,17 +236,17 @@
 }
 
 HPyAPI_FUNC int HPyCallable_Check(HPyContext *ctx, HPy h)
 {
     return PyCallable_Check(_h2py(h));
 }
 
-HPyAPI_FUNC HPy HPyErr_SetString(HPyContext *ctx, HPy h_type, const char *message)
+HPyAPI_FUNC HPy HPyErr_SetString(HPyContext *ctx, HPy h_type, const char *utf8_message)
 {
-    PyErr_SetString(_h2py(h_type), message);
+    PyErr_SetString(_h2py(h_type), utf8_message);
     return HPy_NULL;
 }
 
 HPyAPI_FUNC HPy HPyErr_SetObject(HPyContext *ctx, HPy h_type, HPy h_value)
 {
     PyErr_SetObject(_h2py(h_type), _h2py(h_value));
     return HPy_NULL;
@@ -325,27 +275,27 @@
 }
 
 HPyAPI_FUNC void HPyErr_Clear(HPyContext *ctx)
 {
     PyErr_Clear();
 }
 
-HPyAPI_FUNC HPy HPyErr_NewException(HPyContext *ctx, const char *name, HPy base, HPy dict)
+HPyAPI_FUNC HPy HPyErr_NewException(HPyContext *ctx, const char *utf8_name, HPy base, HPy dict)
 {
-    return _py2h(PyErr_NewException(name, _h2py(base), _h2py(dict)));
+    return _py2h(PyErr_NewException(utf8_name, _h2py(base), _h2py(dict)));
 }
 
-HPyAPI_FUNC HPy HPyErr_NewExceptionWithDoc(HPyContext *ctx, const char *name, const char *doc, HPy base, HPy dict)
+HPyAPI_FUNC HPy HPyErr_NewExceptionWithDoc(HPyContext *ctx, const char *utf8_name, const char *utf8_doc, HPy base, HPy dict)
 {
-    return _py2h(PyErr_NewExceptionWithDoc(name, doc, _h2py(base), _h2py(dict)));
+    return _py2h(PyErr_NewExceptionWithDoc(utf8_name, utf8_doc, _h2py(base), _h2py(dict)));
 }
 
-HPyAPI_FUNC int HPyErr_WarnEx(HPyContext *ctx, HPy category, const char *message, HPy_ssize_t stack_level)
+HPyAPI_FUNC int HPyErr_WarnEx(HPyContext *ctx, HPy category, const char *utf8_message, HPy_ssize_t stack_level)
 {
-    return PyErr_WarnEx(_h2py(category), message, stack_level);
+    return PyErr_WarnEx(_h2py(category), utf8_message, stack_level);
 }
 
 HPyAPI_FUNC void HPyErr_WriteUnraisable(HPyContext *ctx, HPy obj)
 {
     PyErr_WriteUnraisable(_h2py(obj));
 }
 
@@ -355,37 +305,37 @@
 }
 
 HPyAPI_FUNC HPy HPy_GetAttr(HPyContext *ctx, HPy obj, HPy name)
 {
     return _py2h(PyObject_GetAttr(_h2py(obj), _h2py(name)));
 }
 
-HPyAPI_FUNC HPy HPy_GetAttr_s(HPyContext *ctx, HPy obj, const char *name)
+HPyAPI_FUNC HPy HPy_GetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name)
 {
-    return _py2h(PyObject_GetAttrString(_h2py(obj), name));
+    return _py2h(PyObject_GetAttrString(_h2py(obj), utf8_name));
 }
 
 HPyAPI_FUNC int HPy_HasAttr(HPyContext *ctx, HPy obj, HPy name)
 {
     return PyObject_HasAttr(_h2py(obj), _h2py(name));
 }
 
-HPyAPI_FUNC int HPy_HasAttr_s(HPyContext *ctx, HPy obj, const char *name)
+HPyAPI_FUNC int HPy_HasAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name)
 {
-    return PyObject_HasAttrString(_h2py(obj), name);
+    return PyObject_HasAttrString(_h2py(obj), utf8_name);
 }
 
 HPyAPI_FUNC int HPy_SetAttr(HPyContext *ctx, HPy obj, HPy name, HPy value)
 {
     return PyObject_SetAttr(_h2py(obj), _h2py(name), _h2py(value));
 }
 
-HPyAPI_FUNC int HPy_SetAttr_s(HPyContext *ctx, HPy obj, const char *name, HPy value)
+HPyAPI_FUNC int HPy_SetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name, HPy value)
 {
-    return PyObject_SetAttrString(_h2py(obj), name, _h2py(value));
+    return PyObject_SetAttrString(_h2py(obj), utf8_name, _h2py(value));
 }
 
 HPyAPI_FUNC HPy HPy_GetItem(HPyContext *ctx, HPy obj, HPy key)
 {
     return _py2h(PyObject_GetItem(_h2py(obj), _h2py(key)));
 }
 
@@ -395,14 +345,19 @@
 }
 
 HPyAPI_FUNC int HPy_SetItem(HPyContext *ctx, HPy obj, HPy key, HPy value)
 {
     return PyObject_SetItem(_h2py(obj), _h2py(key), _h2py(value));
 }
 
+HPyAPI_FUNC int HPy_DelItem(HPyContext *ctx, HPy obj, HPy key)
+{
+    return PyObject_DelItem(_h2py(obj), _h2py(key));
+}
+
 HPyAPI_FUNC HPy HPy_Type(HPyContext *ctx, HPy obj)
 {
     return _py2h(PyObject_Type(_h2py(obj)));
 }
 
 HPyAPI_FUNC HPy HPy_Repr(HPyContext *ctx, HPy obj)
 {
@@ -450,27 +405,27 @@
 }
 
 HPyAPI_FUNC HPy_ssize_t HPyBytes_GET_SIZE(HPyContext *ctx, HPy h)
 {
     return PyBytes_GET_SIZE(_h2py(h));
 }
 
-HPyAPI_FUNC char *HPyBytes_AsString(HPyContext *ctx, HPy h)
+HPyAPI_FUNC const char *HPyBytes_AsString(HPyContext *ctx, HPy h)
 {
     return PyBytes_AsString(_h2py(h));
 }
 
-HPyAPI_FUNC char *HPyBytes_AS_STRING(HPyContext *ctx, HPy h)
+HPyAPI_FUNC const char *HPyBytes_AS_STRING(HPyContext *ctx, HPy h)
 {
     return PyBytes_AS_STRING(_h2py(h));
 }
 
-HPyAPI_FUNC HPy HPyBytes_FromString(HPyContext *ctx, const char *v)
+HPyAPI_FUNC HPy HPyBytes_FromString(HPyContext *ctx, const char *bytes)
 {
-    return _py2h(PyBytes_FromString(v));
+    return _py2h(PyBytes_FromString(bytes));
 }
 
 HPyAPI_FUNC HPy HPyUnicode_FromString(HPyContext *ctx, const char *utf8)
 {
     return _py2h(PyUnicode_FromString(utf8));
 }
 
@@ -520,22 +475,32 @@
 }
 
 HPyAPI_FUNC HPy_UCS4 HPyUnicode_ReadChar(HPyContext *ctx, HPy h, HPy_ssize_t index)
 {
     return PyUnicode_ReadChar(_h2py(h), index);
 }
 
-HPyAPI_FUNC HPy HPyUnicode_DecodeASCII(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors)
+HPyAPI_FUNC HPy HPyUnicode_DecodeASCII(HPyContext *ctx, const char *ascii, HPy_ssize_t size, const char *errors)
+{
+    return _py2h(PyUnicode_DecodeASCII(ascii, size, errors));
+}
+
+HPyAPI_FUNC HPy HPyUnicode_DecodeLatin1(HPyContext *ctx, const char *latin1, HPy_ssize_t size, const char *errors)
 {
-    return _py2h(PyUnicode_DecodeASCII(s, size, errors));
+    return _py2h(PyUnicode_DecodeLatin1(latin1, size, errors));
 }
 
-HPyAPI_FUNC HPy HPyUnicode_DecodeLatin1(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors)
+HPyAPI_FUNC HPy HPyUnicode_FromEncodedObject(HPyContext *ctx, HPy obj, const char *encoding, const char *errors)
 {
-    return _py2h(PyUnicode_DecodeLatin1(s, size, errors));
+    return _py2h(PyUnicode_FromEncodedObject(_h2py(obj), encoding, errors));
+}
+
+HPyAPI_FUNC HPy HPyUnicode_Substring(HPyContext *ctx, HPy str, HPy_ssize_t start, HPy_ssize_t end)
+{
+    return _py2h(PyUnicode_Substring(_h2py(str), start, end));
 }
 
 HPyAPI_FUNC int HPyList_Check(HPyContext *ctx, HPy h)
 {
     return PyList_Check(_h2py(h));
 }
 
@@ -555,27 +520,62 @@
 }
 
 HPyAPI_FUNC HPy HPyDict_New(HPyContext *ctx)
 {
     return _py2h(PyDict_New());
 }
 
+HPyAPI_FUNC HPy HPyDict_Keys(HPyContext *ctx, HPy h)
+{
+    return _py2h(PyDict_Keys(_h2py(h)));
+}
+
+HPyAPI_FUNC HPy HPyDict_Copy(HPyContext *ctx, HPy h)
+{
+    return _py2h(PyDict_Copy(_h2py(h)));
+}
+
 HPyAPI_FUNC int HPyTuple_Check(HPyContext *ctx, HPy h)
 {
     return PyTuple_Check(_h2py(h));
 }
 
-HPyAPI_FUNC HPy HPyImport_ImportModule(HPyContext *ctx, const char *name)
+HPyAPI_FUNC int HPySlice_Unpack(HPyContext *ctx, HPy slice, HPy_ssize_t *start, HPy_ssize_t *stop, HPy_ssize_t *step)
 {
-    return _py2h(PyImport_ImportModule(name));
+    return PySlice_Unpack(_h2py(slice), start, stop, step);
+}
+
+HPyAPI_FUNC HPy HPyImport_ImportModule(HPyContext *ctx, const char *utf8_name)
+{
+    return _py2h(PyImport_ImportModule(utf8_name));
+}
+
+HPyAPI_FUNC int HPyCapsule_IsValid(HPyContext *ctx, HPy capsule, const char *utf8_name)
+{
+    return PyCapsule_IsValid(_h2py(capsule), utf8_name);
 }
 
 HPyAPI_FUNC void HPy_ReenterPythonExecution(HPyContext *ctx, HPyThreadState state)
 {
     PyEval_RestoreThread(_h2threads(state));
 }
 
 HPyAPI_FUNC HPyThreadState HPy_LeavePythonExecution(HPyContext *ctx)
 {
     return _threads2h(PyEval_SaveThread());
 }
 
+HPyAPI_FUNC HPy HPy_EvalCode(HPyContext *ctx, HPy code, HPy globals, HPy locals)
+{
+    return _py2h(PyEval_EvalCode(_h2py(code), _h2py(globals), _h2py(locals)));
+}
+
+HPyAPI_FUNC HPy HPyContextVar_New(HPyContext *ctx, const char *name, HPy default_value)
+{
+    return _py2h(PyContextVar_New(name, _h2py(default_value)));
+}
+
+HPyAPI_FUNC HPy HPyContextVar_Set(HPyContext *ctx, HPy context_var, HPy value)
+{
+    return _py2h(PyContextVar_Set(_h2py(context_var), _h2py(value)));
+}
+
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,28 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
+typedef HPy (*_HPyCFunction_NOARGS)(HPyContext *, HPy);
+#define _HPyFunc_TRAMPOLINE_HPyFunc_NOARGS(SYM, IMPL) \
+    static cpy_PyObject *SYM(cpy_PyObject *self) \
+    { \
+        _HPyCFunction_NOARGS func = (_HPyCFunction_NOARGS)IMPL; \
+        return _h2py(func(_HPyGetContext(), _py2h(self))); \
+    }
+typedef HPy (*_HPyCFunction_O)(HPyContext *, HPy, HPy);
+#define _HPyFunc_TRAMPOLINE_HPyFunc_O(SYM, IMPL) \
+    static cpy_PyObject *SYM(cpy_PyObject *self, cpy_PyObject *arg) \
+    { \
+        _HPyCFunction_O func = (_HPyCFunction_O)IMPL; \
+        return _h2py(func(_HPyGetContext(), _py2h(self), _py2h(arg))); \
+    }
 typedef HPy (*_HPyCFunction_UNARYFUNC)(HPyContext *, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_UNARYFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0) \
     { \
         _HPyCFunction_UNARYFUNC func = (_HPyCFunction_UNARYFUNC)IMPL; \
         return _h2py(func(_HPyGetContext(), _py2h(arg0))); \
     }
@@ -46,72 +60,72 @@
         return (func(_HPyGetContext(), _py2h(arg0))); \
     }
 typedef HPy (*_HPyCFunction_SSIZEARGFUNC)(HPyContext *, HPy, HPy_ssize_t);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SSIZEARGFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0, HPy_ssize_t arg1) \
     { \
         _HPyCFunction_SSIZEARGFUNC func = (_HPyCFunction_SSIZEARGFUNC)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(arg0), arg1)); \
+        return _h2py(func(_HPyGetContext(), _py2h(arg0), (arg1))); \
     }
 typedef HPy (*_HPyCFunction_SSIZESSIZEARGFUNC)(HPyContext *, HPy, HPy_ssize_t, HPy_ssize_t);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SSIZESSIZEARGFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0, HPy_ssize_t arg1, HPy_ssize_t arg2) \
     { \
         _HPyCFunction_SSIZESSIZEARGFUNC func = (_HPyCFunction_SSIZESSIZEARGFUNC)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(arg0), arg1, arg2)); \
+        return _h2py(func(_HPyGetContext(), _py2h(arg0), (arg1), (arg2))); \
     }
 typedef int (*_HPyCFunction_SSIZEOBJARGPROC)(HPyContext *, HPy, HPy_ssize_t, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SSIZEOBJARGPROC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, HPy_ssize_t arg1, cpy_PyObject *arg2) \
     { \
         _HPyCFunction_SSIZEOBJARGPROC func = (_HPyCFunction_SSIZEOBJARGPROC)IMPL; \
-        return (func(_HPyGetContext(), _py2h(arg0), arg1, _py2h(arg2))); \
+        return (func(_HPyGetContext(), _py2h(arg0), (arg1), _py2h(arg2))); \
     }
 typedef int (*_HPyCFunction_SSIZESSIZEOBJARGPROC)(HPyContext *, HPy, HPy_ssize_t, HPy_ssize_t, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SSIZESSIZEOBJARGPROC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, HPy_ssize_t arg1, HPy_ssize_t arg2, cpy_PyObject *arg3) \
     { \
         _HPyCFunction_SSIZESSIZEOBJARGPROC func = (_HPyCFunction_SSIZESSIZEOBJARGPROC)IMPL; \
-        return (func(_HPyGetContext(), _py2h(arg0), arg1, arg2, _py2h(arg3))); \
+        return (func(_HPyGetContext(), _py2h(arg0), (arg1), (arg2), _py2h(arg3))); \
     }
 typedef int (*_HPyCFunction_OBJOBJARGPROC)(HPyContext *, HPy, HPy, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_OBJOBJARGPROC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, cpy_PyObject *arg1, cpy_PyObject *arg2) \
     { \
         _HPyCFunction_OBJOBJARGPROC func = (_HPyCFunction_OBJOBJARGPROC)IMPL; \
         return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1), _py2h(arg2))); \
     }
 typedef void (*_HPyCFunction_FREEFUNC)(HPyContext *, void *);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_FREEFUNC(SYM, IMPL) \
     static void SYM(void *arg0) \
     { \
         _HPyCFunction_FREEFUNC func = (_HPyCFunction_FREEFUNC)IMPL; \
-        func(_HPyGetContext(), arg0); \
+        func(_HPyGetContext(), (arg0)); \
         return; \
     }
 typedef HPy (*_HPyCFunction_GETATTRFUNC)(HPyContext *, HPy, char *);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_GETATTRFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0, char *arg1) \
     { \
         _HPyCFunction_GETATTRFUNC func = (_HPyCFunction_GETATTRFUNC)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(arg0), arg1)); \
+        return _h2py(func(_HPyGetContext(), _py2h(arg0), (arg1))); \
     }
 typedef HPy (*_HPyCFunction_GETATTROFUNC)(HPyContext *, HPy, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_GETATTROFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0, cpy_PyObject *arg1) \
     { \
         _HPyCFunction_GETATTROFUNC func = (_HPyCFunction_GETATTROFUNC)IMPL; \
         return _h2py(func(_HPyGetContext(), _py2h(arg0), _py2h(arg1))); \
     }
 typedef int (*_HPyCFunction_SETATTRFUNC)(HPyContext *, HPy, char *, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SETATTRFUNC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, char *arg1, cpy_PyObject *arg2) \
     { \
         _HPyCFunction_SETATTRFUNC func = (_HPyCFunction_SETATTRFUNC)IMPL; \
-        return (func(_HPyGetContext(), _py2h(arg0), arg1, _py2h(arg2))); \
+        return (func(_HPyGetContext(), _py2h(arg0), (arg1), _py2h(arg2))); \
     }
 typedef int (*_HPyCFunction_SETATTROFUNC)(HPyContext *, HPy, HPy, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SETATTROFUNC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, cpy_PyObject *arg1, cpy_PyObject *arg2) \
     { \
         _HPyCFunction_SETATTROFUNC func = (_HPyCFunction_SETATTROFUNC)IMPL; \
         return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1), _py2h(arg2))); \
@@ -159,22 +173,22 @@
         return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1), _py2h(arg2))); \
     }
 typedef HPy (*_HPyCFunction_GETTER)(HPyContext *, HPy, void *);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_GETTER(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0, void *arg1) \
     { \
         _HPyCFunction_GETTER func = (_HPyCFunction_GETTER)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(arg0), arg1)); \
+        return _h2py(func(_HPyGetContext(), _py2h(arg0), (arg1))); \
     }
 typedef int (*_HPyCFunction_SETTER)(HPyContext *, HPy, HPy, void *);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_SETTER(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, cpy_PyObject *arg1, void *arg2) \
     { \
         _HPyCFunction_SETTER func = (_HPyCFunction_SETTER)IMPL; \
-        return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1), arg2)); \
+        return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1), (arg2))); \
     }
 typedef int (*_HPyCFunction_OBJOBJPROC)(HPyContext *, HPy, HPy);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_OBJOBJPROC(SYM, IMPL) \
     static int SYM(cpy_PyObject *arg0, cpy_PyObject *arg1) \
     { \
         _HPyCFunction_OBJOBJPROC func = (_HPyCFunction_OBJOBJPROC)IMPL; \
         return (func(_HPyGetContext(), _py2h(arg0), _py2h(arg1))); \
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,59 @@
 #ifndef HPY_CPYTHON_HPYFUNC_TRAMPOLINES_H
 #define HPY_CPYTHON_HPYFUNC_TRAMPOLINES_H
 
-
-typedef HPy (*_HPyCFunction_NOARGS)(HPyContext*, HPy);
-#define _HPyFunc_TRAMPOLINE_HPyFunc_NOARGS(SYM, IMPL)                   \
-    static PyObject *                                                   \
-    SYM(PyObject *self, PyObject *noargs)                               \
-    {                                                                   \
-        _HPyCFunction_NOARGS func = (_HPyCFunction_NOARGS)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(self)));              \
-    }
-
-typedef HPy (*_HPyCFunction_O)(HPyContext*, HPy, HPy);
-#define _HPyFunc_TRAMPOLINE_HPyFunc_O(SYM, IMPL)                        \
-    static PyObject *                                                   \
-    SYM(PyObject *self, PyObject *arg)                                  \
-    {                                                                   \
-        _HPyCFunction_O func = (_HPyCFunction_O)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(self), _py2h(arg)));  \
-    }
-
-typedef HPy (*_HPyCFunction_VARARGS)(HPyContext*, HPy, HPy *, HPy_ssize_t);
+typedef HPy (*_HPyCFunction_VARARGS)(HPyContext*, HPy, const HPy *, size_t);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_VARARGS(SYM, IMPL)                  \
     static PyObject*                                                    \
-    SYM(PyObject *self, PyObject *args)                                 \
+    SYM(PyObject *self, PyObject *const *args, Py_ssize_t nargs)        \
     {                                                                   \
-        /* get the tuple elements as an array of "PyObject *", which */ \
-        /* is equivalent to an array of "HPy" with enough casting... */ \
-        HPy *items = (HPy *)&PyTuple_GET_ITEM(args, 0);                 \
-        Py_ssize_t nargs = PyTuple_GET_SIZE(args);                      \
-        _HPyCFunction_VARARGS func = (_HPyCFunction_VARARGS)IMPL; \
+        _HPyCFunction_VARARGS func = (_HPyCFunction_VARARGS)IMPL;       \
         return _h2py(func(_HPyGetContext(),                             \
-                                 _py2h(self), items, nargs));           \
+                              _py2h(self), _arr_py2h(args), nargs));    \
     }
 
-typedef HPy (*_HPyCFunction_KEYWORDS)(HPyContext*, HPy, HPy *, HPy_ssize_t, HPy);
-#define _HPyFunc_TRAMPOLINE_HPyFunc_KEYWORDS(SYM, IMPL)                 \
-    static PyObject *                                                   \
+typedef HPy (*_HPyCFunction_KEYWORDS)(HPyContext*, HPy, const HPy *, size_t, HPy);
+#define _HPyFunc_TRAMPOLINE_HPyFunc_KEYWORDS(SYM, IMPL)                   \
+    static PyObject *                                                     \
+    SYM(PyObject *self, PyObject *const *args, size_t nargsf,             \
+            PyObject *kwnames)                                            \
+    {                                                                     \
+        _HPyCFunction_KEYWORDS func = (_HPyCFunction_KEYWORDS)IMPL;       \
+        /* We also use HPyFunc_KEYWORDS for HPy_tp_call which is */       \
+        /* called via vectorcall and so nargsf may have the flag set */   \
+        return _h2py(func(_HPyGetContext(), _py2h(self), _arr_py2h(args), \
+                          PyVectorcall_NARGS(nargsf), _py2h(kwnames)));   \
+    }
+
+typedef int (*_HPyCFunction_INITPROC)(HPyContext*, HPy, const HPy *, HPy_ssize_t, HPy);
+#define _HPyFunc_TRAMPOLINE_HPyFunc_INITPROC(SYM, IMPL)                 \
+    static int                                                          \
     SYM(PyObject *self, PyObject *args, PyObject *kw)                   \
     {                                                                   \
         /* get the tuple elements as an array of "PyObject *", which */ \
         /* is equivalent to an array of "HPy" with enough casting... */ \
-        HPy *items = (HPy *)&PyTuple_GET_ITEM(args, 0);                 \
+        PyObject *const *items = &PyTuple_GET_ITEM(args, 0);            \
         Py_ssize_t nargs = PyTuple_GET_SIZE(args);                      \
-        _HPyCFunction_KEYWORDS func = (_HPyCFunction_KEYWORDS)IMPL; \
-        return _h2py(func(_HPyGetContext(), _py2h(self),                \
-                                 items, nargs, _py2h(kw)));             \
+        _HPyCFunction_INITPROC func = (_HPyCFunction_INITPROC)IMPL; \
+        return func(_HPyGetContext(), _py2h(self),                      \
+                    _arr_py2h(items), nargs, _py2h(kw));                \
     }
 
-typedef int (*_HPyCFunction_INITPROC)(HPyContext*, HPy, HPy *, HPy_ssize_t, HPy);
-#define _HPyFunc_TRAMPOLINE_HPyFunc_INITPROC(SYM, IMPL)                 \
-    static int                                                          \
+typedef HPy (*_HPyCFunction_NEWFUNC)(HPyContext*, HPy, const HPy *, HPy_ssize_t, HPy);
+#define _HPyFunc_TRAMPOLINE_HPyFunc_NEWFUNC(SYM, IMPL)                  \
+    static PyObject *                                                   \
     SYM(PyObject *self, PyObject *args, PyObject *kw)                   \
     {                                                                   \
         /* get the tuple elements as an array of "PyObject *", which */ \
         /* is equivalent to an array of "HPy" with enough casting... */ \
-        HPy *items = (HPy *)&PyTuple_GET_ITEM(args, 0);                 \
+        PyObject *const *items = &PyTuple_GET_ITEM(args, 0);            \
         Py_ssize_t nargs = PyTuple_GET_SIZE(args);                      \
-        _HPyCFunction_INITPROC func = (_HPyCFunction_INITPROC)IMPL; \
-        return func(_HPyGetContext(), _py2h(self),                      \
-                    items, nargs, _py2h(kw));                           \
+        _HPyCFunction_NEWFUNC func = (_HPyCFunction_NEWFUNC)IMPL;       \
+        return _h2py(func(_HPyGetContext(), _py2h(self),                \
+                         _arr_py2h(items), nargs, _py2h(kw)));          \
     }
 
 /* special case: the HPy_tp_destroy slot doesn't map to any CPython slot.
    Instead, it is called from our own tp_dealloc: see also
    hpytype_dealloc(). */
 #define _HPyFunc_TRAMPOLINE_HPyFunc_DESTROYFUNC(SYM, IMPL)              \
     static void SYM(void) { abort(); }
@@ -71,26 +61,26 @@
 /* this needs to be written manually because HPy has a different type for
    "op": HPy_RichCmpOp instead of int */
 typedef HPy (*_HPyCFunction_RICHCMPFUNC)(HPyContext *, HPy, HPy, int);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_RICHCMPFUNC(SYM, IMPL)                 \
     static cpy_PyObject *                                                  \
     SYM(PyObject *self, PyObject *obj, int op)                             \
     {                                                                      \
-        _HPyCFunction_RICHCMPFUNC func = (_HPyCFunction_RICHCMPFUNC)IMPL; \
+        _HPyCFunction_RICHCMPFUNC func = (_HPyCFunction_RICHCMPFUNC)IMPL;  \
         return _h2py(func(_HPyGetContext(), _py2h(self), _py2h(obj), op)); \
     }
 
 /* With the cpython ABI, Py_buffer and HPy_buffer are ABI-compatible.
  * Even though casting between them is technically undefined behavior, it
  * should always work. That way, we avoid a costly allocation and copy. */
 typedef int (*_HPyCFunction_GETBUFFERPROC)(HPyContext *, HPy, HPy_buffer *, int);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_GETBUFFERPROC(SYM, IMPL) \
     static int SYM(PyObject *arg0, Py_buffer *arg1, int arg2) \
     { \
-        _HPyCFunction_GETBUFFERPROC func = (_HPyCFunction_GETBUFFERPROC)IMPL; \
+        _HPyCFunction_GETBUFFERPROC func = (_HPyCFunction_GETBUFFERPROC)IMPL;  \
         return (func(_HPyGetContext(), _py2h(arg0), (HPy_buffer*)arg1, arg2)); \
     }
 
 typedef int (*_HPyCFunction_RELEASEBUFFERPROC)(HPyContext *, HPy, HPy_buffer *);
 #define _HPyFunc_TRAMPOLINE_HPyFunc_RELEASEBUFFERPROC(SYM, IMPL) \
     static void SYM(PyObject *arg0, Py_buffer *arg1) \
     { \
@@ -103,8 +93,28 @@
 #define _HPyFunc_TRAMPOLINE_HPyFunc_TRAVERSEPROC(SYM, IMPL)             \
     static int SYM(cpy_PyObject *self, cpy_visitproc visit, void *arg)  \
     {                                                                   \
         return call_traverseproc_from_trampoline((HPyFunc_traverseproc)IMPL, self,            \
                                                  visit, arg);           \
     }
 
+#define HPyCapsule_DESTRUCTOR_TRAMPOLINE(SYM, IMPL)                            \
+    static void SYM(PyObject *capsule)                                         \
+    {                                                                          \
+        const char *name = PyCapsule_GetName(capsule);                         \
+        IMPL(name, PyCapsule_GetPointer(capsule, name),                        \
+                PyCapsule_GetContext(capsule));                                \
+    }
+
+extern void
+_HPyModule_CheckCreateSlotResult(cpy_PyObject **result);
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_MOD_CREATE(SYM, IMPL)                      \
+    static cpy_PyObject* SYM(cpy_PyObject *spec, cpy_PyModuleDef *def)         \
+    {                                                                          \
+        (void) def; /* avoid 'unused' warning */                               \
+        cpy_PyObject* result = _h2py(IMPL(_HPyGetContext(), _py2h(spec)));     \
+        _HPyModule_CheckCreateSlotResult(&result);                             \
+        return result;                                                         \
+    }
+
 #endif // HPY_CPYTHON_HPYFUNC_TRAMPOLINES_H
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/cpython/misc.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/cpython/misc.h`

 * *Files 22% similar despite different names*

```diff
@@ -41,107 +41,27 @@
 
 static inline PyObject * _hg2py(HPyGlobal hf)
 {
     HPy h = { ._i = hf._i };
     return _h2py(h);
 }
 
-// this should maybe autogenerated from public_api.h
-struct _HPyContext_s {
-    const char *name;
-    /* Constants */
-    HPy h_None;
-    HPy h_True;
-    HPy h_False;
-    HPy h_NotImplemented;
-    HPy h_Ellipsis;
-    /* Exceptions */
-    HPy h_BaseException;
-    HPy h_Exception;
-    HPy h_StopAsyncIteration;
-    HPy h_StopIteration;
-    HPy h_GeneratorExit;
-    HPy h_ArithmeticError;
-    HPy h_LookupError;
-    HPy h_AssertionError;
-    HPy h_AttributeError;
-    HPy h_BufferError;
-    HPy h_EOFError;
-    HPy h_FloatingPointError;
-    HPy h_OSError;
-    HPy h_ImportError;
-    HPy h_ModuleNotFoundError;
-    HPy h_IndexError;
-    HPy h_KeyError;
-    HPy h_KeyboardInterrupt;
-    HPy h_MemoryError;
-    HPy h_NameError;
-    HPy h_OverflowError;
-    HPy h_RuntimeError;
-    HPy h_RecursionError;
-    HPy h_NotImplementedError;
-    HPy h_SyntaxError;
-    HPy h_IndentationError;
-    HPy h_TabError;
-    HPy h_ReferenceError;
-    HPy h_SystemError;
-    HPy h_SystemExit;
-    HPy h_TypeError;
-    HPy h_UnboundLocalError;
-    HPy h_UnicodeError;
-    HPy h_UnicodeEncodeError;
-    HPy h_UnicodeDecodeError;
-    HPy h_UnicodeTranslateError;
-    HPy h_ValueError;
-    HPy h_ZeroDivisionError;
-    HPy h_BlockingIOError;
-    HPy h_BrokenPipeError;
-    HPy h_ChildProcessError;
-    HPy h_ConnectionError;
-    HPy h_ConnectionAbortedError;
-    HPy h_ConnectionRefusedError;
-    HPy h_ConnectionResetError;
-    HPy h_FileExistsError;
-    HPy h_FileNotFoundError;
-    HPy h_InterruptedError;
-    HPy h_IsADirectoryError;
-    HPy h_NotADirectoryError;
-    HPy h_PermissionError;
-    HPy h_ProcessLookupError;
-    HPy h_TimeoutError;
-    /* Warnings */
-    HPy h_Warning;
-    HPy h_UserWarning;
-    HPy h_DeprecationWarning;
-    HPy h_PendingDeprecationWarning;
-    HPy h_SyntaxWarning;
-    HPy h_RuntimeWarning;
-    HPy h_FutureWarning;
-    HPy h_ImportWarning;
-    HPy h_UnicodeWarning;
-    HPy h_BytesWarning;
-    HPy h_ResourceWarning;
-    /* Types */
-    HPy h_BaseObjectType;
-    HPy h_TypeType;
-    HPy h_BoolType;
-    HPy h_LongType;
-    HPy h_FloatType;
-    HPy h_UnicodeType;
-    HPy h_TupleType;
-    HPy h_ListType;
-};
+static inline const HPy *_arr_py2h(PyObject *const *py_arr) {
+    assert(sizeof(HPy) == sizeof(PyObject *));
+    return (const HPy *)py_arr;
+}
 
 /* XXX! should be defined only once, not once for every .c! */
 static struct _HPyContext_s _global_ctx;
 
 HPyAPI_FUNC HPyContext * _HPyGetContext(void) {
     HPyContext *ctx = &_global_ctx;
     if (!ctx->name) {
-        ctx->name = "HPy CPython ABI",
+        ctx->name = "HPy CPython ABI";
+        ctx->abi_version = HPY_ABI_VERSION;
         /* Constants */
         ctx->h_None = _py2h(Py_None);
         ctx->h_True = _py2h(Py_True);
         ctx->h_False = _py2h(Py_False);
         ctx->h_NotImplemented = _py2h(Py_NotImplemented);
         ctx->h_Ellipsis = _py2h(Py_Ellipsis);
         /* Exceptions */
@@ -215,14 +135,21 @@
         ctx->h_TypeType = _py2h((PyObject *)&PyType_Type);
         ctx->h_BoolType = _py2h((PyObject *)&PyBool_Type);
         ctx->h_LongType = _py2h((PyObject *)&PyLong_Type);
         ctx->h_FloatType = _py2h((PyObject *)&PyFloat_Type);
         ctx->h_UnicodeType = _py2h((PyObject *)&PyUnicode_Type);
         ctx->h_TupleType = _py2h((PyObject *)&PyTuple_Type);
         ctx->h_ListType = _py2h((PyObject *)&PyList_Type);
+        ctx->h_ComplexType = _py2h((PyObject *)&PyComplex_Type);
+        ctx->h_BytesType = _py2h((PyObject *)&PyBytes_Type);
+        ctx->h_MemoryViewType = _py2h((PyObject *)&PyMemoryView_Type);
+        ctx->h_CapsuleType = _py2h((PyObject *)&PyCapsule_Type);
+        ctx->h_SliceType = _py2h((PyObject *)&PySlice_Type);
+        /* Reflection */
+        ctx->h_Builtins = _py2h(PyEval_GetBuiltins());
     }
     return ctx;
 }
 
 HPyAPI_FUNC HPy HPy_Dup(HPyContext *ctx, HPy handle)
 {
     Py_XINCREF(_h2py(handle));
@@ -295,34 +222,88 @@
 }
 
 HPyAPI_FUNC _HPy_NO_RETURN void HPy_FatalError(HPyContext *ctx, const char *message)
 {
     Py_FatalError(message);
 }
 
-HPyAPI_FUNC HPy HPyType_GenericNew(HPyContext *ctx, HPy type, HPy *args, HPy_ssize_t nargs, HPy kw)
+HPyAPI_FUNC HPy HPyType_GenericNew(HPyContext *ctx, HPy type, const HPy *args, HPy_ssize_t nargs, HPy kw)
 {
     return ctx_Type_GenericNew(ctx, type, args, nargs, kw);
 }
 
-HPyAPI_FUNC void* HPy_AsStruct(HPyContext *ctx, HPy h)
+HPyAPI_FUNC void* _HPy_AsStruct_Object(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_Object(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_Legacy(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_Legacy(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_Type(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_Type(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_Long(HPyContext *ctx, HPy h)
 {
-    return ctx_AsStruct(ctx, h);
+    return ctx_AsStruct_Long(ctx, h);
 }
 
-HPyAPI_FUNC void* HPy_AsStructLegacy(HPyContext *ctx, HPy h)
+HPyAPI_FUNC void* _HPy_AsStruct_Float(HPyContext *ctx, HPy h)
 {
-    return ctx_AsStructLegacy(ctx, h);
+    return ctx_AsStruct_Float(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_Unicode(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_Unicode(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_Tuple(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_Tuple(ctx, h);
+}
+
+HPyAPI_FUNC void* _HPy_AsStruct_List(HPyContext *ctx, HPy h)
+{
+    return ctx_AsStruct_List(ctx, h);
 }
 
 HPyAPI_FUNC HPy HPy_CallTupleDict(HPyContext *ctx, HPy callable, HPy args, HPy kw)
 {
     return ctx_CallTupleDict(ctx, callable, args, kw);
 }
 
+#if PY_VERSION_HEX < 0x03090000
+#    define PyObject_Vectorcall _PyObject_Vectorcall
+#endif
+
+HPyAPI_FUNC HPy HPy_Call(HPyContext *ctx, HPy callable, const HPy *args, size_t nargs, HPy kwnames)
+{
+    assert(sizeof(HPy) == sizeof(PyObject *));
+    return _py2h(PyObject_Vectorcall(_h2py(callable), (PyObject *const *)args, nargs, _h2py(kwnames)));
+}
+
+#if PY_VERSION_HEX < 0x03090000
+#    undef PyObject_Vectorcall
+#endif
+
+HPyAPI_FUNC HPy HPy_CallMethod(HPyContext *ctx, HPy name, const HPy *args, size_t nargs, HPy kwnames)
+{
+#if PY_VERSION_HEX >= 0x03090000
+    assert(sizeof(HPy) == sizeof(PyObject *));
+    return _py2h(PyObject_VectorcallMethod(_h2py(name), (PyObject *const *)args, nargs, _h2py(kwnames)));
+#else
+    return ctx_CallMethod(ctx, name, args, nargs, kwnames);
+#endif
+}
+
 HPyAPI_FUNC void _HPy_Dump(HPyContext *ctx, HPy h)
 {
     ctx_Dump(ctx, h);
 }
 
 HPyAPI_FUNC int HPy_TypeCheck(HPyContext *ctx, HPy h_obj, HPy h_type)
 {
@@ -413,16 +394,169 @@
     return ctx_SetItem_i(ctx, obj, idx, value);
 }
 
 HPyAPI_FUNC int HPy_SetItem_s(HPyContext *ctx, HPy obj, const char *key, HPy value) {
     return ctx_SetItem_s(ctx, obj, key, value);
 }
 
+HPyAPI_FUNC int HPy_DelItem_i(HPyContext *ctx, HPy obj, HPy_ssize_t idx) {
+    return ctx_DelItem_i(ctx, obj, idx);
+}
+
+HPyAPI_FUNC int HPy_DelItem_s(HPyContext *ctx, HPy obj, const char *key) {
+    return ctx_DelItem_s(ctx, obj, key);
+}
+
 HPyAPI_FUNC HPy HPyBytes_FromStringAndSize(HPyContext *ctx, const char *v, HPy_ssize_t len) {
     return ctx_Bytes_FromStringAndSize(ctx, v, len);
 }
 
 HPyAPI_FUNC int HPyErr_Occurred(HPyContext *ctx) {
     return ctx_Err_Occurred(ctx);
 }
 
+HPyAPI_FUNC HPy HPyCapsule_New(HPyContext *ctx, void *pointer, const char *name, HPyCapsule_Destructor *destructor)
+{
+    return ctx_Capsule_New(ctx, pointer, name, destructor);
+}
+
+HPyAPI_FUNC void * HPyCapsule_GetPointer(HPyContext *ctx, HPy capsule, const char *name)
+{
+    return PyCapsule_GetPointer(_h2py(capsule), name);
+}
+
+HPyAPI_FUNC const char * HPyCapsule_GetName(HPyContext *ctx, HPy capsule)
+{
+    return PyCapsule_GetName(_h2py(capsule));
+}
+
+HPyAPI_FUNC void * HPyCapsule_GetContext(HPyContext *ctx, HPy capsule)
+{
+    return PyCapsule_GetContext(_h2py(capsule));
+}
+
+HPyAPI_FUNC int HPyCapsule_SetPointer(HPyContext *ctx, HPy capsule, void *pointer)
+{
+    return PyCapsule_SetPointer(_h2py(capsule), pointer);
+}
+
+HPyAPI_FUNC int HPyCapsule_SetName(HPyContext *ctx, HPy capsule, const char *name)
+{
+    return PyCapsule_SetName(_h2py(capsule), name);
+}
+
+HPyAPI_FUNC int HPyCapsule_SetContext(HPyContext *ctx, HPy capsule, void *context)
+{
+    return PyCapsule_SetContext(_h2py(capsule), context);
+}
+
+HPyAPI_FUNC int HPyCapsule_SetDestructor(HPyContext *ctx, HPy capsule, HPyCapsule_Destructor *destructor)
+{
+    return ctx_Capsule_SetDestructor(ctx, capsule, destructor);
+}
+
+// just for better readability
+#define SIZEOF_INT32 4
+#define SIZEOF_INT64 8
+
+HPyAPI_FUNC HPy HPyLong_FromInt32_t(HPyContext *ctx, int32_t value) {
+#if SIZEOF_LONG >= SIZEOF_INT32
+     return _py2h(PyLong_FromLong((long)value));
+#else
+     return ctx_Long_FromInt32_t ( ctx, value );
+#endif
+}
+
+HPyAPI_FUNC HPy HPyLong_FromUInt32_t(HPyContext *ctx, uint32_t value) {
+#if SIZEOF_LONG >= SIZEOF_INT32
+     return _py2h(PyLong_FromUnsignedLong((unsigned long)value));
+#else
+     return ctx_Long_FromUInt32_t ( ctx, value );
+#endif
+}
+
+HPyAPI_FUNC HPy HPyLong_FromInt64_t(HPyContext *ctx, int64_t v) {
+#if  SIZEOF_LONG_LONG >= SIZEOF_INT64
+     return _py2h(PyLong_FromLongLong((long long)v));
+#else
+     return ctx_Long_FromInt64_t ( ctx, v );
+#endif
+}
+
+HPyAPI_FUNC HPy HPyLong_FromUInt64_t(HPyContext *ctx, uint64_t v) {
+#if  SIZEOF_LONG_LONG >= SIZEOF_INT64
+     return _py2h(PyLong_FromUnsignedLongLong((unsigned long long)v));
+#else
+     return ctx_Long_FromUInt64_t ( ctx, v );
+#endif
+}
+
+HPyAPI_FUNC int32_t HPyLong_AsInt32_t(HPyContext *ctx, HPy h) {
+#if SIZEOF_LONG == SIZEOF_INT32
+     return (int32_t) PyLong_AsLong(_h2py(h));
+#else
+     return ctx_Long_AsInt32_t ( ctx, h );
+#endif
+}
+
+HPyAPI_FUNC uint32_t HPyLong_AsUInt32_t(HPyContext *ctx, HPy h) {
+#if SIZEOF_LONG == SIZEOF_INT32
+     return (uint32_t) PyLong_AsUnsignedLong(_h2py(h));
+#else
+     return ctx_Long_AsUInt32_t ( ctx, h );
+#endif
+}
+
+HPyAPI_FUNC uint32_t HPyLong_AsUInt32_tMask(HPyContext *ctx, HPy h) {
+     return (uint32_t) PyLong_AsUnsignedLongMask(_h2py(h));
+}
+
+HPyAPI_FUNC int64_t HPyLong_AsInt64_t(HPyContext *ctx, HPy h) {
+#if SIZEOF_LONG_LONG == SIZEOF_INT64
+     return (int64_t) PyLong_AsLongLong(_h2py(h));
+#else
+     return ctx_Long_AsInt64_t ( ctx, h );
+#endif
+}
+
+HPyAPI_FUNC uint64_t HPyLong_AsUInt64_t(HPyContext *ctx, HPy h) {
+#if SIZEOF_LONG_LONG == SIZEOF_INT64
+     return (uint64_t) PyLong_AsUnsignedLongLong(_h2py(h));
+#else
+     return ctx_Long_AsUInt64_t ( ctx, h );
+#endif
+}
+
+HPyAPI_FUNC uint64_t HPyLong_AsUInt64_tMask(HPyContext *ctx, HPy h) {
+     return (uint64_t) PyLong_AsUnsignedLongLongMask(_h2py(h));
+}
+
+#undef SIZEOF_INT32
+#undef SIZEOF_INT64
+
+HPyAPI_FUNC HPy HPy_Compile_s(HPyContext *ctx, const char *utf8_source, const char *utf8_filename, HPy_SourceKind kind) {
+    return ctx_Compile_s(ctx, utf8_source, utf8_filename, kind);
+}
+
+HPyAPI_FUNC int32_t
+HPyContextVar_Get(HPyContext *ctx, HPy context_var, HPy default_value, HPy *result) {
+    return ctx_ContextVar_Get(ctx, context_var, default_value, result);
+}
+
+HPyAPI_FUNC const char *
+HPyType_GetName(HPyContext *ctx, HPy type)
+{
+    return ctx_Type_GetName(ctx, type);
+}
+
+HPyAPI_FUNC int HPyType_IsSubtype(HPyContext *ctx, HPy sub, HPy type)
+{
+    return PyType_IsSubtype((PyTypeObject *)_h2py(sub),
+            (PyTypeObject *)_h2py(type));
+}
+
+HPyAPI_FUNC int HPy_SetCallFunction(HPyContext *ctx, HPy h, HPyCallFunction *func)
+{
+    return ctx_SetCallFunction(ctx, h, func);
+}
+
 #endif /* !HPY_CPYTHON_MISC_H */
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/hpyfunc.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/hpyfunc.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #ifndef HPY_UNIVERSAL_HPYFUNC_H
 #define HPY_UNIVERSAL_HPYFUNC_H
 
 typedef enum {
-    HPyFunc_VARARGS  = 1,  // METH_VARARGS
-    HPyFunc_KEYWORDS = 2,  // METH_VARARGS | METH_KEYWORDS
+    HPyFunc_VARARGS  = 1,  // METH_FASTCALL
+    HPyFunc_KEYWORDS = 2,  // METH_FASTCALL | METH_KEYWORDS
     HPyFunc_NOARGS   = 3,  // METH_NOARGS
     HPyFunc_O        = 4,  // METH_O
 
     HPyFunc_DESTROYFUNC,
 
     HPyFunc_GETBUFFERPROC,
     HPyFunc_RELEASEBUFFERPROC,
@@ -30,19 +30,24 @@
     HPyFunc_HASHFUNC,
     HPyFunc_RICHCMPFUNC,
     HPyFunc_GETITERFUNC,
     HPyFunc_ITERNEXTFUNC,
     HPyFunc_DESCRGETFUNC,
     HPyFunc_DESCRSETFUNC,
     HPyFunc_INITPROC,
+    HPyFunc_NEWFUNC,
     HPyFunc_GETTER,
     HPyFunc_SETTER,
     HPyFunc_OBJOBJPROC,
     HPyFunc_TRAVERSEPROC,
     HPyFunc_DESTRUCTOR,
+    HPyFunc_CAPSULE_DESTRUCTOR,
+    HPyFunc_VECTORCALLFUNC,
+
+    HPyFunc_MOD_CREATE,
 
 } HPyFunc_Signature;
 
 /* The typedefs corresponding to the various HPyFunc_Signature members
    are produced inside autogen_hpyfunc_declare.h. */
 
 
@@ -105,16 +110,16 @@
             }                                                           \
     } while (0)
 
 
 
 #include "autogen_hpyfunc_declare.h"
 
-#ifdef HPY_UNIVERSAL_ABI
-#  include "universal/hpyfunc_trampolines.h"
-#  include "universal/autogen_hpyfunc_trampolines.h"
-#else
+#ifdef HPY_ABI_CPYTHON
 #  include "cpython/hpyfunc_trampolines.h"
 #  include "cpython/autogen_hpyfunc_trampolines.h"
-#endif // HPY_UNIVERSAL_ABI
+#else
+#  include "universal/hpyfunc_trampolines.h"
+#  include "universal/autogen_hpyfunc_trampolines.h"
+#endif // HPY_ABI_CPYTHON
 
 #endif /* HPY_UNIVERSAL_HPYFUNC_H */
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/macros.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/macros.h`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_ctx.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_ctx.h`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
        make autogen
 
 */
 
 struct _HPyContext_s {
     const char *name; // used just to make debugging and testing easier
     void *_private;   // used by implementations to store custom data
-    int ctx_version;
+    int abi_version;
     HPy h_None;
     HPy h_True;
     HPy h_False;
     HPy h_NotImplemented;
     HPy h_Ellipsis;
     HPy h_BaseException;
     HPy h_Exception;
@@ -87,36 +87,35 @@
     HPy h_TypeType;
     HPy h_BoolType;
     HPy h_LongType;
     HPy h_FloatType;
     HPy h_UnicodeType;
     HPy h_TupleType;
     HPy h_ListType;
-    HPy (*ctx_Module_Create)(HPyContext *ctx, HPyModuleDef *def);
     HPy (*ctx_Dup)(HPyContext *ctx, HPy h);
     void (*ctx_Close)(HPyContext *ctx, HPy h);
-    HPy (*ctx_Long_FromLong)(HPyContext *ctx, long value);
-    HPy (*ctx_Long_FromUnsignedLong)(HPyContext *ctx, unsigned long value);
-    HPy (*ctx_Long_FromLongLong)(HPyContext *ctx, long long v);
-    HPy (*ctx_Long_FromUnsignedLongLong)(HPyContext *ctx, unsigned long long v);
+    HPy (*ctx_Long_FromInt32_t)(HPyContext *ctx, int32_t value);
+    HPy (*ctx_Long_FromUInt32_t)(HPyContext *ctx, uint32_t value);
+    HPy (*ctx_Long_FromInt64_t)(HPyContext *ctx, int64_t v);
+    HPy (*ctx_Long_FromUInt64_t)(HPyContext *ctx, uint64_t v);
     HPy (*ctx_Long_FromSize_t)(HPyContext *ctx, size_t value);
     HPy (*ctx_Long_FromSsize_t)(HPyContext *ctx, HPy_ssize_t value);
-    long (*ctx_Long_AsLong)(HPyContext *ctx, HPy h);
-    unsigned long (*ctx_Long_AsUnsignedLong)(HPyContext *ctx, HPy h);
-    unsigned long (*ctx_Long_AsUnsignedLongMask)(HPyContext *ctx, HPy h);
-    long long (*ctx_Long_AsLongLong)(HPyContext *ctx, HPy h);
-    unsigned long long (*ctx_Long_AsUnsignedLongLong)(HPyContext *ctx, HPy h);
-    unsigned long long (*ctx_Long_AsUnsignedLongLongMask)(HPyContext *ctx, HPy h);
+    int32_t (*ctx_Long_AsInt32_t)(HPyContext *ctx, HPy h);
+    uint32_t (*ctx_Long_AsUInt32_t)(HPyContext *ctx, HPy h);
+    uint32_t (*ctx_Long_AsUInt32_tMask)(HPyContext *ctx, HPy h);
+    int64_t (*ctx_Long_AsInt64_t)(HPyContext *ctx, HPy h);
+    uint64_t (*ctx_Long_AsUInt64_t)(HPyContext *ctx, HPy h);
+    uint64_t (*ctx_Long_AsUInt64_tMask)(HPyContext *ctx, HPy h);
     size_t (*ctx_Long_AsSize_t)(HPyContext *ctx, HPy h);
     HPy_ssize_t (*ctx_Long_AsSsize_t)(HPyContext *ctx, HPy h);
     void *(*ctx_Long_AsVoidPtr)(HPyContext *ctx, HPy h);
     double (*ctx_Long_AsDouble)(HPyContext *ctx, HPy h);
     HPy (*ctx_Float_FromDouble)(HPyContext *ctx, double v);
     double (*ctx_Float_AsDouble)(HPyContext *ctx, HPy h);
-    HPy (*ctx_Bool_FromLong)(HPyContext *ctx, long v);
+    HPy (*ctx_Bool_FromBool)(HPyContext *ctx, bool v);
     HPy_ssize_t (*ctx_Length)(HPyContext *ctx, HPy h);
     int (*ctx_Number_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_Add)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_Subtract)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_Multiply)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_MatrixMultiply)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_FloorDivide)(HPyContext *ctx, HPy h1, HPy h2);
@@ -148,99 +147,134 @@
     HPy (*ctx_InPlaceRshift)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_InPlaceAnd)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_InPlaceXor)(HPyContext *ctx, HPy h1, HPy h2);
     HPy (*ctx_InPlaceOr)(HPyContext *ctx, HPy h1, HPy h2);
     int (*ctx_Callable_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_CallTupleDict)(HPyContext *ctx, HPy callable, HPy args, HPy kw);
     void (*ctx_FatalError)(HPyContext *ctx, const char *message);
-    void (*ctx_Err_SetString)(HPyContext *ctx, HPy h_type, const char *message);
+    void (*ctx_Err_SetString)(HPyContext *ctx, HPy h_type, const char *utf8_message);
     void (*ctx_Err_SetObject)(HPyContext *ctx, HPy h_type, HPy h_value);
     HPy (*ctx_Err_SetFromErrnoWithFilename)(HPyContext *ctx, HPy h_type, const char *filename_fsencoded);
     void (*ctx_Err_SetFromErrnoWithFilenameObjects)(HPyContext *ctx, HPy h_type, HPy filename1, HPy filename2);
     int (*ctx_Err_Occurred)(HPyContext *ctx);
     int (*ctx_Err_ExceptionMatches)(HPyContext *ctx, HPy exc);
     void (*ctx_Err_NoMemory)(HPyContext *ctx);
     void (*ctx_Err_Clear)(HPyContext *ctx);
-    HPy (*ctx_Err_NewException)(HPyContext *ctx, const char *name, HPy base, HPy dict);
-    HPy (*ctx_Err_NewExceptionWithDoc)(HPyContext *ctx, const char *name, const char *doc, HPy base, HPy dict);
-    int (*ctx_Err_WarnEx)(HPyContext *ctx, HPy category, const char *message, HPy_ssize_t stack_level);
+    HPy (*ctx_Err_NewException)(HPyContext *ctx, const char *utf8_name, HPy base, HPy dict);
+    HPy (*ctx_Err_NewExceptionWithDoc)(HPyContext *ctx, const char *utf8_name, const char *utf8_doc, HPy base, HPy dict);
+    int (*ctx_Err_WarnEx)(HPyContext *ctx, HPy category, const char *utf8_message, HPy_ssize_t stack_level);
     void (*ctx_Err_WriteUnraisable)(HPyContext *ctx, HPy obj);
     int (*ctx_IsTrue)(HPyContext *ctx, HPy h);
     HPy (*ctx_Type_FromSpec)(HPyContext *ctx, HPyType_Spec *spec, HPyType_SpecParam *params);
-    HPy (*ctx_Type_GenericNew)(HPyContext *ctx, HPy type, HPy *args, HPy_ssize_t nargs, HPy kw);
+    HPy (*ctx_Type_GenericNew)(HPyContext *ctx, HPy type, const HPy *args, HPy_ssize_t nargs, HPy kw);
     HPy (*ctx_GetAttr)(HPyContext *ctx, HPy obj, HPy name);
-    HPy (*ctx_GetAttr_s)(HPyContext *ctx, HPy obj, const char *name);
+    HPy (*ctx_GetAttr_s)(HPyContext *ctx, HPy obj, const char *utf8_name);
     int (*ctx_HasAttr)(HPyContext *ctx, HPy obj, HPy name);
-    int (*ctx_HasAttr_s)(HPyContext *ctx, HPy obj, const char *name);
+    int (*ctx_HasAttr_s)(HPyContext *ctx, HPy obj, const char *utf8_name);
     int (*ctx_SetAttr)(HPyContext *ctx, HPy obj, HPy name, HPy value);
-    int (*ctx_SetAttr_s)(HPyContext *ctx, HPy obj, const char *name, HPy value);
+    int (*ctx_SetAttr_s)(HPyContext *ctx, HPy obj, const char *utf8_name, HPy value);
     HPy (*ctx_GetItem)(HPyContext *ctx, HPy obj, HPy key);
     HPy (*ctx_GetItem_i)(HPyContext *ctx, HPy obj, HPy_ssize_t idx);
-    HPy (*ctx_GetItem_s)(HPyContext *ctx, HPy obj, const char *key);
+    HPy (*ctx_GetItem_s)(HPyContext *ctx, HPy obj, const char *utf8_key);
     int (*ctx_Contains)(HPyContext *ctx, HPy container, HPy key);
     int (*ctx_SetItem)(HPyContext *ctx, HPy obj, HPy key, HPy value);
     int (*ctx_SetItem_i)(HPyContext *ctx, HPy obj, HPy_ssize_t idx, HPy value);
-    int (*ctx_SetItem_s)(HPyContext *ctx, HPy obj, const char *key, HPy value);
+    int (*ctx_SetItem_s)(HPyContext *ctx, HPy obj, const char *utf8_key, HPy value);
     HPy (*ctx_Type)(HPyContext *ctx, HPy obj);
     int (*ctx_TypeCheck)(HPyContext *ctx, HPy obj, HPy type);
     int (*ctx_Is)(HPyContext *ctx, HPy obj, HPy other);
-    void *(*ctx_AsStruct)(HPyContext *ctx, HPy h);
-    void *(*ctx_AsStructLegacy)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Object)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Legacy)(HPyContext *ctx, HPy h);
     HPy (*ctx_New)(HPyContext *ctx, HPy h_type, void **data);
     HPy (*ctx_Repr)(HPyContext *ctx, HPy obj);
     HPy (*ctx_Str)(HPyContext *ctx, HPy obj);
     HPy (*ctx_ASCII)(HPyContext *ctx, HPy obj);
     HPy (*ctx_Bytes)(HPyContext *ctx, HPy obj);
     HPy (*ctx_RichCompare)(HPyContext *ctx, HPy v, HPy w, int op);
     int (*ctx_RichCompareBool)(HPyContext *ctx, HPy v, HPy w, int op);
     HPy_hash_t (*ctx_Hash)(HPyContext *ctx, HPy obj);
     int (*ctx_Bytes_Check)(HPyContext *ctx, HPy h);
     HPy_ssize_t (*ctx_Bytes_Size)(HPyContext *ctx, HPy h);
     HPy_ssize_t (*ctx_Bytes_GET_SIZE)(HPyContext *ctx, HPy h);
-    char *(*ctx_Bytes_AsString)(HPyContext *ctx, HPy h);
-    char *(*ctx_Bytes_AS_STRING)(HPyContext *ctx, HPy h);
-    HPy (*ctx_Bytes_FromString)(HPyContext *ctx, const char *v);
-    HPy (*ctx_Bytes_FromStringAndSize)(HPyContext *ctx, const char *v, HPy_ssize_t len);
+    const char *(*ctx_Bytes_AsString)(HPyContext *ctx, HPy h);
+    const char *(*ctx_Bytes_AS_STRING)(HPyContext *ctx, HPy h);
+    HPy (*ctx_Bytes_FromString)(HPyContext *ctx, const char *bytes);
+    HPy (*ctx_Bytes_FromStringAndSize)(HPyContext *ctx, const char *bytes, HPy_ssize_t len);
     HPy (*ctx_Unicode_FromString)(HPyContext *ctx, const char *utf8);
     int (*ctx_Unicode_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_Unicode_AsASCIIString)(HPyContext *ctx, HPy h);
     HPy (*ctx_Unicode_AsLatin1String)(HPyContext *ctx, HPy h);
     HPy (*ctx_Unicode_AsUTF8String)(HPyContext *ctx, HPy h);
     const char *(*ctx_Unicode_AsUTF8AndSize)(HPyContext *ctx, HPy h, HPy_ssize_t *size);
     HPy (*ctx_Unicode_FromWideChar)(HPyContext *ctx, const wchar_t *w, HPy_ssize_t size);
     HPy (*ctx_Unicode_DecodeFSDefault)(HPyContext *ctx, const char *v);
     HPy (*ctx_Unicode_DecodeFSDefaultAndSize)(HPyContext *ctx, const char *v, HPy_ssize_t size);
     HPy (*ctx_Unicode_EncodeFSDefault)(HPyContext *ctx, HPy h);
     HPy_UCS4 (*ctx_Unicode_ReadChar)(HPyContext *ctx, HPy h, HPy_ssize_t index);
-    HPy (*ctx_Unicode_DecodeASCII)(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors);
-    HPy (*ctx_Unicode_DecodeLatin1)(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors);
+    HPy (*ctx_Unicode_DecodeASCII)(HPyContext *ctx, const char *ascii, HPy_ssize_t size, const char *errors);
+    HPy (*ctx_Unicode_DecodeLatin1)(HPyContext *ctx, const char *latin1, HPy_ssize_t size, const char *errors);
     int (*ctx_List_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_List_New)(HPyContext *ctx, HPy_ssize_t len);
     int (*ctx_List_Append)(HPyContext *ctx, HPy h_list, HPy h_item);
     int (*ctx_Dict_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_Dict_New)(HPyContext *ctx);
     int (*ctx_Tuple_Check)(HPyContext *ctx, HPy h);
     HPy (*ctx_Tuple_FromArray)(HPyContext *ctx, HPy items[], HPy_ssize_t n);
-    HPy (*ctx_Import_ImportModule)(HPyContext *ctx, const char *name);
+    HPy (*ctx_Import_ImportModule)(HPyContext *ctx, const char *utf8_name);
     HPy (*ctx_FromPyObject)(HPyContext *ctx, cpy_PyObject *obj);
     cpy_PyObject *(*ctx_AsPyObject)(HPyContext *ctx, HPy h);
     void (*ctx_CallRealFunctionFromTrampoline)(HPyContext *ctx, HPyFunc_Signature sig, HPyCFunction func, void *args);
-    HPyListBuilder (*ctx_ListBuilder_New)(HPyContext *ctx, HPy_ssize_t initial_size);
+    HPyListBuilder (*ctx_ListBuilder_New)(HPyContext *ctx, HPy_ssize_t size);
     void (*ctx_ListBuilder_Set)(HPyContext *ctx, HPyListBuilder builder, HPy_ssize_t index, HPy h_item);
     HPy (*ctx_ListBuilder_Build)(HPyContext *ctx, HPyListBuilder builder);
     void (*ctx_ListBuilder_Cancel)(HPyContext *ctx, HPyListBuilder builder);
-    HPyTupleBuilder (*ctx_TupleBuilder_New)(HPyContext *ctx, HPy_ssize_t initial_size);
+    HPyTupleBuilder (*ctx_TupleBuilder_New)(HPyContext *ctx, HPy_ssize_t size);
     void (*ctx_TupleBuilder_Set)(HPyContext *ctx, HPyTupleBuilder builder, HPy_ssize_t index, HPy h_item);
     HPy (*ctx_TupleBuilder_Build)(HPyContext *ctx, HPyTupleBuilder builder);
     void (*ctx_TupleBuilder_Cancel)(HPyContext *ctx, HPyTupleBuilder builder);
     HPyTracker (*ctx_Tracker_New)(HPyContext *ctx, HPy_ssize_t size);
     int (*ctx_Tracker_Add)(HPyContext *ctx, HPyTracker ht, HPy h);
     void (*ctx_Tracker_ForgetAll)(HPyContext *ctx, HPyTracker ht);
     void (*ctx_Tracker_Close)(HPyContext *ctx, HPyTracker ht);
     void (*ctx_Field_Store)(HPyContext *ctx, HPy target_object, HPyField *target_field, HPy h);
     HPy (*ctx_Field_Load)(HPyContext *ctx, HPy source_object, HPyField source_field);
     void (*ctx_ReenterPythonExecution)(HPyContext *ctx, HPyThreadState state);
     HPyThreadState (*ctx_LeavePythonExecution)(HPyContext *ctx);
     void (*ctx_Global_Store)(HPyContext *ctx, HPyGlobal *global, HPy h);
     HPy (*ctx_Global_Load)(HPyContext *ctx, HPyGlobal global);
     void (*ctx_Dump)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Type)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Long)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Float)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Unicode)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_Tuple)(HPyContext *ctx, HPy h);
+    void *(*ctx_AsStruct_List)(HPyContext *ctx, HPy h);
+    HPyType_BuiltinShape (*ctx_Type_GetBuiltinShape)(HPyContext *ctx, HPy h_type);
+    int (*ctx_DelItem)(HPyContext *ctx, HPy obj, HPy key);
+    int (*ctx_DelItem_i)(HPyContext *ctx, HPy obj, HPy_ssize_t idx);
+    int (*ctx_DelItem_s)(HPyContext *ctx, HPy obj, const char *utf8_key);
+    HPy h_ComplexType;
+    HPy h_BytesType;
+    HPy h_MemoryViewType;
+    HPy h_CapsuleType;
+    HPy h_SliceType;
+    HPy h_Builtins;
+    HPy (*ctx_Capsule_New)(HPyContext *ctx, void *pointer, const char *utf8_name, HPyCapsule_Destructor *destructor);
+    void *(*ctx_Capsule_Get)(HPyContext *ctx, HPy capsule, _HPyCapsule_key key, const char *utf8_name);
+    int (*ctx_Capsule_IsValid)(HPyContext *ctx, HPy capsule, const char *utf8_name);
+    int (*ctx_Capsule_Set)(HPyContext *ctx, HPy capsule, _HPyCapsule_key key, void *value);
+    HPy (*ctx_Compile_s)(HPyContext *ctx, const char *utf8_source, const char *utf8_filename, HPy_SourceKind kind);
+    HPy (*ctx_EvalCode)(HPyContext *ctx, HPy code, HPy globals, HPy locals);
+    HPy (*ctx_ContextVar_New)(HPyContext *ctx, const char *name, HPy default_value);
+    int32_t (*ctx_ContextVar_Get)(HPyContext *ctx, HPy context_var, HPy default_value, HPy *result);
+    HPy (*ctx_ContextVar_Set)(HPyContext *ctx, HPy context_var, HPy value);
+    const char *(*ctx_Type_GetName)(HPyContext *ctx, HPy type);
+    int (*ctx_Type_IsSubtype)(HPyContext *ctx, HPy sub, HPy type);
+    HPy (*ctx_Unicode_FromEncodedObject)(HPyContext *ctx, HPy obj, const char *encoding, const char *errors);
+    HPy (*ctx_Unicode_Substring)(HPyContext *ctx, HPy str, HPy_ssize_t start, HPy_ssize_t end);
+    HPy (*ctx_Dict_Keys)(HPyContext *ctx, HPy h);
+    HPy (*ctx_Dict_Copy)(HPyContext *ctx, HPy h);
+    int (*ctx_Slice_Unpack)(HPyContext *ctx, HPy slice, HPy_ssize_t *start, HPy_ssize_t *stop, HPy_ssize_t *step);
+    int (*ctx_SetCallFunction)(HPyContext *ctx, HPy h, HPyCallFunction *func);
+    HPy (*ctx_Call)(HPyContext *ctx, HPy callable, const HPy *args, size_t nargs, HPy kwnames);
+    HPy (*ctx_CallMethod)(HPyContext *ctx, HPy name, const HPy *args, size_t nargs, HPy kwnames);
 };
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,43 @@
 
    Run this to regenerate:
        make autogen
 
 */
 
 typedef struct {
+    cpy_PyObject *self;
+    cpy_PyObject * result;
+} _HPyFunc_args_NOARGS;
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_NOARGS(SYM, IMPL) \
+    static cpy_PyObject *SYM(cpy_PyObject *self) \
+    { \
+        _HPyFunc_args_NOARGS a = { self }; \
+        _HPy_CallRealFunctionFromTrampoline( \
+           _ctx_for_trampolines, HPyFunc_NOARGS, (HPyCFunction)IMPL, &a); \
+        return a.result; \
+    }
+
+typedef struct {
+    cpy_PyObject *self;
+    cpy_PyObject *arg;
+    cpy_PyObject * result;
+} _HPyFunc_args_O;
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_O(SYM, IMPL) \
+    static cpy_PyObject *SYM(cpy_PyObject *self, cpy_PyObject *arg) \
+    { \
+        _HPyFunc_args_O a = { self, arg }; \
+        _HPy_CallRealFunctionFromTrampoline( \
+           _ctx_for_trampolines, HPyFunc_O, (HPyCFunction)IMPL, &a); \
+        return a.result; \
+    }
+
+typedef struct {
     cpy_PyObject *arg0;
     cpy_PyObject * result;
 } _HPyFunc_args_UNARYFUNC;
 
 #define _HPyFunc_TRAMPOLINE_HPyFunc_UNARYFUNC(SYM, IMPL) \
     static cpy_PyObject *SYM(cpy_PyObject *arg0) \
     { \
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/universal/autogen_trampolines.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/autogen_trampolines.h`

 * *Files 12% similar despite different names*

```diff
@@ -6,72 +6,68 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
-HPyAPI_FUNC HPy HPyModule_Create(HPyContext *ctx, HPyModuleDef *def) {
-     return ctx->ctx_Module_Create ( ctx, def ); 
-}
-
 HPyAPI_FUNC HPy HPy_Dup(HPyContext *ctx, HPy h) {
      return ctx->ctx_Dup ( ctx, h ); 
 }
 
 HPyAPI_FUNC void HPy_Close(HPyContext *ctx, HPy h) {
      ctx->ctx_Close ( ctx, h ); 
 }
 
-HPyAPI_FUNC HPy HPyLong_FromLong(HPyContext *ctx, long value) {
-     return ctx->ctx_Long_FromLong ( ctx, value ); 
+HPyAPI_FUNC HPy HPyLong_FromInt32_t(HPyContext *ctx, int32_t value) {
+     return ctx->ctx_Long_FromInt32_t ( ctx, value ); 
 }
 
-HPyAPI_FUNC HPy HPyLong_FromUnsignedLong(HPyContext *ctx, unsigned long value) {
-     return ctx->ctx_Long_FromUnsignedLong ( ctx, value ); 
+HPyAPI_FUNC HPy HPyLong_FromUInt32_t(HPyContext *ctx, uint32_t value) {
+     return ctx->ctx_Long_FromUInt32_t ( ctx, value ); 
 }
 
-HPyAPI_FUNC HPy HPyLong_FromLongLong(HPyContext *ctx, long long v) {
-     return ctx->ctx_Long_FromLongLong ( ctx, v ); 
+HPyAPI_FUNC HPy HPyLong_FromInt64_t(HPyContext *ctx, int64_t v) {
+     return ctx->ctx_Long_FromInt64_t ( ctx, v ); 
 }
 
-HPyAPI_FUNC HPy HPyLong_FromUnsignedLongLong(HPyContext *ctx, unsigned long long v) {
-     return ctx->ctx_Long_FromUnsignedLongLong ( ctx, v ); 
+HPyAPI_FUNC HPy HPyLong_FromUInt64_t(HPyContext *ctx, uint64_t v) {
+     return ctx->ctx_Long_FromUInt64_t ( ctx, v ); 
 }
 
 HPyAPI_FUNC HPy HPyLong_FromSize_t(HPyContext *ctx, size_t value) {
      return ctx->ctx_Long_FromSize_t ( ctx, value ); 
 }
 
 HPyAPI_FUNC HPy HPyLong_FromSsize_t(HPyContext *ctx, HPy_ssize_t value) {
      return ctx->ctx_Long_FromSsize_t ( ctx, value ); 
 }
 
-HPyAPI_FUNC long HPyLong_AsLong(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsLong ( ctx, h ); 
+HPyAPI_FUNC int32_t HPyLong_AsInt32_t(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsInt32_t ( ctx, h ); 
 }
 
-HPyAPI_FUNC unsigned long HPyLong_AsUnsignedLong(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsUnsignedLong ( ctx, h ); 
+HPyAPI_FUNC uint32_t HPyLong_AsUInt32_t(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsUInt32_t ( ctx, h ); 
 }
 
-HPyAPI_FUNC unsigned long HPyLong_AsUnsignedLongMask(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsUnsignedLongMask ( ctx, h ); 
+HPyAPI_FUNC uint32_t HPyLong_AsUInt32_tMask(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsUInt32_tMask ( ctx, h ); 
 }
 
-HPyAPI_FUNC long long HPyLong_AsLongLong(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsLongLong ( ctx, h ); 
+HPyAPI_FUNC int64_t HPyLong_AsInt64_t(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsInt64_t ( ctx, h ); 
 }
 
-HPyAPI_FUNC unsigned long long HPyLong_AsUnsignedLongLong(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsUnsignedLongLong ( ctx, h ); 
+HPyAPI_FUNC uint64_t HPyLong_AsUInt64_t(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsUInt64_t ( ctx, h ); 
 }
 
-HPyAPI_FUNC unsigned long long HPyLong_AsUnsignedLongLongMask(HPyContext *ctx, HPy h) {
-     return ctx->ctx_Long_AsUnsignedLongLongMask ( ctx, h ); 
+HPyAPI_FUNC uint64_t HPyLong_AsUInt64_tMask(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Long_AsUInt64_tMask ( ctx, h ); 
 }
 
 HPyAPI_FUNC size_t HPyLong_AsSize_t(HPyContext *ctx, HPy h) {
      return ctx->ctx_Long_AsSize_t ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy_ssize_t HPyLong_AsSsize_t(HPyContext *ctx, HPy h) {
@@ -90,16 +86,16 @@
      return ctx->ctx_Float_FromDouble ( ctx, v ); 
 }
 
 HPyAPI_FUNC double HPyFloat_AsDouble(HPyContext *ctx, HPy h) {
      return ctx->ctx_Float_AsDouble ( ctx, h ); 
 }
 
-HPyAPI_FUNC HPy HPyBool_FromLong(HPyContext *ctx, long v) {
-     return ctx->ctx_Bool_FromLong ( ctx, v ); 
+HPyAPI_FUNC HPy HPyBool_FromBool(HPyContext *ctx, bool v) {
+     return ctx->ctx_Bool_FromBool ( ctx, v ); 
 }
 
 HPyAPI_FUNC HPy_ssize_t HPy_Length(HPyContext *ctx, HPy h) {
      return ctx->ctx_Length ( ctx, h ); 
 }
 
 HPyAPI_FUNC int HPyNumber_Check(HPyContext *ctx, HPy h) {
@@ -246,16 +242,24 @@
      return ctx->ctx_Callable_Check ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy HPy_CallTupleDict(HPyContext *ctx, HPy callable, HPy args, HPy kw) {
      return ctx->ctx_CallTupleDict ( ctx, callable, args, kw ); 
 }
 
-HPyAPI_FUNC HPy HPyErr_SetString(HPyContext *ctx, HPy h_type, const char *message) {
-     ctx->ctx_Err_SetString ( ctx, h_type, message ); return HPy_NULL; 
+HPyAPI_FUNC HPy HPy_Call(HPyContext *ctx, HPy callable, const HPy *args, size_t nargs, HPy kwnames) {
+     return ctx->ctx_Call ( ctx, callable, args, nargs, kwnames ); 
+}
+
+HPyAPI_FUNC HPy HPy_CallMethod(HPyContext *ctx, HPy name, const HPy *args, size_t nargs, HPy kwnames) {
+     return ctx->ctx_CallMethod ( ctx, name, args, nargs, kwnames ); 
+}
+
+HPyAPI_FUNC HPy HPyErr_SetString(HPyContext *ctx, HPy h_type, const char *utf8_message) {
+     ctx->ctx_Err_SetString ( ctx, h_type, utf8_message ); return HPy_NULL; 
 }
 
 HPyAPI_FUNC HPy HPyErr_SetObject(HPyContext *ctx, HPy h_type, HPy h_value) {
      ctx->ctx_Err_SetObject ( ctx, h_type, h_value ); return HPy_NULL; 
 }
 
 HPyAPI_FUNC HPy HPyErr_SetFromErrnoWithFilename(HPyContext *ctx, HPy h_type, const char *filename_fsencoded) {
@@ -278,112 +282,160 @@
      ctx->ctx_Err_NoMemory ( ctx ); return HPy_NULL; 
 }
 
 HPyAPI_FUNC void HPyErr_Clear(HPyContext *ctx) {
      ctx->ctx_Err_Clear ( ctx ); 
 }
 
-HPyAPI_FUNC HPy HPyErr_NewException(HPyContext *ctx, const char *name, HPy base, HPy dict) {
-     return ctx->ctx_Err_NewException ( ctx, name, base, dict ); 
+HPyAPI_FUNC HPy HPyErr_NewException(HPyContext *ctx, const char *utf8_name, HPy base, HPy dict) {
+     return ctx->ctx_Err_NewException ( ctx, utf8_name, base, dict ); 
 }
 
-HPyAPI_FUNC HPy HPyErr_NewExceptionWithDoc(HPyContext *ctx, const char *name, const char *doc, HPy base, HPy dict) {
-     return ctx->ctx_Err_NewExceptionWithDoc ( ctx, name, doc, base, dict ); 
+HPyAPI_FUNC HPy HPyErr_NewExceptionWithDoc(HPyContext *ctx, const char *utf8_name, const char *utf8_doc, HPy base, HPy dict) {
+     return ctx->ctx_Err_NewExceptionWithDoc ( ctx, utf8_name, utf8_doc, base, dict ); 
 }
 
-HPyAPI_FUNC int HPyErr_WarnEx(HPyContext *ctx, HPy category, const char *message, HPy_ssize_t stack_level) {
-     return ctx->ctx_Err_WarnEx ( ctx, category, message, stack_level ); 
+HPyAPI_FUNC int HPyErr_WarnEx(HPyContext *ctx, HPy category, const char *utf8_message, HPy_ssize_t stack_level) {
+     return ctx->ctx_Err_WarnEx ( ctx, category, utf8_message, stack_level ); 
 }
 
 HPyAPI_FUNC void HPyErr_WriteUnraisable(HPyContext *ctx, HPy obj) {
      ctx->ctx_Err_WriteUnraisable ( ctx, obj ); 
 }
 
 HPyAPI_FUNC int HPy_IsTrue(HPyContext *ctx, HPy h) {
      return ctx->ctx_IsTrue ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy HPyType_FromSpec(HPyContext *ctx, HPyType_Spec *spec, HPyType_SpecParam *params) {
      return ctx->ctx_Type_FromSpec ( ctx, spec, params ); 
 }
 
-HPyAPI_FUNC HPy HPyType_GenericNew(HPyContext *ctx, HPy type, HPy *args, HPy_ssize_t nargs, HPy kw) {
+HPyAPI_FUNC HPy HPyType_GenericNew(HPyContext *ctx, HPy type, const HPy *args, HPy_ssize_t nargs, HPy kw) {
      return ctx->ctx_Type_GenericNew ( ctx, type, args, nargs, kw ); 
 }
 
 HPyAPI_FUNC HPy HPy_GetAttr(HPyContext *ctx, HPy obj, HPy name) {
      return ctx->ctx_GetAttr ( ctx, obj, name ); 
 }
 
-HPyAPI_FUNC HPy HPy_GetAttr_s(HPyContext *ctx, HPy obj, const char *name) {
-     return ctx->ctx_GetAttr_s ( ctx, obj, name ); 
+HPyAPI_FUNC HPy HPy_GetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name) {
+     return ctx->ctx_GetAttr_s ( ctx, obj, utf8_name ); 
 }
 
 HPyAPI_FUNC int HPy_HasAttr(HPyContext *ctx, HPy obj, HPy name) {
      return ctx->ctx_HasAttr ( ctx, obj, name ); 
 }
 
-HPyAPI_FUNC int HPy_HasAttr_s(HPyContext *ctx, HPy obj, const char *name) {
-     return ctx->ctx_HasAttr_s ( ctx, obj, name ); 
+HPyAPI_FUNC int HPy_HasAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name) {
+     return ctx->ctx_HasAttr_s ( ctx, obj, utf8_name ); 
 }
 
 HPyAPI_FUNC int HPy_SetAttr(HPyContext *ctx, HPy obj, HPy name, HPy value) {
      return ctx->ctx_SetAttr ( ctx, obj, name, value ); 
 }
 
-HPyAPI_FUNC int HPy_SetAttr_s(HPyContext *ctx, HPy obj, const char *name, HPy value) {
-     return ctx->ctx_SetAttr_s ( ctx, obj, name, value ); 
+HPyAPI_FUNC int HPy_SetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name, HPy value) {
+     return ctx->ctx_SetAttr_s ( ctx, obj, utf8_name, value ); 
 }
 
 HPyAPI_FUNC HPy HPy_GetItem(HPyContext *ctx, HPy obj, HPy key) {
      return ctx->ctx_GetItem ( ctx, obj, key ); 
 }
 
 HPyAPI_FUNC HPy HPy_GetItem_i(HPyContext *ctx, HPy obj, HPy_ssize_t idx) {
      return ctx->ctx_GetItem_i ( ctx, obj, idx ); 
 }
 
-HPyAPI_FUNC HPy HPy_GetItem_s(HPyContext *ctx, HPy obj, const char *key) {
-     return ctx->ctx_GetItem_s ( ctx, obj, key ); 
+HPyAPI_FUNC HPy HPy_GetItem_s(HPyContext *ctx, HPy obj, const char *utf8_key) {
+     return ctx->ctx_GetItem_s ( ctx, obj, utf8_key ); 
 }
 
 HPyAPI_FUNC int HPy_Contains(HPyContext *ctx, HPy container, HPy key) {
      return ctx->ctx_Contains ( ctx, container, key ); 
 }
 
 HPyAPI_FUNC int HPy_SetItem(HPyContext *ctx, HPy obj, HPy key, HPy value) {
      return ctx->ctx_SetItem ( ctx, obj, key, value ); 
 }
 
 HPyAPI_FUNC int HPy_SetItem_i(HPyContext *ctx, HPy obj, HPy_ssize_t idx, HPy value) {
      return ctx->ctx_SetItem_i ( ctx, obj, idx, value ); 
 }
 
-HPyAPI_FUNC int HPy_SetItem_s(HPyContext *ctx, HPy obj, const char *key, HPy value) {
-     return ctx->ctx_SetItem_s ( ctx, obj, key, value ); 
+HPyAPI_FUNC int HPy_SetItem_s(HPyContext *ctx, HPy obj, const char *utf8_key, HPy value) {
+     return ctx->ctx_SetItem_s ( ctx, obj, utf8_key, value ); 
+}
+
+HPyAPI_FUNC int HPy_DelItem(HPyContext *ctx, HPy obj, HPy key) {
+     return ctx->ctx_DelItem ( ctx, obj, key ); 
+}
+
+HPyAPI_FUNC int HPy_DelItem_i(HPyContext *ctx, HPy obj, HPy_ssize_t idx) {
+     return ctx->ctx_DelItem_i ( ctx, obj, idx ); 
+}
+
+HPyAPI_FUNC int HPy_DelItem_s(HPyContext *ctx, HPy obj, const char *utf8_key) {
+     return ctx->ctx_DelItem_s ( ctx, obj, utf8_key ); 
 }
 
 HPyAPI_FUNC HPy HPy_Type(HPyContext *ctx, HPy obj) {
      return ctx->ctx_Type ( ctx, obj ); 
 }
 
 HPyAPI_FUNC int HPy_TypeCheck(HPyContext *ctx, HPy obj, HPy type) {
      return ctx->ctx_TypeCheck ( ctx, obj, type ); 
 }
 
+HPyAPI_FUNC const char *HPyType_GetName(HPyContext *ctx, HPy type) {
+     return ctx->ctx_Type_GetName ( ctx, type ); 
+}
+
+HPyAPI_FUNC int HPyType_IsSubtype(HPyContext *ctx, HPy sub, HPy type) {
+     return ctx->ctx_Type_IsSubtype ( ctx, sub, type ); 
+}
+
 HPyAPI_FUNC int HPy_Is(HPyContext *ctx, HPy obj, HPy other) {
      return ctx->ctx_Is ( ctx, obj, other ); 
 }
 
-HPyAPI_FUNC void *HPy_AsStruct(HPyContext *ctx, HPy h) {
-     return ctx->ctx_AsStruct ( ctx, h ); 
+HPyAPI_FUNC void *_HPy_AsStruct_Object(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Object ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Legacy(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Legacy ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Type(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Type ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Long(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Long ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Float(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Float ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Unicode(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Unicode ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_Tuple(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_Tuple ( ctx, h ); 
+}
+
+HPyAPI_FUNC void *_HPy_AsStruct_List(HPyContext *ctx, HPy h) {
+     return ctx->ctx_AsStruct_List ( ctx, h ); 
 }
 
-HPyAPI_FUNC void *HPy_AsStructLegacy(HPyContext *ctx, HPy h) {
-     return ctx->ctx_AsStructLegacy ( ctx, h ); 
+HPyAPI_FUNC HPyType_BuiltinShape _HPyType_GetBuiltinShape(HPyContext *ctx, HPy h_type) {
+     return ctx->ctx_Type_GetBuiltinShape ( ctx, h_type ); 
 }
 
 HPyAPI_FUNC HPy HPy_Repr(HPyContext *ctx, HPy obj) {
      return ctx->ctx_Repr ( ctx, obj ); 
 }
 
 HPyAPI_FUNC HPy HPy_Str(HPyContext *ctx, HPy obj) {
@@ -418,28 +470,28 @@
      return ctx->ctx_Bytes_Size ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy_ssize_t HPyBytes_GET_SIZE(HPyContext *ctx, HPy h) {
      return ctx->ctx_Bytes_GET_SIZE ( ctx, h ); 
 }
 
-HPyAPI_FUNC char *HPyBytes_AsString(HPyContext *ctx, HPy h) {
+HPyAPI_FUNC const char *HPyBytes_AsString(HPyContext *ctx, HPy h) {
      return ctx->ctx_Bytes_AsString ( ctx, h ); 
 }
 
-HPyAPI_FUNC char *HPyBytes_AS_STRING(HPyContext *ctx, HPy h) {
+HPyAPI_FUNC const char *HPyBytes_AS_STRING(HPyContext *ctx, HPy h) {
      return ctx->ctx_Bytes_AS_STRING ( ctx, h ); 
 }
 
-HPyAPI_FUNC HPy HPyBytes_FromString(HPyContext *ctx, const char *v) {
-     return ctx->ctx_Bytes_FromString ( ctx, v ); 
+HPyAPI_FUNC HPy HPyBytes_FromString(HPyContext *ctx, const char *bytes) {
+     return ctx->ctx_Bytes_FromString ( ctx, bytes ); 
 }
 
-HPyAPI_FUNC HPy HPyBytes_FromStringAndSize(HPyContext *ctx, const char *v, HPy_ssize_t len) {
-     return ctx->ctx_Bytes_FromStringAndSize ( ctx, v, len ); 
+HPyAPI_FUNC HPy HPyBytes_FromStringAndSize(HPyContext *ctx, const char *bytes, HPy_ssize_t len) {
+     return ctx->ctx_Bytes_FromStringAndSize ( ctx, bytes, len ); 
 }
 
 HPyAPI_FUNC HPy HPyUnicode_FromString(HPyContext *ctx, const char *utf8) {
      return ctx->ctx_Unicode_FromString ( ctx, utf8 ); 
 }
 
 HPyAPI_FUNC int HPyUnicode_Check(HPyContext *ctx, HPy h) {
@@ -478,20 +530,28 @@
      return ctx->ctx_Unicode_EncodeFSDefault ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy_UCS4 HPyUnicode_ReadChar(HPyContext *ctx, HPy h, HPy_ssize_t index) {
      return ctx->ctx_Unicode_ReadChar ( ctx, h, index ); 
 }
 
-HPyAPI_FUNC HPy HPyUnicode_DecodeASCII(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors) {
-     return ctx->ctx_Unicode_DecodeASCII ( ctx, s, size, errors ); 
+HPyAPI_FUNC HPy HPyUnicode_DecodeASCII(HPyContext *ctx, const char *ascii, HPy_ssize_t size, const char *errors) {
+     return ctx->ctx_Unicode_DecodeASCII ( ctx, ascii, size, errors ); 
 }
 
-HPyAPI_FUNC HPy HPyUnicode_DecodeLatin1(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors) {
-     return ctx->ctx_Unicode_DecodeLatin1 ( ctx, s, size, errors ); 
+HPyAPI_FUNC HPy HPyUnicode_DecodeLatin1(HPyContext *ctx, const char *latin1, HPy_ssize_t size, const char *errors) {
+     return ctx->ctx_Unicode_DecodeLatin1 ( ctx, latin1, size, errors ); 
+}
+
+HPyAPI_FUNC HPy HPyUnicode_FromEncodedObject(HPyContext *ctx, HPy obj, const char *encoding, const char *errors) {
+     return ctx->ctx_Unicode_FromEncodedObject ( ctx, obj, encoding, errors ); 
+}
+
+HPyAPI_FUNC HPy HPyUnicode_Substring(HPyContext *ctx, HPy str, HPy_ssize_t start, HPy_ssize_t end) {
+     return ctx->ctx_Unicode_Substring ( ctx, str, start, end ); 
 }
 
 HPyAPI_FUNC int HPyList_Check(HPyContext *ctx, HPy h) {
      return ctx->ctx_List_Check ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy HPyList_New(HPyContext *ctx, HPy_ssize_t len) {
@@ -506,56 +566,84 @@
      return ctx->ctx_Dict_Check ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy HPyDict_New(HPyContext *ctx) {
      return ctx->ctx_Dict_New ( ctx ); 
 }
 
+HPyAPI_FUNC HPy HPyDict_Keys(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Dict_Keys ( ctx, h ); 
+}
+
+HPyAPI_FUNC HPy HPyDict_Copy(HPyContext *ctx, HPy h) {
+     return ctx->ctx_Dict_Copy ( ctx, h ); 
+}
+
 HPyAPI_FUNC int HPyTuple_Check(HPyContext *ctx, HPy h) {
      return ctx->ctx_Tuple_Check ( ctx, h ); 
 }
 
 HPyAPI_FUNC HPy HPyTuple_FromArray(HPyContext *ctx, HPy items[], HPy_ssize_t n) {
      return ctx->ctx_Tuple_FromArray ( ctx, items, n ); 
 }
 
-HPyAPI_FUNC HPy HPyImport_ImportModule(HPyContext *ctx, const char *name) {
-     return ctx->ctx_Import_ImportModule ( ctx, name ); 
+HPyAPI_FUNC int HPySlice_Unpack(HPyContext *ctx, HPy slice, HPy_ssize_t *start, HPy_ssize_t *stop, HPy_ssize_t *step) {
+     return ctx->ctx_Slice_Unpack ( ctx, slice, start, stop, step ); 
+}
+
+HPyAPI_FUNC HPy HPyImport_ImportModule(HPyContext *ctx, const char *utf8_name) {
+     return ctx->ctx_Import_ImportModule ( ctx, utf8_name ); 
+}
+
+HPyAPI_FUNC HPy HPyCapsule_New(HPyContext *ctx, void *pointer, const char *utf8_name, HPyCapsule_Destructor *destructor) {
+     return ctx->ctx_Capsule_New ( ctx, pointer, utf8_name, destructor ); 
+}
+
+HPyAPI_FUNC void *HPyCapsule_Get(HPyContext *ctx, HPy capsule, _HPyCapsule_key key, const char *utf8_name) {
+     return ctx->ctx_Capsule_Get ( ctx, capsule, key, utf8_name ); 
+}
+
+HPyAPI_FUNC int HPyCapsule_IsValid(HPyContext *ctx, HPy capsule, const char *utf8_name) {
+     return ctx->ctx_Capsule_IsValid ( ctx, capsule, utf8_name ); 
+}
+
+HPyAPI_FUNC int HPyCapsule_Set(HPyContext *ctx, HPy capsule, _HPyCapsule_key key, void *value) {
+     return ctx->ctx_Capsule_Set ( ctx, capsule, key, value ); 
 }
 
 HPyAPI_FUNC HPy HPy_FromPyObject(HPyContext *ctx, cpy_PyObject *obj) {
      return ctx->ctx_FromPyObject ( ctx, obj ); 
 }
 
 HPyAPI_FUNC cpy_PyObject *HPy_AsPyObject(HPyContext *ctx, HPy h) {
      return ctx->ctx_AsPyObject ( ctx, h ); 
 }
 
 HPyAPI_FUNC void _HPy_CallRealFunctionFromTrampoline(HPyContext *ctx, HPyFunc_Signature sig, HPyCFunction func, void *args) {
      ctx->ctx_CallRealFunctionFromTrampoline ( ctx, sig, func, args ); 
 }
 
-HPyAPI_FUNC HPyListBuilder HPyListBuilder_New(HPyContext *ctx, HPy_ssize_t initial_size) {
-     return ctx->ctx_ListBuilder_New ( ctx, initial_size ); 
+HPyAPI_FUNC HPyListBuilder HPyListBuilder_New(HPyContext *ctx, HPy_ssize_t size) {
+     return ctx->ctx_ListBuilder_New ( ctx, size ); 
 }
 
 HPyAPI_FUNC void HPyListBuilder_Set(HPyContext *ctx, HPyListBuilder builder, HPy_ssize_t index, HPy h_item) {
      ctx->ctx_ListBuilder_Set ( ctx, builder, index, h_item ); 
 }
 
 HPyAPI_FUNC HPy HPyListBuilder_Build(HPyContext *ctx, HPyListBuilder builder) {
      return ctx->ctx_ListBuilder_Build ( ctx, builder ); 
 }
 
 HPyAPI_FUNC void HPyListBuilder_Cancel(HPyContext *ctx, HPyListBuilder builder) {
      ctx->ctx_ListBuilder_Cancel ( ctx, builder ); 
 }
 
-HPyAPI_FUNC HPyTupleBuilder HPyTupleBuilder_New(HPyContext *ctx, HPy_ssize_t initial_size) {
-     return ctx->ctx_TupleBuilder_New ( ctx, initial_size ); 
+HPyAPI_FUNC HPyTupleBuilder HPyTupleBuilder_New(HPyContext *ctx, HPy_ssize_t size) {
+     return ctx->ctx_TupleBuilder_New ( ctx, size ); 
 }
 
 HPyAPI_FUNC void HPyTupleBuilder_Set(HPyContext *ctx, HPyTupleBuilder builder, HPy_ssize_t index, HPy h_item) {
      ctx->ctx_TupleBuilder_Set ( ctx, builder, index, h_item ); 
 }
 
 HPyAPI_FUNC HPy HPyTupleBuilder_Build(HPyContext *ctx, HPyTupleBuilder builder) {
@@ -606,7 +694,31 @@
      return ctx->ctx_Global_Load ( ctx, global ); 
 }
 
 HPyAPI_FUNC void _HPy_Dump(HPyContext *ctx, HPy h) {
      ctx->ctx_Dump ( ctx, h ); 
 }
 
+HPyAPI_FUNC HPy HPy_Compile_s(HPyContext *ctx, const char *utf8_source, const char *utf8_filename, HPy_SourceKind kind) {
+     return ctx->ctx_Compile_s ( ctx, utf8_source, utf8_filename, kind ); 
+}
+
+HPyAPI_FUNC HPy HPy_EvalCode(HPyContext *ctx, HPy code, HPy globals, HPy locals) {
+     return ctx->ctx_EvalCode ( ctx, code, globals, locals ); 
+}
+
+HPyAPI_FUNC HPy HPyContextVar_New(HPyContext *ctx, const char *name, HPy default_value) {
+     return ctx->ctx_ContextVar_New ( ctx, name, default_value ); 
+}
+
+HPyAPI_FUNC int32_t HPyContextVar_Get(HPyContext *ctx, HPy context_var, HPy default_value, HPy *result) {
+     return ctx->ctx_ContextVar_Get ( ctx, context_var, default_value, result ); 
+}
+
+HPyAPI_FUNC HPy HPyContextVar_Set(HPyContext *ctx, HPy context_var, HPy value) {
+     return ctx->ctx_ContextVar_Set ( ctx, context_var, value ); 
+}
+
+HPyAPI_FUNC int HPy_SetCallFunction(HPyContext *ctx, HPy h, HPyCallFunction *func) {
+     return ctx->ctx_SetCallFunction ( ctx, h, func ); 
+}
+
```

### Comparing `hpy-0.0.4/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h` & `hpy-0.9.0rc1/hpy/devel/include/hpy/universal/hpyfunc_trampolines.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,165 +1,177 @@
 #ifndef HPY_UNIVERSAL_HPYFUNC_TRAMPOLINES_H
 #define HPY_UNIVERSAL_HPYFUNC_TRAMPOLINES_H
 
 /* This file should be autogenerated */
 
 typedef struct {
     cpy_PyObject *self;
+    cpy_PyObject *const *args;
+    HPy_ssize_t nargs;
     cpy_PyObject *result;
-} _HPyFunc_args_NOARGS;
-
-typedef struct {
-    cpy_PyObject *self;
-    cpy_PyObject *arg;
-    cpy_PyObject *result;
-} _HPyFunc_args_O;
+} _HPyFunc_args_VARARGS;
 
 typedef struct {
     cpy_PyObject *self;
-    cpy_PyObject *args;
+    cpy_PyObject *const *args;
+    /* We also use HPyFunc_KEYWORDS for HPy_tp_call which will be called as
+       vectorcall function from CPython. Therefore, 'nargsf' may also have bit
+       'PY_VECTORCALL_ARGUMENTS_OFFSET' set. */
+    size_t nargsf;
+    cpy_PyObject *kwnames;
     cpy_PyObject *result;
-} _HPyFunc_args_VARARGS;
+} _HPyFunc_args_KEYWORDS;
 
 typedef struct {
     cpy_PyObject *self;
     cpy_PyObject *args;
     cpy_PyObject *kw;
-    cpy_PyObject *result;
-} _HPyFunc_args_KEYWORDS;
+    int result;
+} _HPyFunc_args_INITPROC;
 
 typedef struct {
     cpy_PyObject *self;
     cpy_PyObject *args;
     cpy_PyObject *kw;
-    int result;
-} _HPyFunc_args_INITPROC;
+    cpy_PyObject *result;
+} _HPyFunc_args_NEWFUNC;
 
 typedef struct {
     cpy_PyObject *arg0;
     cpy_PyObject *arg1;
     HPy_RichCmpOp arg2;
     cpy_PyObject * result;
 } _HPyFunc_args_RICHCMPFUNC;
 
-
-#define _HPyFunc_TRAMPOLINE_HPyFunc_NOARGS(SYM, IMPL)                   \
-    static cpy_PyObject *                                               \
-    SYM(cpy_PyObject *self, cpy_PyObject *noargs)                       \
-    {                                                                   \
-        _HPyFunc_args_NOARGS a = { self };                              \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-            _ctx_for_trampolines, HPyFunc_NOARGS, (HPyCFunction)IMPL, &a);            \
-        return a.result;                                                \
-    }
-
-#define _HPyFunc_TRAMPOLINE_HPyFunc_O(SYM, IMPL)                        \
-    static cpy_PyObject *                                               \
-    SYM(cpy_PyObject *self, cpy_PyObject *arg)                          \
-    {                                                                   \
-        _HPyFunc_args_O a = { self, arg };                              \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-            _ctx_for_trampolines, HPyFunc_O, (HPyCFunction)IMPL, &a);                 \
-        return a.result;                                                \
-    }
-
-
-#define _HPyFunc_TRAMPOLINE_HPyFunc_VARARGS(SYM, IMPL)                  \
-    static cpy_PyObject *                                               \
-    SYM(cpy_PyObject *self, cpy_PyObject *args)                         \
-    {                                                                   \
-        _HPyFunc_args_VARARGS a = { self, args };                       \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-            _ctx_for_trampolines, HPyFunc_VARARGS, (HPyCFunction)IMPL, &a);           \
-        return a.result;                                                \
-    }
-
-
-#define _HPyFunc_TRAMPOLINE_HPyFunc_KEYWORDS(SYM, IMPL)                 \
-    static cpy_PyObject *                                               \
-    SYM(cpy_PyObject *self, cpy_PyObject *args, cpy_PyObject *kw)       \
-    {                                                                   \
-        _HPyFunc_args_KEYWORDS a = { self, args, kw };                  \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-            _ctx_for_trampolines, HPyFunc_KEYWORDS, (HPyCFunction)IMPL, &a);          \
-        return a.result;                                                \
-    }
-
-#define _HPyFunc_TRAMPOLINE_HPyFunc_INITPROC(SYM, IMPL)                 \
-    static int                                                          \
-    SYM(cpy_PyObject *self, cpy_PyObject *args, cpy_PyObject *kw)       \
-    {                                                                   \
-        _HPyFunc_args_INITPROC a = { self, args, kw };                  \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-            _ctx_for_trampolines, HPyFunc_INITPROC, (HPyCFunction)IMPL, &a);          \
-        return a.result;                                                \
+#define _HPyFunc_TRAMPOLINE_HPyFunc_VARARGS(SYM, IMPL)                      \
+    static cpy_PyObject *                                                   \
+    SYM(cpy_PyObject *self, cpy_PyObject *const *args, HPy_ssize_t nargs)   \
+    {                                                                       \
+        _HPyFunc_args_VARARGS a = { self, args, nargs };                    \
+        _HPy_CallRealFunctionFromTrampoline(                                \
+            _ctx_for_trampolines, HPyFunc_VARARGS, (HPyCFunction)IMPL, &a); \
+        return a.result;                                                    \
+    }
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_KEYWORDS(SYM, IMPL)                      \
+    static cpy_PyObject *                                                    \
+    SYM(cpy_PyObject *self, cpy_PyObject *const *args, size_t nargs,         \
+            cpy_PyObject *kwnames)                                           \
+    {                                                                        \
+        _HPyFunc_args_KEYWORDS a = { self, args, nargs, kwnames };           \
+        _HPy_CallRealFunctionFromTrampoline(                                 \
+            _ctx_for_trampolines, HPyFunc_KEYWORDS, (HPyCFunction)IMPL, &a); \
+        return a.result;                                                     \
+    }
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_INITPROC(SYM, IMPL)                      \
+    static int                                                               \
+    SYM(cpy_PyObject *self, cpy_PyObject *args, cpy_PyObject *kw)            \
+    {                                                                        \
+        _HPyFunc_args_INITPROC a = { self, args, kw };                       \
+        _HPy_CallRealFunctionFromTrampoline(                                 \
+            _ctx_for_trampolines, HPyFunc_INITPROC, (HPyCFunction)IMPL, &a); \
+        return a.result;                                                     \
+    }
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_NEWFUNC(SYM, IMPL)                       \
+    static cpy_PyObject *                                                    \
+    SYM(cpy_PyObject *self, cpy_PyObject *args, cpy_PyObject *kw)            \
+    {                                                                        \
+        _HPyFunc_args_NEWFUNC a = { self, args, kw };                        \
+        _HPy_CallRealFunctionFromTrampoline(                                 \
+            _ctx_for_trampolines, HPyFunc_NEWFUNC, (HPyCFunction)IMPL, &a);  \
+        return a.result;                                                     \
     }
 
 /* special case: the HPy_tp_destroy slot doesn't map to any CPython slot.
    Instead, it is called from our own tp_dealloc: see also
    hpytype_dealloc(). */
-#define _HPyFunc_TRAMPOLINE_HPyFunc_DESTROYFUNC(SYM, IMPL)              \
+#define _HPyFunc_TRAMPOLINE_HPyFunc_DESTROYFUNC(SYM, IMPL) \
     static void SYM(void) { abort(); }
 
 
 /* this needs to be written manually because HPy has a different type for
    "op": HPy_RichCmpOp instead of int */
-#define _HPyFunc_TRAMPOLINE_HPyFunc_RICHCMPFUNC(SYM, IMPL)              \
-    static cpy_PyObject *                                               \
-    SYM(cpy_PyObject *self, cpy_PyObject *obj, int op)                  \
-    {                                                                   \
-        _HPyFunc_args_RICHCMPFUNC a = { self, obj, (HPy_RichCmpOp)op };                \
-        _HPy_CallRealFunctionFromTrampoline(                            \
-           _ctx_for_trampolines, HPyFunc_RICHCMPFUNC, (HPyCFunction)IMPL, &a);        \
-        return a.result;                                                \
+#define _HPyFunc_TRAMPOLINE_HPyFunc_RICHCMPFUNC(SYM, IMPL)                     \
+    static cpy_PyObject *                                                      \
+    SYM(cpy_PyObject *self, cpy_PyObject *obj, int op)                         \
+    {                                                                          \
+        _HPyFunc_args_RICHCMPFUNC a = { self, obj, (HPy_RichCmpOp)op };        \
+        _HPy_CallRealFunctionFromTrampoline(                                   \
+           _ctx_for_trampolines, HPyFunc_RICHCMPFUNC, (HPyCFunction)IMPL, &a); \
+        return a.result;                                                       \
     }
 
 typedef struct {
     cpy_PyObject *self;
     cpy_Py_buffer *view;
     int flags;
     int result;
 } _HPyFunc_args_GETBUFFERPROC;
 
-#define _HPyFunc_TRAMPOLINE_HPyFunc_GETBUFFERPROC(SYM, IMPL) \
-    static int SYM(cpy_PyObject *self, cpy_Py_buffer *view, int flags) \
-    { \
-        _HPyFunc_args_GETBUFFERPROC a = {self, view, flags}; \
-        _HPy_CallRealFunctionFromTrampoline( \
+#define _HPyFunc_TRAMPOLINE_HPyFunc_GETBUFFERPROC(SYM, IMPL)                     \
+    static int SYM(cpy_PyObject *self, cpy_Py_buffer *view, int flags)           \
+    {                                                                            \
+        _HPyFunc_args_GETBUFFERPROC a = {self, view, flags};                     \
+        _HPy_CallRealFunctionFromTrampoline(                                     \
            _ctx_for_trampolines, HPyFunc_GETBUFFERPROC, (HPyCFunction)IMPL, &a); \
-        return a.result; \
+        return a.result;                                                         \
     }
 
 typedef struct {
     cpy_PyObject *self;
     cpy_Py_buffer *view;
 } _HPyFunc_args_RELEASEBUFFERPROC;
 
 #define _HPyFunc_TRAMPOLINE_HPyFunc_RELEASEBUFFERPROC(SYM, IMPL) \
-    static void SYM(cpy_PyObject *self, cpy_Py_buffer *view) \
-    { \
-        _HPyFunc_args_RELEASEBUFFERPROC a = {self, view}; \
-        _HPy_CallRealFunctionFromTrampoline( \
-           _ctx_for_trampolines, HPyFunc_RELEASEBUFFERPROC, (HPyCFunction)IMPL, &a); \
-        return; \
+    static void SYM(cpy_PyObject *self, cpy_Py_buffer *view)     \
+    {                                                            \
+        _HPyFunc_args_RELEASEBUFFERPROC a = {self, view};        \
+        _HPy_CallRealFunctionFromTrampoline(                     \
+           _ctx_for_trampolines, HPyFunc_RELEASEBUFFERPROC,      \
+           (HPyCFunction)IMPL, &a);                              \
+        return;                                                  \
     }
 
 
 typedef struct {
     cpy_PyObject *self;
     cpy_visitproc visit;
     void *arg;
     int result;
 } _HPyFunc_args_TRAVERSEPROC;
 
-#define _HPyFunc_TRAMPOLINE_HPyFunc_TRAVERSEPROC(SYM, IMPL) \
+#define _HPyFunc_TRAMPOLINE_HPyFunc_TRAVERSEPROC(SYM, IMPL)            \
     static int SYM(cpy_PyObject *self, cpy_visitproc visit, void *arg) \
-    { \
-        _HPyFunc_args_TRAVERSEPROC a = { self, visit, arg }; \
-        _HPy_CallRealFunctionFromTrampoline( \
-           _ctx_for_trampolines, HPyFunc_TRAVERSEPROC, (HPyCFunction)IMPL, &a); \
-        return a.result; \
+    {                                                                  \
+        _HPyFunc_args_TRAVERSEPROC a = { self, visit, arg };           \
+        _HPy_CallRealFunctionFromTrampoline(                           \
+           _ctx_for_trampolines, HPyFunc_TRAVERSEPROC,                 \
+           (HPyCFunction)IMPL, &a);                                    \
+        return a.result;                                               \
+    }
+
+#define HPyCapsule_DESTRUCTOR_TRAMPOLINE(SYM, IMPL)                       \
+    static void SYM(cpy_PyObject *capsule)                                \
+    {                                                                     \
+        _HPy_CallRealFunctionFromTrampoline(_ctx_for_trampolines,         \
+                HPyFunc_CAPSULE_DESTRUCTOR, (HPyCFunction)IMPL, capsule); \
     }
 
+typedef struct {
+    cpy_PyObject *spec;
+    cpy_PyObject *result;
+} _HPyFunc_args_MOD_CREATE;
+
+#define _HPyFunc_TRAMPOLINE_HPyFunc_MOD_CREATE(SYM, IMPL)                     \
+    static cpy_PyObject* SYM(cpy_PyObject *spec, cpy_PyModuleDef *def)        \
+    {                                                                         \
+        (void) def; /* avoid 'unused' warning */                              \
+        _HPyFunc_args_UNARYFUNC a = { spec };                                 \
+        _HPy_CallRealFunctionFromTrampoline(                                  \
+           _ctx_for_trampolines, HPyFunc_MOD_CREATE, (HPyCFunction)IMPL, &a); \
+        return a.result;                                                      \
+    }
 
 
 #endif // HPY_UNIVERSAL_HPYFUNC_TRAMPOLINES_H
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/argparse.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/argparse.c`

 * *Files 10% similar despite different names*

```diff
@@ -406,75 +406,75 @@
 /**
  * Parse positional arguments.
  *
  * :param ctx:
  *     The execution context.
  * :param ht:
  *     An optional pointer to an HPyTracker. If the format string never
- *     results in new handles being created, `ht` may be `NULL`. Currently
- *     no formatting options to this function require an HPyTracker.
+ *     results in new handles being created, ``ht`` may be ``NULL``. Currently
+ *     only the ``O`` formatting option to this function requires an HPyTracker.
  * :param args:
  *     The array of positional arguments to parse.
  * :param nargs:
- *     The number of elements in args.
+ *     The number of elements in ``args``.
  * :param fmt:
  *     The format string to use to parse the arguments.
  * :param ...:
  *     A va_list of references to variables in which to store the parsed
  *     arguments. The number and types of the arguments should match the
- *     the format strint, `fmt`.
+ *     the format string, ``fmt``.
  *
- * :returns: 0 on failure, 1 on success.
+ * :returns: ``0`` on failure, ``1`` on success.
  *
- * If a `NULL` pointer is passed to `ht` and an `HPyTracker` is required by
- * the format string, an exception will be raised.
+ * If a ``NULL`` pointer is passed to ``ht`` and an HPyTracker is required by
+ * the format string, a ``SystemError`` will be raised.
  *
- * If a pointer is provided to `ht`, the `HPyTracker` will always be created
- * and must be closed with `HPyTracker_Close` if parsing succeeds (after all
+ * If a pointer is provided to ``ht``, the HPyTracker will always be created
+ * and must be closed with ``HPyTracker_Close`` if parsing succeeds (after all
  * handles returned are no longer needed). If parsing fails, this function
- * will close the `HPyTracker` automatically.
+ * will close the HPyTracker automatically.
  *
  * Examples:
  *
- * Using `HPyArg_Parse` without an `HPyTracker`:
+ * Using ``HPyArg_Parse`` without an HPyTracker:
  *
  * .. code-block:: c
  *
  *     long a, b;
  *     if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
  *         return HPy_NULL;
  *     ...
  *
- * Using `HPyArg_Parse` with an `HPyTracker`:
+ * Using ``HPyArg_Parse`` with an HPyTracker:
  *
  * .. code-block:: c
  *
  *     long a, b;
  *     HPyTracker ht;
  *     if (!HPyArg_Parse(ctx, &ht, args, nargs, "ll", &a, &b))
  *         return HPy_NULL;
  *     ...
  *     HPyTracker_Close(ctx, ht);
  *     ...
  *
  * .. note::
  *
- *    Currently `HPyArg_Parse` never requires the use of an `HPyTracker`.
+ *    Currently ``HPyArg_Parse`` never requires the use of an HPyTracker.
  *    The option exists only to support releasing temporary storage used by
  *    future format string codes (e.g. for character strings).
  */
 HPyAPI_HELPER int
-HPyArg_Parse(HPyContext *ctx, HPyTracker *ht, HPy *args, HPy_ssize_t nargs, const char *fmt, ...)
+HPyArg_Parse(HPyContext *ctx, HPyTracker *ht, const HPy *args, size_t nargs, const char *fmt, ...)
 {
     const char *fmt1 = fmt;
     const char *err_fmt = NULL;
     const char *fmt_end = NULL;
 
     int optional = 0;
-    HPy_ssize_t i = 0;
+    size_t i = 0;
     HPy current_arg;
 
     fmt_end = parse_err_fmt(fmt, &err_fmt);
 
     if (ht != NULL) {
         *ht = HPyTracker_New(ctx, 0);
         if (HPy_IsNull(*ht)) {
@@ -512,104 +512,57 @@
             "mismatched args (too many arguments for fmt)");
         goto error;
     }
 
     va_end(vl);
     return 1;
 
-    error:
-        va_end(vl);
-        if (ht != NULL) {
-            HPyTracker_Close(ctx, *ht);
-        }
-        return 0;
+error:
+    va_end(vl);
+    if (ht != NULL) {
+        HPyTracker_Close(ctx, *ht);
+    }
+    return 0;
 }
 
+static HPy
+find_keyword(HPyContext *ctx, HPy kwnames, HPy_ssize_t n_kwnames, const HPy *args, const char *key)
+{
+    for (HPy_ssize_t i = 0; i < n_kwnames; i++) {
+        HPy kwname = HPy_GetItem_i(ctx, kwnames, i);
+        HPy h_key = HPyUnicode_FromString(ctx, key);
+        int eq = HPy_RichCompareBool(ctx, kwname, h_key, HPy_EQ);
+        HPy_Close(ctx, h_key);
+        HPy_Close(ctx, kwname);
+        if (eq) {
+            return args[i];
+        }
+    }
+    return HPy_NULL;
+}
 
-/**
- * Parse positional and keyword arguments.
- *
- * :param ctx:
- *     The execution context.
- * :param ht:
- *     An optional pointer to an HPyTracker. If the format string never
- *     results in new handles being created, `ht` may be `NULL`. Currently
- *     only the `O` formatting option to this function requires an HPyTracker.
- * :param args:
- *     The array of positional arguments to parse.
- * :param nargs:
- *     The number of elements in args.
- * :param kw:
- *     A handle to the dictionary of keyword arguments.
- * :param fmt:
- *     The format string to use to parse the arguments.
- * :param keywords:
- *     An `NULL` terminated array of argument names. The number of names
- *     should match the format string provided. Positional only arguments
- *     should have the name `""` (i.e. the null-terminated empty string).
- *     Positional only arguments must preceded all other arguments.
- * :param ...:
- *     A va_list of references to variables in which to store the parsed
- *     arguments. The number and types of the arguments should match the
- *     the format strint, `fmt`.
- *
- * :returns: 0 on failure, 1 on success.
- *
- * If a `NULL` pointer is passed to `ht` and an `HPyTracker` is required by
- * the format string, an exception will be raised.
- *
- * If a pointer is provided to `ht`, the `HPyTracker` will always be created
- * and must be closed with `HPyTracker_Close` if parsing succeeds (after all
- * handles returned are no longer needed). If parsing fails, this function
- * will close the `HPyTracker` automatically.
- *
- * Examples:
- *
- * Using `HPyArg_ParseKeywords` without an `HPyTracker`:
- *
- * .. code-block:: c
- *
- *     long a, b;
- *     if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kw, "ll", &a, &b))
- *         return HPy_NULL;
- *     ...
- *
- * Using `HPyArg_ParseKeywords` with an `HPyTracker`:
- *
- * .. code-block:: c
- *
- *     HPy a, b;
- *     HPyTracker ht;
- *     if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "OO", &a, &b))
- *         return HPy_NULL;
- *     ...
- *     HPyTracker_Close(ctx, ht);
- *     ...
- *
- * .. note::
- *
- *     Currently `HPyArg_ParseKeywords` only requires the use of an `HPyTracker`
- *     when the `O` format is used. In future other new format string codes
- *     (e.g. for character strings) may also require it.
- */
-HPyAPI_HELPER int
-HPyArg_ParseKeywords(HPyContext *ctx, HPyTracker *ht, HPy *args, HPy_ssize_t nargs, HPy kw,
-                     const char *fmt, const char *keywords[], ...)
+static int
+parse_keywords(HPyContext *ctx, HPyTracker *ht, const HPy *args,
+               size_t nargs, HPy kw, int kwnames, const char *fmt,
+               const char *keywords[], va_list *p_va)
 {
     const char *fmt1 = fmt;
     const char *err_fmt = NULL;
     const char *fmt_end = NULL;
 
     int optional = 0;
     int keyword_only = 0;
-    HPy_ssize_t i = 0;
-    HPy_ssize_t nkw = 0;
+    size_t i = 0;
+    size_t nkw = 0;
+    HPy_ssize_t n_kwnames = 0;
     HPy current_arg;
     int current_arg_needs_closing = 0;
 
+    assert(p_va != NULL);
+
     fmt_end = parse_err_fmt(fmt, &err_fmt);
 
     // first count positional only arguments
     while (keywords[nkw] != NULL && !*keywords[nkw]) {
         nkw++;
     }
     // then check and count the rest
@@ -625,16 +578,22 @@
     if (ht != NULL) {
         *ht = HPyTracker_New(ctx, 0);
         if (HPy_IsNull(*ht)) {
             return 0;
         }
     }
 
-    va_list vl;
-    va_start(vl, keywords);
+    if (kwnames && !HPy_IsNull(kw)) {
+        n_kwnames = HPy_Length(ctx, kw);
+        if (n_kwnames < 0) {
+            set_error(ctx, ctx->h_SystemError, err_fmt,
+                "could not retrieve length of keyword names tuple");
+            return 0;
+        }
+    }
 
     while (fmt1 != fmt_end) {
         if (*fmt1 == '|') {
             optional = 1;
             fmt1++;
             continue;
         }
@@ -661,28 +620,41 @@
                 set_error(ctx, ctx->h_TypeError, err_fmt,
                     "keyword only argument passed as positional argument");
                 goto error;
             }
             current_arg = args[i];
         }
         else if (!HPy_IsNull(kw) && *keywords[i]) {
-            current_arg = HPy_GetItem_s(ctx, kw, keywords[i]);
-            // Track the handle or lear any KeyError that was raised. If an
-            // error was raised current_arg will be HPy_NULL and will be
-            // handled appropriately below depending on whether the current
-            // argument is optional or not
-            if (!HPy_IsNull(current_arg)) {
-                current_arg_needs_closing = 1;
-            }
-            else {
-                HPyErr_Clear(ctx);
+            if (kwnames) {
+                current_arg = find_keyword(ctx, kw, n_kwnames, args+nargs,
+                                           keywords[i]);
+                /*
+                 * Clear any error that was raised. If an error was raised
+                 * current_arg will be HPy_NULL and will be handled
+                 * appropriately below depending on whether the current argument
+                 * is optional or not.
+                 */
+                if (HPy_IsNull(current_arg)) {
+                    HPyErr_Clear(ctx);
+                }
+            } else {
+                current_arg = HPy_GetItem_s(ctx, kw, keywords[i]);
+                /*
+                 * Track the handle or clear any KeyError that was raised (for
+                 * the same reason as explained above).
+                 */
+                if (!HPy_IsNull(current_arg)) {
+                    current_arg_needs_closing = 1;
+                } else {
+                    HPyErr_Clear(ctx);
+                }
             }
         }
         if (!HPy_IsNull(current_arg) || optional) {
-            if (!parse_item(ctx, ht, current_arg, 1, &fmt1, &vl, err_fmt)) {
+            if (!parse_item(ctx, ht, current_arg, 1, &fmt1, p_va, err_fmt)) {
                 goto error;
             }
         }
         else {
             set_error(ctx, ctx->h_TypeError, err_fmt,
                 "no value for required argument");
             goto error;
@@ -694,21 +666,154 @@
         i++;
     }
     if (i != nkw) {
         set_error(ctx, ctx->h_TypeError, err_fmt,
             "mismatched args (too many keywords for fmt)");
         goto error;
     }
-
-    va_end(vl);
     return 1;
 
-    error:
-        va_end(vl);
-        if (ht != NULL) {
-            HPyTracker_Close(ctx, *ht);
-        }
-        if (current_arg_needs_closing) {
-            HPy_Close(ctx, current_arg);
-        }
-        return 0;
+error:
+    if (ht != NULL) {
+        HPyTracker_Close(ctx, *ht);
+    }
+    if (current_arg_needs_closing) {
+        HPy_Close(ctx, current_arg);
+    }
+    return 0;
+}
+
+
+/**
+ * Parse positional and keyword arguments.
+ *
+ * :param ctx:
+ *     The execution context.
+ * :param ht:
+ *     An optional pointer to an HPyTracker. If the format string never
+ *     results in new handles being created, ``ht`` may be ``NULL``. Currently
+ *     only the ``O`` formatting option to this function requires an HPyTracker.
+ * :param args:
+ *     The array of positional arguments to parse.
+ * :param nargs:
+ *     The number of elements in ``args``.
+ * :param kwnames:
+ *     A handle to the tuple of keyword argument names (may be ``HPy_NULL``).
+ *     The values of the keyword arguments are appended to ``args``. Argument
+ *     ``nargs`` does not include the keyword argument count.
+ * :param fmt:
+ *     The format string to use to parse the arguments.
+ * :param keywords:
+ *     A ``NULL``-terminated array of argument names. The number of names
+ *     should match the format string provided. Positional only arguments
+ *     should have the name ``""`` (i.e. the null-terminated empty string).
+ *     Positional only arguments must preceded all other arguments.
+ * :param ...:
+ *     A va_list of references to variables in which to store the parsed
+ *     arguments. The number and types of the arguments should match the
+ *     the format string, ``fmt``.
+ *
+ * :returns: ``0`` on failure, ``1`` on success.
+ *
+ * If a ``NULL`` pointer is passed to ``ht`` and an HPyTracker is required by
+ * the format string, a ``SystemError`` will be raised.
+ *
+ * If a pointer is provided to ``ht``, the HPyTracker will always be created and
+ * must be closed with ``HPyTracker_Close`` if parsing succeeds (after all
+ * handles returned are no longer needed). If parsing fails, this function will
+ * close the HPyTracker automatically.
+ *
+ * Examples:
+ *
+ * Using `HPyArg_ParseKeywords` without an `HPyTracker`:
+ *
+ * .. code-block:: c
+ *
+ *     long a, b;
+ *     if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kwnames, "ll", &a, &b))
+ *         return HPy_NULL;
+ *     ...
+ *
+ * Using `HPyArg_ParseKeywords` with an `HPyTracker`:
+ *
+ * .. code-block:: c
+ *
+ *     HPy a, b;
+ *     HPyTracker ht;
+ *     if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kwnames, "OO", &a, &b))
+ *         return HPy_NULL;
+ *     ...
+ *     HPyTracker_Close(ctx, ht);
+ *     ...
+ *
+ * .. note::
+ *
+ *     Currently ``HPyArg_ParseKeywords`` only requires the use of an
+ *     ``HPyTracker`` when the ``O`` format is used. In future other new format
+ *     string codes (e.g. for character strings) may also require it.
+ */
+HPyAPI_HELPER int
+HPyArg_ParseKeywords(HPyContext *ctx, HPyTracker *ht, const HPy *args,
+                     size_t nargs, HPy kwnames, const char *fmt,
+                     const char *keywords[], ...)
+{
+    int retval;
+    va_list va;
+
+    va_start(va, keywords);
+    retval = parse_keywords(ctx, ht, args, nargs, kwnames, 1, fmt, keywords, &va);
+    va_end(va);
+    return retval;
+}
+
+/**
+ * Parse positional arguments and keyword arguments in a dict.
+ *
+ * :param ctx:
+ *     The execution context.
+ * :param ht:
+ *     An optional pointer to an HPyTracker. If the format string never
+ *     results in new handles being created, ``ht`` may be ``NULL``. Currently
+ *     only the ``O`` formatting option to this function requires an HPyTracker.
+ * :param args:
+ *     The array of positional arguments to parse.
+ * :param nargs:
+ *     The number of elements in ``args``.
+ * :param kw:
+ *     A handle to the dictionary of keyword arguments (may be ``HPy_NULL``).
+ * :param fmt:
+ *     The format string to use to parse the arguments.
+ * :param keywords:
+ *     A ``NULL``-terminated array of argument names. The number of names
+ *     should match the format string provided. Positional only arguments
+ *     should have the name ``""`` (i.e. the null-terminated empty string).
+ *     Positional only arguments must preceded all other arguments.
+ * :param ...:
+ *     A va_list of references to variables in which to store the parsed
+ *     arguments. The number and types of the arguments should match the
+ *     the format string, ``fmt``.
+ *
+ * :returns: ``0`` on failure, ``1`` on success.
+ *
+ * If a ``NULL`` pointer is passed to ``ht`` and an HPyTracker is required by
+ * the format string, a ``SystemError`` will be raised.
+ *
+ * If a pointer is provided to ``ht``, the HPyTracker will always be created and
+ * must be closed with ``HPyTracker_Close`` if parsing succeeds (after all
+ * handles returned are no longer needed). If parsing fails, this function will
+ * close the HPyTracker automatically.
+ *
+ * For examples, see :c:func:`HPyArg_ParseKeywords`.
+ */
+HPyAPI_HELPER int
+HPyArg_ParseKeywordsDict(HPyContext *ctx, HPyTracker *ht, const HPy *args,
+                         HPy_ssize_t nargs, HPy kw, const char *fmt,
+                         const char *keywords[], ...)
+{
+    int retval;
+    va_list va;
+
+    va_start(va, keywords);
+    retval = parse_keywords(ctx, ht, args, nargs, kw, 0, fmt, keywords, &va);
+    va_end(va);
+    return retval;
 }
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/buildvalue.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/buildvalue.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 /**
  * Implementation of HPy_BuildValue.
  *
- * Note: HPy_BuildValue is a runtime helper functions, i.e., it is not a part
- * of the HPy context, but is available to HPy extensions to incorporate at
- * compile time.
- *
- * HPy_BuildValue creates a new value based on a format string from the values
- * passed in variadic arguments. Returns HPy_NULL in case of an error and raises
- * an exception.
- *
- * HPy_BuildValue does not always build a tuple. It builds a tuple only if its format
- * string contains two or more format units. If the format string is empty, it returns
- * None; if it contains exactly one format unit, it returns whatever object is described
- * by that format unit. To force it to return a tuple of size 0 or one, parenthesize the
- * format string.
- *
- * Building complex values with HPy_BuildValue is more convenient than the equivalent
- * code that uses more granular APIs with proper error handling and cleanup. Moreover,
- * HPy_BuildValue provides straightforward way to port existing code that uses
- * Py_BuildValue.
- *
- * HPy_BuildValue always returns a new handle that will be owned by the caller. Even
- * an artificial example 'HPy_BuildValue(ctx, "O", h)' does not simply forward
- * the value stored in 'h' but duplicates the handle.
+ * Note: :c:func:`HPy_BuildValue` is a runtime helper functions, i.e., it is not
+ * a part of the HPy context, but is available to HPy extensions to incorporate
+ * at compile time.
+ *
+ * ``HPy_BuildValue`` creates a new value based on a format string from the
+ * values passed in variadic arguments. Returns ``HPy_NULL`` in case of an error
+ * and raises an exception.
+ *
+ * ``HPy_BuildValue`` does not always build a tuple. It builds a tuple only if
+ * its format string contains two or more format units. If the format string is
+ * empty, it returns ``None``; if it contains exactly one format unit, it
+ * returns whatever object is described by that format unit. To force it to
+ * return a tuple of size ``0`` or one, parenthesize the format string.
+ *
+ * Building complex values with ``HPy_BuildValue`` is more convenient than the
+ * equivalent code that uses more granular APIs with proper error handling and
+ * cleanup. Moreover, ``HPy_BuildValue`` provides straightforward way to port
+ * existing code that uses ``Py_BuildValue``.
+ *
+ * ``HPy_BuildValue`` always returns a new handle that will be owned by the
+ * caller. Even an artificial example ``HPy_BuildValue(ctx, "O", h)`` does not
+ * simply forward the value stored in ``h`` but duplicates the handle.
  *
  * Supported Formatting Strings
  * ----------------------------
  *
  * Numbers
  * ~~~~~~~
  *
@@ -44,14 +44,17 @@
  *
  * ``L (int) [long long]``
  *     Convert a C long long to a Python integer object.
  *
  * ``K (int) [unsigned long long]``
  *     Convert a C unsigned long long to a Python integer object.
  *
+ * ``n (int) [HPy_ssize_t]``
+ *     Convert a C HPy_ssize_t to a Python integer object.
+ *
  * ``f (float) [float]``
  *     Convert a C float to a Python floating point number.
  *
  * ``d (float) [double]``
  *     Convert a C double to a Python floating point number.
  *
  * Collections
@@ -97,14 +100,29 @@
 
 static HPy_ssize_t count_items(HPyContext *ctx, const char *fmt, char end);
 static HPy build_tuple(HPyContext *ctx, const char **fmt, va_list *values, HPy_ssize_t size, char expected_end);
 static HPy build_list(HPyContext *ctx, const char **fmt, va_list *values, HPy_ssize_t size);
 static HPy build_dict(HPyContext *ctx, const char **fmt, va_list *values);
 static HPy build_single(HPyContext *ctx, const char **fmt, va_list *values, int *needs_close);
 
+/**
+ * Creates a new value based on a format string from the values passed in
+ * variadic arguments.
+ *
+ * :param ctx:
+ *     The execution context.
+ * :param fmt:
+ *     The format string (ASCII only; must not be ``NULL``). For details, see
+ *     :ref:`api-reference/build-value:supported formatting strings`.
+ * :param ...:
+ *     Variable arguments according to the provided format string.
+ *
+ * :returns:
+ *     A handle to the built Python value or ``HPy_NULL`` in case of errors.
+ */
 HPyAPI_HELPER
 HPy HPy_BuildValue(HPyContext *ctx, const char *fmt, ...)
 {
     va_list values;
     HPy result;
     va_start(values, fmt);
     HPy_ssize_t size = count_items(ctx, fmt, '\0');
@@ -146,15 +164,15 @@
                 } else {
                     if (level == 0 || top_level_par == 'X') {
                         HPyErr_SetString(ctx, ctx->h_SystemError, "internal error in HPy_BuildValue");
                         return -1;
                     }
                     par_type = top_level_par;
                 }
-                snprintf(msg, MESSAGE_BUF_SIZE, "unmatched '%c' in the format string passed to HPy_BuildValue", par_type);
+                snprintf(msg, sizeof(msg), "unmatched '%c' in the format string passed to HPy_BuildValue", par_type);
                 HPyErr_SetString(ctx, ctx->h_SystemError, msg);
                 return -1;
             }
 
             case '[':
             case '(':
             case '{':
@@ -223,14 +241,17 @@
 
         case 'L':
             return HPyLong_FromLongLong(ctx, va_arg(*values, long long));
 
         case 'K':
             return HPyLong_FromUnsignedLongLong(ctx, va_arg(*values, unsigned long long));
 
+        case 'n':
+            return HPyLong_FromSsize_t(ctx, va_arg(*values, HPy_ssize_t));
+
         case 's':
             return HPyUnicode_FromString(ctx, va_arg(*values, const char*));
 
         case 'O':
         case 'S': {
             HPy handle = va_arg(*values, HPy);
             if (HPy_IsNull(handle)) {
@@ -256,15 +277,15 @@
 
         case 'f': // Note: floats are promoted to doubles when passed in "..."
         case 'd':
             return HPyFloat_FromDouble(ctx, va_arg(*values, double));
 
         default: {
             char message[MESSAGE_BUF_SIZE];
-            snprintf(message, MESSAGE_BUF_SIZE, "bad format char '%c' in the format string passed to HPy_BuildValue", format_char);
+            snprintf(message, sizeof(message), "bad format char '%c' in the format string passed to HPy_BuildValue", format_char);
             HPyErr_SetString(ctx, ctx->h_SystemError, message);
             return HPy_NULL;
         }
     } // switch
 }
 
 static HPy build_dict(HPyContext *ctx, const char **fmt, va_list *values)
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/ctx_bytes.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_bytes.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #include <Python.h>
 #include "hpy.h"
 #include "hpy/runtime/ctx_funcs.h"
 
-#ifdef HPY_UNIVERSAL_ABI
+#ifndef HPY_ABI_CPYTHON
    // for _h2py and _py2h
 #  include "handles.h"
 #endif
 
 
 _HPy_HIDDEN HPy
 ctx_Bytes_FromStringAndSize(HPyContext *ctx, const char *v, HPy_ssize_t len)
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/ctx_listbuilder.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_listbuilder.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #include <stddef.h>
 #include <Python.h>
 #include "hpy.h"
 
-#ifdef HPY_UNIVERSAL_ABI
+#ifndef HPY_ABI_CPYTHON
    // for _h2py and _py2h
 #  include "handles.h"
 #endif
 
 
 _HPy_HIDDEN HPyListBuilder
-ctx_ListBuilder_New(HPyContext *ctx, HPy_ssize_t initial_size)
+ctx_ListBuilder_New(HPyContext *ctx, HPy_ssize_t size)
 {
-    PyObject *lst = PyList_New(initial_size);
+    PyObject *lst = PyList_New(size);
     if (lst == NULL)
         PyErr_Clear();   /* delay the MemoryError */
     return (HPyListBuilder){(HPy_ssize_t)lst};
 }
 
 _HPy_HIDDEN void
 ctx_ListBuilder_Set(HPyContext *ctx, HPyListBuilder builder,
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/ctx_object.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_object.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,33 @@
 #include <Python.h>
 #include "hpy.h"
 
-#ifdef HPY_UNIVERSAL_ABI
+#ifndef HPY_ABI_CPYTHON
    // for _h2py and _py2h
 #  include "handles.h"
 #endif
 
 
 _HPy_HIDDEN void
 ctx_Dump(HPyContext *ctx, HPy h)
 {
     // just use _PyObject_Dump for now, but we might want to add more info
     // about the handle itself in the future.
     _PyObject_Dump(_h2py(h));
 }
 
-/* NOTE: contrarily to CPython, the HPy have to check that h_type is a
-   type. On CPython it's not necessarily because it passes a PyTypeObject*,
-   but here we can only receive an HPy.
-
-   However, we can't/don't want to raise an exception if you pass a non-type,
-   because the CPython version (PyObject_TypeCheck) always succeed and it
-   would be too easy to forget to check the return value. We just raise a
-   fatal error instead.
-
-   Hopefully the slowdown is not too much. If it proves to be too much, we
-   could say that the function is allowed to crash if you pass a non-type, and
-   do the check only in debug mode.
+/* NOTE: In contrast to CPython, HPy has to check that 'h_type' is a type. This
+   is not necessary on CPython because it requires C type 'PyTypeObject *' but
+   here we can only receive an HPy handle. Appropriate checking of the argument
+   will be done in the debug mode.
 */
 _HPy_HIDDEN int
 ctx_TypeCheck(HPyContext *ctx, HPy h_obj, HPy h_type)
 {
-    PyObject *type= _h2py(h_type);
-    assert(type != NULL);
-    if (!PyType_Check(type)) {
-        Py_FatalError("HPy_TypeCheck arg 2 must be a type");
-    }
-    return PyObject_TypeCheck(_h2py(h_obj), (PyTypeObject*)type);
+    return PyObject_TypeCheck(_h2py(h_obj), (PyTypeObject*)_h2py(h_type));
 }
 
 _HPy_HIDDEN int
 ctx_Is(HPyContext *ctx, HPy h_obj, HPy h_other)
 {
     return _h2py(h_obj) == _h2py(h_other);
 }
@@ -80,7 +67,27 @@
     PyObject* key_o = PyUnicode_FromString(key);
     if (key_o == NULL)
         return -1;
     int result = PyObject_SetItem(_h2py(obj), key_o, _h2py(value));
     Py_DECREF(key_o);
     return result;
 }
+
+_HPy_HIDDEN int
+ctx_DelItem_i(HPyContext *ctx, HPy obj, HPy_ssize_t idx) {
+    PyObject* key = PyLong_FromSsize_t(idx);
+    if (key == NULL)
+        return -1;
+    int result = PyObject_DelItem(_h2py(obj), key);
+    Py_DECREF(key);
+    return result;
+}
+
+_HPy_HIDDEN int
+ctx_DelItem_s(HPyContext *ctx, HPy obj, const char *key) {
+    PyObject* key_o = PyUnicode_FromString(key);
+    if (key_o == NULL)
+        return -1;
+    int result = PyObject_DelItem(_h2py(obj), key_o);
+    Py_DECREF(key_o);
+    return result;
+}
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/ctx_tracker.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tracker.c`

 * *Files 14% similar despite different names*

```diff
@@ -94,19 +94,14 @@
     if (hp->handles == NULL) {
         free(hp);
         HPyErr_NoMemory(ctx);
         return _hp2ht(0);
     }
     hp->capacity = capacity;
     hp->length = 0;
-    // cppcheck thinks that hp->handles is a memory leak because we cast the
-    // pointer to an int (and thus the pointer is "lost" from its POV, I
-    // suppose). But it's not a real leak because we free it in
-    // ctx_Tracker_Close:
-    // cppcheck-suppress memleak
     return _hp2ht(hp);
 }
 
 static int
 tracker_resize(HPyContext *ctx, _HPyTracker_s *hp, HPy_ssize_t capacity)
 {
     HPy *new_handles;
```

### Comparing `hpy-0.0.4/hpy/devel/src/runtime/ctx_tuplebuilder.c` & `hpy-0.9.0rc1/hpy/devel/src/runtime/ctx_tuplebuilder.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #include <stddef.h>
 #include <Python.h>
 #include "hpy.h"
 
-#ifdef HPY_UNIVERSAL_ABI
+#ifndef HPY_ABI_CPYTHON
    // for _h2py and _py2h
 #  include "handles.h"
 #endif
 
 
 _HPy_HIDDEN HPyTupleBuilder
-ctx_TupleBuilder_New(HPyContext *ctx, HPy_ssize_t initial_size)
+ctx_TupleBuilder_New(HPyContext *ctx, HPy_ssize_t size)
 {
-    PyObject *tup = PyTuple_New(initial_size);
+    PyObject *tup = PyTuple_New(size);
     if (tup == NULL) {
         PyErr_Clear();   /* delay the MemoryError */
         /* note: it's done this way so that the caller doesn't need to
            check if HPyTupleBuilder_New() or every HPyTupleBuilder_Set()
            raised.  If there is a rare error like a MemoryError somewhere,
            further calls to the HPyTupleBuilder are ignored.  The final
            HPyTupleBuilder_Build() will re-raise the MemoryError and so
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/__main__.py` & `hpy-0.9.0rc1/hpy/tools/autogen/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 """
 Parse public_api.h and generate various stubs around
 """
 import sys
 import py
 import pycparser
 from packaging import version
-if version.parse(pycparser.__version__) < version.parse('2.20'):
-    raise ImportError('You need pycparser>=2.20 to run autogen')
+if version.parse(pycparser.__version__) < version.parse('2.21'):
+    raise ImportError('You need pycparser>=2.21 to run autogen')
 
-from .parse import HPyAPI, PUBLIC_API_H
-from .ctx import autogen_ctx_h, autogen_ctx_def_h
+from .parse import HPyAPI, AUTOGEN_H
+from .ctx import (autogen_ctx_h,
+                  autogen_ctx_def_h,
+                  cpython_autogen_ctx_h)
 from .trampolines import (autogen_trampolines_h,
                           cpython_autogen_api_impl_h,
                           universal_autogen_ctx_impl_h)
 from .hpyfunc import autogen_hpyfunc_declare_h
 from .hpyfunc import autogen_hpyfunc_trampoline_h
 from .hpyfunc import autogen_ctx_call_i
 from .hpyfunc import autogen_cpython_hpyfunc_trampoline_h
 from .hpyslot import autogen_hpyslot_h
 from .debug import (autogen_debug_ctx_init_h,
                     autogen_debug_wrappers,
                     autogen_debug_ctx_call_i)
+from .trace import (autogen_tracer_ctx_init_h,
+                    autogen_tracer_wrappers,
+                    autogen_trace_func_table_c)
 from .pypy import autogen_pypy_txt
+from .doc import (autogen_function_index,
+                  autogen_doc_api_mapping)
+
 
 def main():
     if len(sys.argv) != 2:
         print('Usage: python -m hpy.tools.autogen OUTDIR')
         sys.exit(1)
     outdir = py.path.local(sys.argv[1])
 
-    api = HPyAPI.parse(PUBLIC_API_H)
+    api = HPyAPI.parse(AUTOGEN_H)
     ## for func in api.functions:
     ##     print(func)
 
     for cls in (autogen_ctx_h,
                 autogen_ctx_def_h,
+                cpython_autogen_ctx_h,
                 autogen_trampolines_h,
                 cpython_autogen_api_impl_h,
                 universal_autogen_ctx_impl_h,
                 autogen_hpyfunc_declare_h,
                 autogen_hpyfunc_trampoline_h,
                 autogen_ctx_call_i,
                 autogen_cpython_hpyfunc_trampoline_h,
                 autogen_hpyslot_h,
                 autogen_debug_ctx_init_h,
                 autogen_debug_wrappers,
                 autogen_debug_ctx_call_i,
-                autogen_pypy_txt):
+                autogen_tracer_ctx_init_h,
+                autogen_tracer_wrappers,
+                autogen_trace_func_table_c,
+                autogen_pypy_txt,
+                autogen_function_index,
+                autogen_doc_api_mapping):
         cls(api).write(outdir)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/autogenfile.py` & `hpy-0.9.0rc1/hpy/tools/autogen/autogenfile.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/tools/autogen/debug.py` & `hpy-0.9.0rc1/hpy/tools/autogen/trace.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,182 @@
 from copy import deepcopy
 from pycparser import c_ast
 from .autogenfile import AutoGenFile
 from .parse import toC, find_typedecl, get_context_return_type, \
     maybe_make_void, make_void, get_return_constant
-from .hpyfunc import NO_CALL
 
 
-class HPy_2_DHPy_Visitor(c_ast.NodeVisitor):
-    "Visitor which renames all HPy types to DHPy"
+# We will call the delegate context's function but we still need to unwrap
+# the context. This is in contrast to, e.g., the debug mode, where you would
+# manually write a wrapper function. Here we can generate that as well.
+NO_WRAPPER = {
+    '_HPy_CallRealFunctionFromTrampoline',
+    'HPy_FatalError',
+}
 
-    def visit_IdentifierType(self, node):
-        if node.names == ['HPy']:
-            node.names = ['DHPy']
+class Ctx2TctxVisitor(c_ast.NodeVisitor):
+    """Visitor which renames all ctx to tctx"""
 
     def visit_TypeDecl(self, node):
         if node.declname == 'ctx':
-            node.declname = 'dctx'
+            node.declname = 'tctx'
         self.generic_visit(node)
 
 def funcnode_with_new_name(node, name):
     newnode = deepcopy(node)
     typedecl = find_typedecl(newnode)
     typedecl.declname = name
     return newnode
 
-def get_debug_wrapper_node(func):
-    newnode = funcnode_with_new_name(func.node, 'debug_%s' % func.ctx_name())
+def get_trace_wrapper_node(func):
+    newnode = funcnode_with_new_name(func.node, 'trace_%s' % func.ctx_name())
     maybe_make_void(func, newnode)
-    # fix all the types
-    visitor = HPy_2_DHPy_Visitor()
+    # rename ctx to tctx
+    visitor = Ctx2TctxVisitor()
     visitor.visit(newnode)
     return newnode
 
-
-class autogen_debug_ctx_init_h(AutoGenFile):
-    PATH = 'hpy/debug/src/autogen_debug_ctx_init.h'
+class autogen_tracer_ctx_init_h(AutoGenFile):
+    PATH = 'hpy/trace/src/autogen_trace_ctx_init.h'
 
     def generate(self):
         lines = []
         w = lines.append
-        # emit the declarations for all the debug_ctx_* functions
+        # emit the declarations for all the trace_ctx_* functions
         for func in self.api.functions:
-            w(toC(get_debug_wrapper_node(func)) + ';')
+            if func.name not in NO_WRAPPER:
+                w(toC(get_trace_wrapper_node(func)) + ';')
+        n_decls = len(self.api.functions) + len(self.api.variables)
+        w('')
+        w(f'static inline void trace_ctx_init_info(HPyTraceInfo *info, HPyContext *uctx)')
+        w('{')
+        w(f'    info->magic_number = HPY_TRACE_MAGIC;')
+        w(f'    info->uctx = uctx;')
+        w(f'    info->call_counts = (uint64_t *)calloc({n_decls}, sizeof(uint64_t));')
+        w(f'    info->durations = (_HPyTime_t *)calloc({n_decls}, sizeof(_HPyTime_t));')
+        w(f'    info->on_enter_func = HPy_NULL;')
+        w(f'    info->on_exit_func = HPy_NULL;')
+        w('}')
         w('')
-        w('static inline void debug_ctx_init_fields(HPyContext *dctx, HPyContext *uctx)')
+        w(f'static inline void trace_ctx_free_info(HPyTraceInfo *info)')
+        w('{')
+        w(f'    assert(info->magic_number == HPY_TRACE_MAGIC);')
+        w(f'    free(info->call_counts);')
+        w(f'    free(info->durations);')
+        w(f'    HPy_Close(info->uctx, info->on_enter_func);')
+        w(f'    HPy_Close(info->uctx, info->on_exit_func);')
+        w('}')
+        w('')
+        w(f'static inline void trace_ctx_init_fields(HPyContext *tctx, HPyContext *uctx)')
         w('{')
         for var in self.api.variables:
             name = var.name
-            w(f'    dctx->{name} = DHPy_open(dctx, uctx->{name});')
+            w(f'    tctx->{name} = uctx->{name};')
         for func in self.api.functions:
-            name = func.ctx_name()
-            w(f'    dctx->{name} = &debug_{name};')
-
+            if func.name in NO_WRAPPER:
+                name = func.ctx_name()
+                w(f'    tctx->{name} = uctx->{name};')
+            else:
+                name = func.ctx_name()
+                w(f'    tctx->{name} = &trace_{name};')
         w('}')
         return '\n'.join(lines)
 
 
-class autogen_debug_wrappers(AutoGenFile):
-    PATH = 'hpy/debug/src/autogen_debug_wrappers.c'
-
-    NO_WRAPPER = {
-        '_HPy_CallRealFunctionFromTrampoline',
-        'HPy_Close',
-        'HPyUnicode_AsUTF8AndSize',
-        'HPyTuple_FromArray',
-        'HPyType_GenericNew',
-        'HPyType_FromSpec',
-        'HPyTracker_New',
-        'HPyTracker_Add',
-        'HPyTracker_ForgetAll',
-        'HPyTracker_Close',
-    }
+class autogen_tracer_wrappers(AutoGenFile):
+    PATH = 'hpy/trace/src/autogen_trace_wrappers.c'
 
     def generate(self):
         lines = []
         w = lines.append
-        w('#include "debug_internal.h"')
+        w('#include "trace_internal.h"')
         w('')
         for func in self.api.functions:
-            debug_wrapper = self.gen_debug_wrapper(func)
+            debug_wrapper = self.gen_trace_wrapper(func)
             if debug_wrapper:
                 w(debug_wrapper)
                 w('')
         return '\n'.join(lines)
 
-    def gen_debug_wrapper(self, func):
-        if func.name in self.NO_WRAPPER:
+    def gen_trace_wrapper(self, func):
+        if func.name in NO_WRAPPER:
             return
-        #
+
         assert not func.is_varargs()
-        node = get_debug_wrapper_node(func)
+        node = get_trace_wrapper_node(func)
         const_return = get_return_constant(func)
         if const_return:
             make_void(node)
         signature = toC(node)
         rettype = get_context_return_type(node, const_return)
-        #
+
         def get_params():
             lst = []
             for p in node.type.args.params:
                 if p.name == 'ctx':
-                    lst.append('get_info(dctx)->uctx')
-                elif toC(p.type) == 'DHPy':
-                    lst.append('DHPy_unwrap(dctx, %s)' % p.name)
-                elif toC(p.type) in ('DHPy *', 'DHPy []'):
-                    assert False, ('C type %s not supported, please write the wrapper '
-                                   'for %s by hand' % (toC(p.type), func.name))
+                    lst.append('uctx')
                 else:
                     lst.append(p.name)
             return ', '.join(lst)
         params = get_params()
-        #
+
         lines = []
         w = lines.append
         w(signature)
         w('{')
+        w(f'    HPyTraceInfo *info = hpy_trace_on_enter(tctx, {func.ctx_index});')
+        w(f'    HPyContext *uctx = info->uctx;')
+        w(f'    _HPyTime_t _ts_start, _ts_end;')
+        w(f'    _HPyClockStatus_t r0, r1;')
+        w(f'    r0 = get_monotonic_clock(&_ts_start);')
         if rettype == 'void':
             w(f'    {func.name}({params});')
-        elif rettype == 'DHPy':
-            w(f'    return DHPy_open(dctx, {func.name}({params}));')
         else:
-            w(f'    return {func.name}({params});')
+            w(f'    {rettype} res = {func.name}({params});')
+        w(f'    r1 = get_monotonic_clock(&_ts_end);')
+        w(f'    hpy_trace_on_exit(info, {func.ctx_index}, r0, r1, &_ts_start, &_ts_end);')
+        if rettype != 'void':
+            w(f'    return res;')
         w('}')
         return '\n'.join(lines)
 
 
-class autogen_debug_ctx_call_i(AutoGenFile):
-    PATH = 'hpy/debug/src/autogen_debug_ctx_call.i'
+class autogen_trace_func_table_c(AutoGenFile):
+    PATH = 'hpy/trace/src/autogen_trace_func_table.c'
 
     def generate(self):
         lines = []
         w = lines.append
-        for hpyfunc in self.api.hpyfunc_typedefs:
-            name = hpyfunc.base_name()
-            NAME = name.upper()
-            if NAME in NO_CALL:
-                continue
-            #
-            c_ret_type = toC(hpyfunc.return_type())
-            args = ['dctx']
-            dhpys = []
-            for i, param in enumerate(hpyfunc.params()[1:]):
-                pname = param.name
-                if pname is None:
-                    pname = 'arg%d' % i
-                if toC(param.type) == 'HPy':
-                    dhpys.append(pname)
-                    args.append(f'dh_{pname}')
-                else:
-                    args.append(f'a->{pname}')
-            args = ', '.join(args)
-            #
-            w(f'    case HPyFunc_{NAME}: {{')
-            w(f'        HPyFunc_{name} f = (HPyFunc_{name})func;')
-            w(f'        _HPyFunc_args_{NAME} *a = (_HPyFunc_args_{NAME}*)args;')
-            for pname in dhpys:
-                w(f'        DHPy dh_{pname} = _py2dh(dctx, a->{pname});')
-            #
-            if c_ret_type == 'void':
-                w(f'        f({args});')
-            elif c_ret_type == 'HPy':
-                w(f'        DHPy dh_result = f({args});')
-            else:
-                w(f'        a->result = f({args});')
-            #
-            for pname in dhpys:
-                w(f'        DHPy_close_and_check(dctx, dh_{pname});')
-            #
-            if c_ret_type == 'HPy':
-                w(f'        a->result = _dh2py(dctx, dh_result);')
-                w(f'        DHPy_close(dctx, dh_result);')
-            #
-            w(f'        return;')
-            w(f'    }}')
+
+        n_funcs = len(self.api.functions)
+        n_decls = n_funcs + len(self.api.variables)
+        func_table = ['NO_FUNC'] * n_decls
+        for func in self.api.functions:
+            name = func.ctx_name()
+            func_table[func.ctx_index] = f'"{name}"'
+
+        w('#include "trace_internal.h"')
+        w('')
+        w(f'#define TRACE_NFUNC {n_funcs}')
+        w('')
+        w('#define NO_FUNC ""')
+        w('static const char *trace_func_table[] = {')
+        for func in func_table:
+            w(f'    {func},')
+        w(f'    NULL /* sentinel */')
+        w('};')
+        w('')
+        w('int hpy_trace_get_nfunc(void)')
+        w('{')
+        w('    return TRACE_NFUNC;')
+        w('}')
+        w('')
+        w('const char * hpy_trace_get_func_name(int idx)')
+        w('{')
+        w(f'    if (idx >= 0 && idx < {n_decls})')
+        w('        return trace_func_table[idx];')
+        w('    return NULL;')
+        w('}')
+        w('')
         return '\n'.join(lines)
+
+
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/hpyfunc.py` & `hpy-0.9.0rc1/hpy/tools/autogen/hpyfunc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from copy import deepcopy
 from pycparser import c_ast
 from .autogenfile import AutoGenFile
 from .parse import toC, find_typedecl
 
-NO_CALL = ('NOARGS', 'O', 'VARARGS', 'KEYWORDS', 'INITPROC', 'DESTROYFUNC',
-           'GETBUFFERPROC', 'RELEASEBUFFERPROC', 'TRAVERSEPROC')
+NO_CALL = ('VARARGS', 'KEYWORDS', 'INITPROC', 'DESTROYFUNC',
+           'GETBUFFERPROC', 'RELEASEBUFFERPROC', 'TRAVERSEPROC', 'MOD_CREATE',
+           'VECTORCALLFUNC', 'NEWFUNC')
 NO_TRAMPOLINE = NO_CALL + ('RICHCMPFUNC',)
 
+# This is a list of type that can automatically be converted from Python to HPy
+# and vice versa.
+AUTO_CONVERSION_TYPES = ('HPy', 'HPy_ssize_t', 'void *', 'int', 'char *',
+                         'HPy_hash_t', 'HPy_RichCmpOp', 'void')
+
 class autogen_hpyfunc_declare_h(AutoGenFile):
     PATH = 'hpy/devel/include/hpy/autogen_hpyfunc_declare.h'
 
     ## #define _HPyFunc_DECLARE_HPyFunc_NOARGS(SYM)  \
     ##     static HPy SYM(HPyContext *ctx, HPy self)
 
     def generate(self):
         lines = []
         w = lines.append
         for hpyfunc in self.api.hpyfunc_typedefs:
             # declare a function named 'SYM' of the appropriate type
             funcdecl = hpyfunc.node.type.type
             symdecl = deepcopy(funcdecl)
+            if isinstance(symdecl.type, c_ast.PtrDecl):
+                symdecl.type = symdecl.type.type
             symdecl.type.declname = 'SYM'
             symdecl = toC(symdecl)
             #
             # generate a macro emitting 'symdecl'
             name = hpyfunc.base_name().upper()
             w(f'#define _HPyFunc_DECLARE_HPyFunc_{name}(SYM) static {symdecl}')
         w('')
@@ -51,17 +59,19 @@
         w = lines.append
         for hpyfunc in self.api.hpyfunc_typedefs:
             NAME = hpyfunc.base_name().upper()
             if NAME in NO_TRAMPOLINE:
                 continue
             #
             tramp_node = deepcopy(hpyfunc.node.type.type)
+            if isinstance(tramp_node.type, c_ast.PtrDecl):
+                tramp_node.type = tramp_node.type.type
             tramp_node.type.declname = 'SYM'
             tramp_node = hpy_to_cpy(tramp_node)
-            assert toC(tramp_node.args.params[0].type) == 'HPyContext *'
+            assert toC(tramp_node.args.params[0].type) in ['void', 'HPyContext *']
             tramp_node.args.params = [hpy_to_cpy(p)
                                       for p in tramp_node.args.params[1:]]
             for i, param in enumerate(tramp_node.args.params):
                 typedecl = find_typedecl(param.type)
                 if typedecl.declname is None:
                     param.name = 'arg%d' % i
                     typedecl.declname = 'arg%d' % i
@@ -89,14 +99,30 @@
             else:
                 w(f'        return a.result; \\')
             w(f'    }}')
             w('')
         return '\n'.join(lines)
 
 
+def _py2h(type):
+    if type == 'HPy':
+        return '_py2h'
+    elif type in AUTO_CONVERSION_TYPES:
+        return ''
+    raise TypeError(f'cannot generate automatic conversion for type \'{type}\'')
+
+
+def _h2py(type):
+    if type == 'HPy':
+        return '_h2py'
+    elif type in AUTO_CONVERSION_TYPES:
+        return ''
+    raise TypeError(f'cannot generate automatic conversion for type \'{type}\'')
+
+
 class autogen_ctx_call_i(AutoGenFile):
     PATH = 'hpy/universal/src/autogen_ctx_call.i'
 
     def generate(self):
         lines = []
         w = lines.append
         for hpyfunc in self.api.hpyfunc_typedefs:
@@ -107,29 +133,24 @@
             #
             c_ret_type = toC(hpyfunc.return_type())
             args = ['ctx']
             for i, param in enumerate(hpyfunc.params()[1:]):
                 pname = param.name
                 if pname is None:
                     pname = 'arg%d' % i
-                if toC(param.type) == 'HPy':
-                    args.append(f'_py2h(a->{pname})')
-                else:
-                    args.append(f'a->{pname}')
+                args.append(f'{_py2h(toC(param.type))}(a->{pname})')
             args = ', '.join(args)
             #
             w(f'    case HPyFunc_{NAME}: {{')
             w(f'        HPyFunc_{name} f = (HPyFunc_{name})func;')
             w(f'        _HPyFunc_args_{NAME} *a = (_HPyFunc_args_{NAME}*)args;')
             if c_ret_type == 'void':
                 w(f'        f({args});')
-            elif c_ret_type == 'HPy':
-                w(f'        a->result = _h2py(f({args}));')
             else:
-                w(f'        a->result = f({args});')
+                w(f'        a->result = {_h2py(c_ret_type)}(f({args}));')
             w(f'        return;')
             w(f'    }}')
         return '\n'.join(lines)
 
 
 class autogen_cpython_hpyfunc_trampoline_h(AutoGenFile):
     PATH = 'hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h'
@@ -140,40 +161,36 @@
         for hpyfunc in self.api.hpyfunc_typedefs:
             name = hpyfunc.base_name()
             NAME = name.upper()
             if NAME in NO_TRAMPOLINE:
                 continue
             #
             tramp_node = deepcopy(hpyfunc.node.type.type)
+            if isinstance(tramp_node.type, c_ast.PtrDecl):
+                tramp_node.type = tramp_node.type.type
             tramp_node.type.declname = 'SYM'
             tramp_node = hpy_to_cpy(tramp_node)
             tramp_node.args.params = [hpy_to_cpy(p)
                                       for p in tramp_node.args.params[1:]]
             for i, param in enumerate(tramp_node.args.params):
                 typedecl = find_typedecl(param.type)
                 if typedecl.declname is None:
                     param.name = 'arg%d' % i
                     typedecl.declname = 'arg%d' % i
 
-            if toC(hpyfunc.return_type()) == 'HPy':
-                result = '_h2py'
-            else:
-                result = ''
+            result = _h2py(toC(hpyfunc.return_type()))
             args = ['_HPyGetContext()']
             func_ptr_ret_type = toC(hpyfunc.return_type())
             func_ptr_sig = ['HPyContext *']
             for i, param in enumerate(hpyfunc.params()[1:]):
                 pname = param.name
                 if pname is None:
                     pname = 'arg%d' % i
                 func_ptr_sig.append(toC(param.type))
-                if toC(param.type) == 'HPy':
-                    args.append(f'_py2h({pname})')
-                else:
-                    args.append(f'{pname}')
+                args.append(f'{_py2h(toC(param.type))}({pname})')
             args = ', '.join(args)
             func_ptr_sig = ', '.join(func_ptr_sig)
             #
             w(f'typedef {func_ptr_ret_type} (*_HPyCFunction_{NAME})({func_ptr_sig});')
             w(f'#define _HPyFunc_TRAMPOLINE_HPyFunc_{NAME}(SYM, IMPL) \\')
             w(f'    static {toC(tramp_node)} \\')
             w(f'    {{ \\')
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/hpyslot.py` & `hpy-0.9.0rc1/hpy/tools/autogen/hpyslot.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/tools/autogen/pypy.py` & `hpy-0.9.0rc1/hpy/tools/autogen/pypy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .autogenfile import AutoGenFile
 from .parse import toC
 
 # this class should probably be moved somewhere in the PyPy repo
 class autogen_pypy_txt(AutoGenFile):
     PATH = 'hpy/tools/autogen/autogen_pypy.txt'
-    LANGUAGE = 'txt' # to avoid insering the disclaimer
+    LANGUAGE = 'txt' # to avoid inserting the disclaimer
 
     def generate(self):
         lines = []
         w = lines.append
         w("typedef struct _HPyContext_s {")
-        w("    int ctx_version;")
+        w("    int abi_version;")
         for var in self.api.variables:
             w("    struct _HPy_s %s;" % var.ctx_name())
         for func in self.api.functions:
             w("    void * %s;" % func.ctx_name())
         w("} _struct_HPyContext_s;")
         w("")
         w("")
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/testing/test_autogen.py` & `hpy-0.9.0rc1/hpy/tools/autogen/testing/test_autogen.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,40 +27,43 @@
 
     @pytest.fixture
     def initargs(self, tmpdir):
         self.tmpdir = tmpdir
 
     def parse(self, src):
         fname = self.tmpdir.join('test_api.h')
-        # automatically add usefuly typedefs
+        # automatically add useful typedefs
         src = """
+            #define STRINGIFY(X) #X
+            #define HPy_ID(X) _Pragma(STRINGIFY(id=X)) \\
+
             typedef int HPy;
             typedef int HPyContext;
         """ + src
         fname.write(src)
         return HPyAPI.parse(fname)
 
 
 class TestHPyAPI(BaseTestAutogen):
 
     def test_ctx_name(self):
         api = self.parse("""
-            HPy h_None;
-            HPy HPy_Dup(HPyContext *ctx, HPy h);
-            void* _HPy_AsStruct(HPyContext *ctx, HPy h);
+            HPy_ID(0) HPy h_None;
+            HPy_ID(1) HPy HPy_Dup(HPyContext *ctx, HPy h);
+            HPy_ID(2) void* _HPy_AsStruct(HPyContext *ctx, HPy h);
         """)
         assert api.get_var('h_None').ctx_name() == 'h_None'
         assert api.get_func('HPy_Dup').ctx_name() == 'ctx_Dup'
         assert api.get_func('_HPy_AsStruct').ctx_name() == 'ctx_AsStruct'
 
     def test_cpython_name(self):
         api = self.parse("""
-            HPy HPy_Dup(HPyContext *ctx, HPy h);
-            long HPyLong_AsLong(HPyContext *ctx, HPy h);
-            HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
+            HPy_ID(0) HPy HPy_Dup(HPyContext *ctx, HPy h);
+            HPy_ID(1) long HPyLong_AsLong(HPyContext *ctx, HPy h);
+            HPy_ID(2) HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
         """)
         assert api.get_func('HPy_Dup').cpython_name is None
         assert api.get_func('HPyLong_AsLong').cpython_name == 'PyLong_AsLong'
         assert api.get_func('HPy_Add').cpython_name == 'PyNumber_Add'
 
     def test_hpyslot(self):
         api = self.parse("""
@@ -73,79 +76,115 @@
         assert nb_add.value == '7'
         assert nb_add.hpyfunc == 'HPyFunc_BINARYFUNC'
         #
         tp_repr = api.get_slot('HPy_tp_repr')
         assert tp_repr.value == '66'
         assert tp_repr.hpyfunc == 'HPyFunc_REPRFUNC'
 
+    def test_parse_id(self):
+        api = self.parse("""
+            HPy_ID(0) HPy h_Foo;
+            HPy_ID(1)
+            long HPyFoo_Bar(HPyContext *ctx, HPy h);
+        """)
+        assert len(api.variables) == 1
+        assert len(api.functions) == 1
+        assert api.variables[0].ctx_index == 0
+        assert api.functions[0].ctx_index == 1
+
+        # don't allow gaps in the sequence of IDs
+        with pytest.raises(AssertionError):
+            self.parse("""
+            HPy_ID(0) HPy h_Foo;
+            HPy_ID(3) long HPyFoo_Bar(HPyContext *ctx, HPy h);
+            """)
+
+        # don't allow re-using of IDs
+        with pytest.raises(AssertionError):
+            self.parse("""
+            HPy_ID(0) HPy h_Foo;
+            HPy_ID(0) HPy h_Foo;
+            """)
+
+        # all context members must have an ID
+        with pytest.raises(ValueError):
+            self.parse("HPy h_Foo;")
+
+        # pragmas must be of form '#pramga key=value'
+        with pytest.raises(ValueError):
+            self.parse("#pragma hello\nHPy h_Foo;")
+
+        # pragmas value must be an integer
+        with pytest.raises(ValueError):
+            self.parse("#pragma hello=world\nHPy h_Foo;")
 
 class TestAutoGen(BaseTestAutogen):
 
     def test_autogen_ctx_h(self):
         api = self.parse("""
-            HPy h_None;
-            HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
+            HPy_ID(0) HPy h_None;
+            HPy_ID(1) HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
         """)
         got = autogen_ctx_h(api).generate()
         exp = """
             struct _HPyContext_s {
                 const char *name; // used just to make debugging and testing easier
                 void *_private;   // used by implementations to store custom data
-                int ctx_version;
+                int abi_version;
                 HPy h_None;
                 HPy (*ctx_Add)(HPyContext *ctx, HPy h1, HPy h2);
             };
         """
         assert src_equal(exp, got)
 
     def test_autogen_ctx_def_h(self):
         api = self.parse("""
-            HPy h_None;
-            HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
+            HPy_ID(0) HPy h_None;
+            HPy_ID(1) HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
         """)
         got = autogen_ctx_def_h(api).generate()
         exp = """
             struct _HPyContext_s g_universal_ctx = {
                 .name = "HPy Universal ABI (CPython backend)",
                 ._private = NULL,
-                .ctx_version = 1,
+                .abi_version = HPY_ABI_VERSION,
                 /* h_None & co. are initialized by init_universal_ctx() */
                 .ctx_Add = &ctx_Add,
             };
         """
         assert src_equal(exp, got)
 
     def test_autogen_trampolines_h(self):
         api = self.parse("""
-            HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
-            void HPy_Close(HPyContext *ctx, HPy h);
-            void* _HPy_AsStruct(HPyContext *ctx, HPy h);
+            HPy_ID(0) HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
+            HPy_ID(1) void HPy_Close(HPyContext *ctx, HPy h);
+            HPy_ID(2) void* _HPy_AsStruct(HPyContext *ctx, HPy h);
         """)
         got = autogen_trampolines_h(api).generate()
         exp = """
-            static inline HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2) {
+            HPyAPI_FUNC HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2) {
                 return ctx->ctx_Add ( ctx, h1, h2 );
             }
 
-            static inline void HPy_Close(HPyContext *ctx, HPy h) {
+            HPyAPI_FUNC void HPy_Close(HPyContext *ctx, HPy h) {
                 ctx->ctx_Close ( ctx, h );
             }
 
-            static inline void *_HPy_AsStruct(HPyContext *ctx, HPy h) {
+            HPyAPI_FUNC void *_HPy_AsStruct(HPyContext *ctx, HPy h) {
                 return ctx->ctx_AsStruct ( ctx, h );
             }
         """
         assert src_equal(got, exp)
 
     def test_cpython_api_impl_h(self):
         api = self.parse("""
-            HPy HPy_Dup(HPyContext *ctx, HPy h);
-            HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
-            HPy HPyLong_FromLong(HPyContext *ctx, long value);
-            char* HPyBytes_AsString(HPyContext *ctx, HPy h);
+            HPy_ID(0) HPy HPy_Dup(HPyContext *ctx, HPy h);
+            HPy_ID(1) HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2);
+            HPy_ID(2) HPy HPyLong_FromLong(HPyContext *ctx, long value);
+            HPy_ID(3) char* HPyBytes_AsString(HPyContext *ctx, HPy h);
         """)
         got = cpython_autogen_api_impl_h(api).generate()
         exp = """
             HPyAPI_FUNC
             HPy HPy_Add(HPyContext *ctx, HPy h1, HPy h2)
             {
                 return _py2h(PyNumber_Add(_h2py(h1), _h2py(h2)));
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/testing/test_hpyfunc.py` & `hpy-0.9.0rc1/hpy/tools/autogen/testing/test_hpyfunc.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,43 +46,43 @@
             } _HPyFunc_args_FOO;
 
             #define _HPyFunc_TRAMPOLINE_HPyFunc_FOO(SYM, IMPL) \
                 static cpy_PyObject *SYM(cpy_PyObject *arg, int xy) \
                 { \
                     _HPyFunc_args_FOO a = { arg, xy }; \
                     _HPy_CallRealFunctionFromTrampoline( \
-                       _ctx_for_trampolines, HPyFunc_FOO, IMPL, &a); \
+                       _ctx_for_trampolines, HPyFunc_FOO, (HPyCFunction)IMPL, &a); \
                     return a.result; \
                 }
 
             typedef struct {
                 cpy_PyObject *arg0;
                 int arg1;
                 cpy_PyObject * result;
             } _HPyFunc_args_BAR;
 
             #define _HPyFunc_TRAMPOLINE_HPyFunc_BAR(SYM, IMPL) \
                 static cpy_PyObject *SYM(cpy_PyObject *arg0, int arg1) \
                 { \
                     _HPyFunc_args_BAR a = { arg0, arg1 }; \
                     _HPy_CallRealFunctionFromTrampoline( \
-                       _ctx_for_trampolines, HPyFunc_BAR, IMPL, &a); \
+                       _ctx_for_trampolines, HPyFunc_BAR, (HPyCFunction)IMPL, &a); \
                     return a.result; \
                 }
 
             typedef struct {
                 int x;
             } _HPyFunc_args_PROC;
 
             #define _HPyFunc_TRAMPOLINE_HPyFunc_PROC(SYM, IMPL) \
                 static void SYM(int x) \
                 { \
                     _HPyFunc_args_PROC a = { x }; \
                     _HPy_CallRealFunctionFromTrampoline( \
-                       _ctx_for_trampolines, HPyFunc_PROC, IMPL, &a); \
+                       _ctx_for_trampolines, HPyFunc_PROC, (HPyCFunction)IMPL, &a); \
                     return; \
                 }
         """
         assert src_equal(got, exp)
 
     def test_autogen_ctx_call_i(self):
         api = self.parse("""
@@ -123,19 +123,23 @@
     def test_autogen_cpython_hpyfunc_trampoline_h(self):
         api = self.parse("""
             typedef HPy (*HPyFunc_foo)(HPyContext *ctx, HPy arg, int xy);
             typedef HPy (*HPyFunc_bar)(HPyContext *ctx, HPy, int);
         """)
         got = autogen_cpython_hpyfunc_trampoline_h(api).generate()
         exp = r"""
+            typedef HPy (*_HPyCFunction_FOO)(HPyContext *, HPy, int);
             #define _HPyFunc_TRAMPOLINE_HPyFunc_FOO(SYM, IMPL) \
                 static cpy_PyObject *SYM(cpy_PyObject *arg, int xy) \
                 { \
-                    return _h2py(IMPL(_HPyGetContext(), _py2h(arg), xy)); \
+                    _HPyCFunction_FOO func = (_HPyCFunction_FOO)IMPL; \
+                    return _h2py(func(_HPyGetContext(), _py2h(arg), xy)); \
                 }
+            typedef HPy (*_HPyCFunction_BAR)(HPyContext *, HPy, int);
             #define _HPyFunc_TRAMPOLINE_HPyFunc_BAR(SYM, IMPL) \
                 static cpy_PyObject *SYM(cpy_PyObject *arg0, int arg1) \
                 { \
-                    return _h2py(IMPL(_HPyGetContext(), _py2h(arg0), arg1)); \
+                    _HPyCFunction_BAR func = (_HPyCFunction_BAR)IMPL; \
+                    return _h2py(func(_HPyGetContext(), _py2h(arg0), arg1)); \
                 }
         """
         assert src_equal(got, exp)
```

### Comparing `hpy-0.0.4/hpy/tools/autogen/trampolines.py` & `hpy-0.9.0rc1/hpy/tools/autogen/trampolines.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/tools/valgrind/hpy.supp` & `hpy-0.9.0rc1/hpy/tools/valgrind/hpy.supp`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {
-   <ctx_Module_Create_leak>
+   <_HPyModuleDef_CreatePyModuleDef_leak>
    Memcheck:Leak
    match-leak-kinds: definite,indirect
    ...
-   fun:ctx_Module_Create
+   fun:_HPyModuleDef_CreatePyModuleDef
    ...
 }
 
 {
   <ctx_Type_FromSpec_leak>
   Memcheck:Leak
   match-leak-kinds: definite
```

### Comparing `hpy-0.0.4/hpy/tools/valgrind/python.supp` & `hpy-0.9.0rc1/hpy/tools/valgrind/python.supp`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/universal/src/autogen_ctx_call.i` & `hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_call.i`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,26 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
+    case HPyFunc_NOARGS: {
+        HPyFunc_noargs f = (HPyFunc_noargs)func;
+        _HPyFunc_args_NOARGS *a = (_HPyFunc_args_NOARGS*)args;
+        a->result = _h2py(f(ctx, _py2h(a->self)));
+        return;
+    }
+    case HPyFunc_O: {
+        HPyFunc_o f = (HPyFunc_o)func;
+        _HPyFunc_args_O *a = (_HPyFunc_args_O*)args;
+        a->result = _h2py(f(ctx, _py2h(a->self), _py2h(a->arg)));
+        return;
+    }
     case HPyFunc_UNARYFUNC: {
         HPyFunc_unaryfunc f = (HPyFunc_unaryfunc)func;
         _HPyFunc_args_UNARYFUNC *a = (_HPyFunc_args_UNARYFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0)));
         return;
     }
     case HPyFunc_BINARYFUNC: {
@@ -27,99 +39,99 @@
         _HPyFunc_args_TERNARYFUNC *a = (_HPyFunc_args_TERNARYFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_INQUIRY: {
         HPyFunc_inquiry f = (HPyFunc_inquiry)func;
         _HPyFunc_args_INQUIRY *a = (_HPyFunc_args_INQUIRY*)args;
-        a->result = f(ctx, _py2h(a->arg0));
+        a->result = (f(ctx, _py2h(a->arg0)));
         return;
     }
     case HPyFunc_LENFUNC: {
         HPyFunc_lenfunc f = (HPyFunc_lenfunc)func;
         _HPyFunc_args_LENFUNC *a = (_HPyFunc_args_LENFUNC*)args;
-        a->result = f(ctx, _py2h(a->arg0));
+        a->result = (f(ctx, _py2h(a->arg0)));
         return;
     }
     case HPyFunc_SSIZEARGFUNC: {
         HPyFunc_ssizeargfunc f = (HPyFunc_ssizeargfunc)func;
         _HPyFunc_args_SSIZEARGFUNC *a = (_HPyFunc_args_SSIZEARGFUNC*)args;
-        a->result = _h2py(f(ctx, _py2h(a->arg0), a->arg1));
+        a->result = _h2py(f(ctx, _py2h(a->arg0), (a->arg1)));
         return;
     }
     case HPyFunc_SSIZESSIZEARGFUNC: {
         HPyFunc_ssizessizeargfunc f = (HPyFunc_ssizessizeargfunc)func;
         _HPyFunc_args_SSIZESSIZEARGFUNC *a = (_HPyFunc_args_SSIZESSIZEARGFUNC*)args;
-        a->result = _h2py(f(ctx, _py2h(a->arg0), a->arg1, a->arg2));
+        a->result = _h2py(f(ctx, _py2h(a->arg0), (a->arg1), (a->arg2)));
         return;
     }
     case HPyFunc_SSIZEOBJARGPROC: {
         HPyFunc_ssizeobjargproc f = (HPyFunc_ssizeobjargproc)func;
         _HPyFunc_args_SSIZEOBJARGPROC *a = (_HPyFunc_args_SSIZEOBJARGPROC*)args;
-        a->result = f(ctx, _py2h(a->arg0), a->arg1, _py2h(a->arg2));
+        a->result = (f(ctx, _py2h(a->arg0), (a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_SSIZESSIZEOBJARGPROC: {
         HPyFunc_ssizessizeobjargproc f = (HPyFunc_ssizessizeobjargproc)func;
         _HPyFunc_args_SSIZESSIZEOBJARGPROC *a = (_HPyFunc_args_SSIZESSIZEOBJARGPROC*)args;
-        a->result = f(ctx, _py2h(a->arg0), a->arg1, a->arg2, _py2h(a->arg3));
+        a->result = (f(ctx, _py2h(a->arg0), (a->arg1), (a->arg2), _py2h(a->arg3)));
         return;
     }
     case HPyFunc_OBJOBJARGPROC: {
         HPyFunc_objobjargproc f = (HPyFunc_objobjargproc)func;
         _HPyFunc_args_OBJOBJARGPROC *a = (_HPyFunc_args_OBJOBJARGPROC*)args;
-        a->result = f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2));
+        a->result = (f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_FREEFUNC: {
         HPyFunc_freefunc f = (HPyFunc_freefunc)func;
         _HPyFunc_args_FREEFUNC *a = (_HPyFunc_args_FREEFUNC*)args;
-        f(ctx, a->arg0);
+        f(ctx, (a->arg0));
         return;
     }
     case HPyFunc_GETATTRFUNC: {
         HPyFunc_getattrfunc f = (HPyFunc_getattrfunc)func;
         _HPyFunc_args_GETATTRFUNC *a = (_HPyFunc_args_GETATTRFUNC*)args;
-        a->result = _h2py(f(ctx, _py2h(a->arg0), a->arg1));
+        a->result = _h2py(f(ctx, _py2h(a->arg0), (a->arg1)));
         return;
     }
     case HPyFunc_GETATTROFUNC: {
         HPyFunc_getattrofunc f = (HPyFunc_getattrofunc)func;
         _HPyFunc_args_GETATTROFUNC *a = (_HPyFunc_args_GETATTROFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0), _py2h(a->arg1)));
         return;
     }
     case HPyFunc_SETATTRFUNC: {
         HPyFunc_setattrfunc f = (HPyFunc_setattrfunc)func;
         _HPyFunc_args_SETATTRFUNC *a = (_HPyFunc_args_SETATTRFUNC*)args;
-        a->result = f(ctx, _py2h(a->arg0), a->arg1, _py2h(a->arg2));
+        a->result = (f(ctx, _py2h(a->arg0), (a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_SETATTROFUNC: {
         HPyFunc_setattrofunc f = (HPyFunc_setattrofunc)func;
         _HPyFunc_args_SETATTROFUNC *a = (_HPyFunc_args_SETATTROFUNC*)args;
-        a->result = f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2));
+        a->result = (f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_REPRFUNC: {
         HPyFunc_reprfunc f = (HPyFunc_reprfunc)func;
         _HPyFunc_args_REPRFUNC *a = (_HPyFunc_args_REPRFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0)));
         return;
     }
     case HPyFunc_HASHFUNC: {
         HPyFunc_hashfunc f = (HPyFunc_hashfunc)func;
         _HPyFunc_args_HASHFUNC *a = (_HPyFunc_args_HASHFUNC*)args;
-        a->result = f(ctx, _py2h(a->arg0));
+        a->result = (f(ctx, _py2h(a->arg0)));
         return;
     }
     case HPyFunc_RICHCMPFUNC: {
         HPyFunc_richcmpfunc f = (HPyFunc_richcmpfunc)func;
         _HPyFunc_args_RICHCMPFUNC *a = (_HPyFunc_args_RICHCMPFUNC*)args;
-        a->result = _h2py(f(ctx, _py2h(a->arg0), _py2h(a->arg1), a->arg2));
+        a->result = _h2py(f(ctx, _py2h(a->arg0), _py2h(a->arg1), (a->arg2)));
         return;
     }
     case HPyFunc_GETITERFUNC: {
         HPyFunc_getiterfunc f = (HPyFunc_getiterfunc)func;
         _HPyFunc_args_GETITERFUNC *a = (_HPyFunc_args_GETITERFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0)));
         return;
@@ -135,33 +147,33 @@
         _HPyFunc_args_DESCRGETFUNC *a = (_HPyFunc_args_DESCRGETFUNC*)args;
         a->result = _h2py(f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_DESCRSETFUNC: {
         HPyFunc_descrsetfunc f = (HPyFunc_descrsetfunc)func;
         _HPyFunc_args_DESCRSETFUNC *a = (_HPyFunc_args_DESCRSETFUNC*)args;
-        a->result = f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2));
+        a->result = (f(ctx, _py2h(a->arg0), _py2h(a->arg1), _py2h(a->arg2)));
         return;
     }
     case HPyFunc_GETTER: {
         HPyFunc_getter f = (HPyFunc_getter)func;
         _HPyFunc_args_GETTER *a = (_HPyFunc_args_GETTER*)args;
-        a->result = _h2py(f(ctx, _py2h(a->arg0), a->arg1));
+        a->result = _h2py(f(ctx, _py2h(a->arg0), (a->arg1)));
         return;
     }
     case HPyFunc_SETTER: {
         HPyFunc_setter f = (HPyFunc_setter)func;
         _HPyFunc_args_SETTER *a = (_HPyFunc_args_SETTER*)args;
-        a->result = f(ctx, _py2h(a->arg0), _py2h(a->arg1), a->arg2);
+        a->result = (f(ctx, _py2h(a->arg0), _py2h(a->arg1), (a->arg2)));
         return;
     }
     case HPyFunc_OBJOBJPROC: {
         HPyFunc_objobjproc f = (HPyFunc_objobjproc)func;
         _HPyFunc_args_OBJOBJPROC *a = (_HPyFunc_args_OBJOBJPROC*)args;
-        a->result = f(ctx, _py2h(a->arg0), _py2h(a->arg1));
+        a->result = (f(ctx, _py2h(a->arg0), _py2h(a->arg1)));
         return;
     }
     case HPyFunc_DESTRUCTOR: {
         HPyFunc_destructor f = (HPyFunc_destructor)func;
         _HPyFunc_args_DESTRUCTOR *a = (_HPyFunc_args_DESTRUCTOR*)args;
         f(ctx, _py2h(a->arg0));
         return;
```

### Comparing `hpy-0.0.4/hpy/universal/src/autogen_ctx_impl.h` & `hpy-0.9.0rc1/hpy/universal/src/autogen_ctx_impl.h`

 * *Files 4% similar despite different names*

```diff
@@ -6,74 +6,24 @@
    See also hpy.tools.autogen and hpy/tools/public_api.h
 
    Run this to regenerate:
        make autogen
 
 */
 
-HPyAPI_IMPL HPy ctx_Long_FromLong(HPyContext *ctx, long value)
-{
-    return _py2h(PyLong_FromLong(value));
-}
-
-HPyAPI_IMPL HPy ctx_Long_FromUnsignedLong(HPyContext *ctx, unsigned long value)
-{
-    return _py2h(PyLong_FromUnsignedLong(value));
-}
-
-HPyAPI_IMPL HPy ctx_Long_FromLongLong(HPyContext *ctx, long long v)
-{
-    return _py2h(PyLong_FromLongLong(v));
-}
-
-HPyAPI_IMPL HPy ctx_Long_FromUnsignedLongLong(HPyContext *ctx, unsigned long long v)
-{
-    return _py2h(PyLong_FromUnsignedLongLong(v));
-}
-
 HPyAPI_IMPL HPy ctx_Long_FromSize_t(HPyContext *ctx, size_t value)
 {
     return _py2h(PyLong_FromSize_t(value));
 }
 
 HPyAPI_IMPL HPy ctx_Long_FromSsize_t(HPyContext *ctx, HPy_ssize_t value)
 {
     return _py2h(PyLong_FromSsize_t(value));
 }
 
-HPyAPI_IMPL long ctx_Long_AsLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsLong(_h2py(h));
-}
-
-HPyAPI_IMPL unsigned long ctx_Long_AsUnsignedLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLong(_h2py(h));
-}
-
-HPyAPI_IMPL unsigned long ctx_Long_AsUnsignedLongMask(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongMask(_h2py(h));
-}
-
-HPyAPI_IMPL long long ctx_Long_AsLongLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsLongLong(_h2py(h));
-}
-
-HPyAPI_IMPL unsigned long long ctx_Long_AsUnsignedLongLong(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongLong(_h2py(h));
-}
-
-HPyAPI_IMPL unsigned long long ctx_Long_AsUnsignedLongLongMask(HPyContext *ctx, HPy h)
-{
-    return PyLong_AsUnsignedLongLongMask(_h2py(h));
-}
-
 HPyAPI_IMPL size_t ctx_Long_AsSize_t(HPyContext *ctx, HPy h)
 {
     return PyLong_AsSize_t(_h2py(h));
 }
 
 HPyAPI_IMPL HPy_ssize_t ctx_Long_AsSsize_t(HPyContext *ctx, HPy h)
 {
@@ -96,15 +46,15 @@
 }
 
 HPyAPI_IMPL double ctx_Float_AsDouble(HPyContext *ctx, HPy h)
 {
     return PyFloat_AsDouble(_h2py(h));
 }
 
-HPyAPI_IMPL HPy ctx_Bool_FromLong(HPyContext *ctx, long v)
+HPyAPI_IMPL HPy ctx_Bool_FromBool(HPyContext *ctx, bool v)
 {
     return _py2h(PyBool_FromLong(v));
 }
 
 HPyAPI_IMPL HPy_ssize_t ctx_Length(HPyContext *ctx, HPy h)
 {
     return PyObject_Length(_h2py(h));
@@ -286,17 +236,17 @@
 }
 
 HPyAPI_IMPL int ctx_Callable_Check(HPyContext *ctx, HPy h)
 {
     return PyCallable_Check(_h2py(h));
 }
 
-HPyAPI_IMPL void ctx_Err_SetString(HPyContext *ctx, HPy h_type, const char *message)
+HPyAPI_IMPL void ctx_Err_SetString(HPyContext *ctx, HPy h_type, const char *utf8_message)
 {
-    PyErr_SetString(_h2py(h_type), message);
+    PyErr_SetString(_h2py(h_type), utf8_message);
 }
 
 HPyAPI_IMPL void ctx_Err_SetObject(HPyContext *ctx, HPy h_type, HPy h_value)
 {
     PyErr_SetObject(_h2py(h_type), _h2py(h_value));
 }
 
@@ -321,27 +271,27 @@
 }
 
 HPyAPI_IMPL void ctx_Err_Clear(HPyContext *ctx)
 {
     PyErr_Clear();
 }
 
-HPyAPI_IMPL HPy ctx_Err_NewException(HPyContext *ctx, const char *name, HPy base, HPy dict)
+HPyAPI_IMPL HPy ctx_Err_NewException(HPyContext *ctx, const char *utf8_name, HPy base, HPy dict)
 {
-    return _py2h(PyErr_NewException(name, _h2py(base), _h2py(dict)));
+    return _py2h(PyErr_NewException(utf8_name, _h2py(base), _h2py(dict)));
 }
 
-HPyAPI_IMPL HPy ctx_Err_NewExceptionWithDoc(HPyContext *ctx, const char *name, const char *doc, HPy base, HPy dict)
+HPyAPI_IMPL HPy ctx_Err_NewExceptionWithDoc(HPyContext *ctx, const char *utf8_name, const char *utf8_doc, HPy base, HPy dict)
 {
-    return _py2h(PyErr_NewExceptionWithDoc(name, doc, _h2py(base), _h2py(dict)));
+    return _py2h(PyErr_NewExceptionWithDoc(utf8_name, utf8_doc, _h2py(base), _h2py(dict)));
 }
 
-HPyAPI_IMPL int ctx_Err_WarnEx(HPyContext *ctx, HPy category, const char *message, HPy_ssize_t stack_level)
+HPyAPI_IMPL int ctx_Err_WarnEx(HPyContext *ctx, HPy category, const char *utf8_message, HPy_ssize_t stack_level)
 {
-    return PyErr_WarnEx(_h2py(category), message, stack_level);
+    return PyErr_WarnEx(_h2py(category), utf8_message, stack_level);
 }
 
 HPyAPI_IMPL void ctx_Err_WriteUnraisable(HPyContext *ctx, HPy obj)
 {
     PyErr_WriteUnraisable(_h2py(obj));
 }
 
@@ -351,37 +301,37 @@
 }
 
 HPyAPI_IMPL HPy ctx_GetAttr(HPyContext *ctx, HPy obj, HPy name)
 {
     return _py2h(PyObject_GetAttr(_h2py(obj), _h2py(name)));
 }
 
-HPyAPI_IMPL HPy ctx_GetAttr_s(HPyContext *ctx, HPy obj, const char *name)
+HPyAPI_IMPL HPy ctx_GetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name)
 {
-    return _py2h(PyObject_GetAttrString(_h2py(obj), name));
+    return _py2h(PyObject_GetAttrString(_h2py(obj), utf8_name));
 }
 
 HPyAPI_IMPL int ctx_HasAttr(HPyContext *ctx, HPy obj, HPy name)
 {
     return PyObject_HasAttr(_h2py(obj), _h2py(name));
 }
 
-HPyAPI_IMPL int ctx_HasAttr_s(HPyContext *ctx, HPy obj, const char *name)
+HPyAPI_IMPL int ctx_HasAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name)
 {
-    return PyObject_HasAttrString(_h2py(obj), name);
+    return PyObject_HasAttrString(_h2py(obj), utf8_name);
 }
 
 HPyAPI_IMPL int ctx_SetAttr(HPyContext *ctx, HPy obj, HPy name, HPy value)
 {
     return PyObject_SetAttr(_h2py(obj), _h2py(name), _h2py(value));
 }
 
-HPyAPI_IMPL int ctx_SetAttr_s(HPyContext *ctx, HPy obj, const char *name, HPy value)
+HPyAPI_IMPL int ctx_SetAttr_s(HPyContext *ctx, HPy obj, const char *utf8_name, HPy value)
 {
-    return PyObject_SetAttrString(_h2py(obj), name, _h2py(value));
+    return PyObject_SetAttrString(_h2py(obj), utf8_name, _h2py(value));
 }
 
 HPyAPI_IMPL HPy ctx_GetItem(HPyContext *ctx, HPy obj, HPy key)
 {
     return _py2h(PyObject_GetItem(_h2py(obj), _h2py(key)));
 }
 
@@ -391,14 +341,19 @@
 }
 
 HPyAPI_IMPL int ctx_SetItem(HPyContext *ctx, HPy obj, HPy key, HPy value)
 {
     return PyObject_SetItem(_h2py(obj), _h2py(key), _h2py(value));
 }
 
+HPyAPI_IMPL int ctx_DelItem(HPyContext *ctx, HPy obj, HPy key)
+{
+    return PyObject_DelItem(_h2py(obj), _h2py(key));
+}
+
 HPyAPI_IMPL HPy ctx_Type(HPyContext *ctx, HPy obj)
 {
     return _py2h(PyObject_Type(_h2py(obj)));
 }
 
 HPyAPI_IMPL HPy ctx_Repr(HPyContext *ctx, HPy obj)
 {
@@ -446,27 +401,27 @@
 }
 
 HPyAPI_IMPL HPy_ssize_t ctx_Bytes_GET_SIZE(HPyContext *ctx, HPy h)
 {
     return PyBytes_GET_SIZE(_h2py(h));
 }
 
-HPyAPI_IMPL char *ctx_Bytes_AsString(HPyContext *ctx, HPy h)
+HPyAPI_IMPL const char *ctx_Bytes_AsString(HPyContext *ctx, HPy h)
 {
     return PyBytes_AsString(_h2py(h));
 }
 
-HPyAPI_IMPL char *ctx_Bytes_AS_STRING(HPyContext *ctx, HPy h)
+HPyAPI_IMPL const char *ctx_Bytes_AS_STRING(HPyContext *ctx, HPy h)
 {
     return PyBytes_AS_STRING(_h2py(h));
 }
 
-HPyAPI_IMPL HPy ctx_Bytes_FromString(HPyContext *ctx, const char *v)
+HPyAPI_IMPL HPy ctx_Bytes_FromString(HPyContext *ctx, const char *bytes)
 {
-    return _py2h(PyBytes_FromString(v));
+    return _py2h(PyBytes_FromString(bytes));
 }
 
 HPyAPI_IMPL HPy ctx_Unicode_FromString(HPyContext *ctx, const char *utf8)
 {
     return _py2h(PyUnicode_FromString(utf8));
 }
 
@@ -516,22 +471,32 @@
 }
 
 HPyAPI_IMPL HPy_UCS4 ctx_Unicode_ReadChar(HPyContext *ctx, HPy h, HPy_ssize_t index)
 {
     return PyUnicode_ReadChar(_h2py(h), index);
 }
 
-HPyAPI_IMPL HPy ctx_Unicode_DecodeASCII(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors)
+HPyAPI_IMPL HPy ctx_Unicode_DecodeASCII(HPyContext *ctx, const char *ascii, HPy_ssize_t size, const char *errors)
+{
+    return _py2h(PyUnicode_DecodeASCII(ascii, size, errors));
+}
+
+HPyAPI_IMPL HPy ctx_Unicode_DecodeLatin1(HPyContext *ctx, const char *latin1, HPy_ssize_t size, const char *errors)
 {
-    return _py2h(PyUnicode_DecodeASCII(s, size, errors));
+    return _py2h(PyUnicode_DecodeLatin1(latin1, size, errors));
 }
 
-HPyAPI_IMPL HPy ctx_Unicode_DecodeLatin1(HPyContext *ctx, const char *s, HPy_ssize_t size, const char *errors)
+HPyAPI_IMPL HPy ctx_Unicode_FromEncodedObject(HPyContext *ctx, HPy obj, const char *encoding, const char *errors)
 {
-    return _py2h(PyUnicode_DecodeLatin1(s, size, errors));
+    return _py2h(PyUnicode_FromEncodedObject(_h2py(obj), encoding, errors));
+}
+
+HPyAPI_IMPL HPy ctx_Unicode_Substring(HPyContext *ctx, HPy str, HPy_ssize_t start, HPy_ssize_t end)
+{
+    return _py2h(PyUnicode_Substring(_h2py(str), start, end));
 }
 
 HPyAPI_IMPL int ctx_List_Check(HPyContext *ctx, HPy h)
 {
     return PyList_Check(_h2py(h));
 }
 
@@ -551,27 +516,62 @@
 }
 
 HPyAPI_IMPL HPy ctx_Dict_New(HPyContext *ctx)
 {
     return _py2h(PyDict_New());
 }
 
+HPyAPI_IMPL HPy ctx_Dict_Keys(HPyContext *ctx, HPy h)
+{
+    return _py2h(PyDict_Keys(_h2py(h)));
+}
+
+HPyAPI_IMPL HPy ctx_Dict_Copy(HPyContext *ctx, HPy h)
+{
+    return _py2h(PyDict_Copy(_h2py(h)));
+}
+
 HPyAPI_IMPL int ctx_Tuple_Check(HPyContext *ctx, HPy h)
 {
     return PyTuple_Check(_h2py(h));
 }
 
-HPyAPI_IMPL HPy ctx_Import_ImportModule(HPyContext *ctx, const char *name)
+HPyAPI_IMPL int ctx_Slice_Unpack(HPyContext *ctx, HPy slice, HPy_ssize_t *start, HPy_ssize_t *stop, HPy_ssize_t *step)
 {
-    return _py2h(PyImport_ImportModule(name));
+    return PySlice_Unpack(_h2py(slice), start, stop, step);
+}
+
+HPyAPI_IMPL HPy ctx_Import_ImportModule(HPyContext *ctx, const char *utf8_name)
+{
+    return _py2h(PyImport_ImportModule(utf8_name));
+}
+
+HPyAPI_IMPL int ctx_Capsule_IsValid(HPyContext *ctx, HPy capsule, const char *utf8_name)
+{
+    return PyCapsule_IsValid(_h2py(capsule), utf8_name);
 }
 
 HPyAPI_IMPL void ctx_ReenterPythonExecution(HPyContext *ctx, HPyThreadState state)
 {
     PyEval_RestoreThread(_h2threads(state));
 }
 
 HPyAPI_IMPL HPyThreadState ctx_LeavePythonExecution(HPyContext *ctx)
 {
     return _threads2h(PyEval_SaveThread());
 }
 
+HPyAPI_IMPL HPy ctx_EvalCode(HPyContext *ctx, HPy code, HPy globals, HPy locals)
+{
+    return _py2h(PyEval_EvalCode(_h2py(code), _h2py(globals), _h2py(locals)));
+}
+
+HPyAPI_IMPL HPy ctx_ContextVar_New(HPyContext *ctx, const char *name, HPy default_value)
+{
+    return _py2h(PyContextVar_New(name, _h2py(default_value)));
+}
+
+HPyAPI_IMPL HPy ctx_ContextVar_Set(HPyContext *ctx, HPy context_var, HPy value)
+{
+    return _py2h(PyContextVar_Set(_h2py(context_var), _h2py(value)));
+}
+
```

### Comparing `hpy-0.0.4/hpy/universal/src/ctx_meth.c` & `hpy-0.9.0rc1/hpy/universal/src/ctx_meth.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include <Python.h>
 #include "ctx_meth.h"
 #include "hpy/runtime/ctx_type.h"
+#include "hpy/runtime/ctx_module.h"
 #include "handles.h"
 
 static void _buffer_h2py(HPyContext *ctx, const HPy_buffer *src, Py_buffer *dest)
 {
     dest->buf = src->buf;
     dest->obj = HPy_AsPyObject(ctx, src->obj);
     dest->len = src->len;
@@ -34,59 +35,59 @@
 }
 
 HPyAPI_IMPL void
 ctx_CallRealFunctionFromTrampoline(HPyContext *ctx, HPyFunc_Signature sig,
                                    void* (*func)(), void *args)
 {
     switch (sig) {
-    case HPyFunc_NOARGS: {
-        HPyFunc_noargs f = (HPyFunc_noargs)func;
-        _HPyFunc_args_NOARGS *a = (_HPyFunc_args_NOARGS*)args;
-        a->result = _h2py(f(ctx, _py2h(a->self)));
-        return;
-    }
-    case HPyFunc_O: {
-        HPyFunc_o f = (HPyFunc_o)func;
-        _HPyFunc_args_O *a = (_HPyFunc_args_O*)args;
-        a->result = _h2py(f(ctx, _py2h(a->self), _py2h(a->arg)));
-        return;
-    }
     case HPyFunc_VARARGS: {
         HPyFunc_varargs f = (HPyFunc_varargs)func;
         _HPyFunc_args_VARARGS *a = (_HPyFunc_args_VARARGS*)args;
-        Py_ssize_t nargs = PyTuple_GET_SIZE(a->args);
-        HPy *h_args = (HPy *)alloca(nargs * sizeof(HPy));
-        for (Py_ssize_t i = 0; i < nargs; i++) {
-            h_args[i] = _py2h(PyTuple_GET_ITEM(a->args, i));
+        HPy *h_args = (HPy *)alloca(a->nargs * sizeof(HPy));
+        for (HPy_ssize_t i = 0; i < a->nargs; i++) {
+            h_args[i] = _py2h(a->args[i]);
         }
-        a->result = _h2py(f(ctx, _py2h(a->self), h_args, nargs));
+        a->result = _h2py(f(ctx, _py2h(a->self), h_args, a->nargs));
         return;
     }
     case HPyFunc_KEYWORDS: {
         HPyFunc_keywords f = (HPyFunc_keywords)func;
         _HPyFunc_args_KEYWORDS *a = (_HPyFunc_args_KEYWORDS*)args;
-        Py_ssize_t nargs = PyTuple_GET_SIZE(a->args);
-        HPy *h_args = (HPy *)alloca(nargs * sizeof(HPy));
-        for (Py_ssize_t i = 0; i < nargs; i++) {
-            h_args[i] = _py2h(PyTuple_GET_ITEM(a->args, i));
+        size_t n_kwnames = a->kwnames != NULL ? PyTuple_GET_SIZE(a->kwnames) : 0;
+        size_t nargs = PyVectorcall_NARGS(a->nargsf);
+        size_t nargs_with_kw = nargs + n_kwnames;
+        HPy *h_args = (HPy *)alloca(nargs_with_kw * sizeof(HPy));
+        for (size_t i = 0; i < nargs_with_kw; i++) {
+            h_args[i] = _py2h(a->args[i]);
         }
-        a->result = _h2py(f(ctx, _py2h(a->self), h_args, nargs, _py2h(a->kw)));
+        a->result = _h2py(f(ctx, _py2h(a->self), h_args, nargs, _py2h(a->kwnames)));
         return;
     }
     case HPyFunc_INITPROC: {
         HPyFunc_initproc f = (HPyFunc_initproc)func;
         _HPyFunc_args_INITPROC *a = (_HPyFunc_args_INITPROC*)args;
         Py_ssize_t nargs = PyTuple_GET_SIZE(a->args);
         HPy *h_args = (HPy *)alloca(nargs * sizeof(HPy));
         for (Py_ssize_t i = 0; i < nargs; i++) {
             h_args[i] = _py2h(PyTuple_GET_ITEM(a->args, i));
         }
         a->result = f(ctx, _py2h(a->self), h_args, nargs, _py2h(a->kw));
         return;
     }
+    case HPyFunc_NEWFUNC: {
+        HPyFunc_newfunc f = (HPyFunc_newfunc)func;
+        _HPyFunc_args_NEWFUNC *a = (_HPyFunc_args_NEWFUNC*)args;
+        Py_ssize_t nargs = PyTuple_GET_SIZE(a->args);
+        HPy *h_args = (HPy *)alloca(nargs * sizeof(HPy));
+        for (Py_ssize_t i = 0; i < nargs; i++) {
+            h_args[i] = _py2h(PyTuple_GET_ITEM(a->args, i));
+        }
+        a->result = _h2py(f(ctx, _py2h(a->self), h_args, nargs, _py2h(a->kw)));
+        return;
+    }
     case HPyFunc_GETBUFFERPROC: {
         HPyFunc_getbufferproc f = (HPyFunc_getbufferproc)func;
         _HPyFunc_args_GETBUFFERPROC *a = (_HPyFunc_args_GETBUFFERPROC*)args;
         HPy_buffer hbuf;
         a->result = f(ctx, _py2h(a->self), &hbuf, a->flags);
         if (a->result < 0) {
             a->view->obj = NULL;
@@ -109,12 +110,27 @@
     case HPyFunc_TRAVERSEPROC: {
         HPyFunc_traverseproc f = (HPyFunc_traverseproc)func;
         _HPyFunc_args_TRAVERSEPROC *a = (_HPyFunc_args_TRAVERSEPROC*)args;
         a->result = call_traverseproc_from_trampoline(f, a->self,
                                                       a->visit, a->arg);
         return;
     }
+    case HPyFunc_CAPSULE_DESTRUCTOR: {
+        HPyFunc_Capsule_Destructor f = (HPyFunc_Capsule_Destructor)func;
+        PyObject *capsule = (PyObject *)args;
+        const char *name = PyCapsule_GetName(capsule);
+        f(name, PyCapsule_GetPointer(capsule, name),
+                PyCapsule_GetContext(capsule));
+        return;
+    }
+    case HPyFunc_MOD_CREATE: {
+            HPyFunc_unaryfunc f = (HPyFunc_unaryfunc)func;
+            _HPyFunc_args_UNARYFUNC *a = (_HPyFunc_args_UNARYFUNC*)args;
+            a->result = _h2py(f(ctx, _py2h(a->arg0)));
+            _HPyModule_CheckCreateSlotResult(&a->result);
+            return;
+    }
 #include "autogen_ctx_call.i"
     default:
         Py_FatalError("Unsupported HPyFunc_Signature in ctx_meth.c");
     }
 }
```

### Comparing `hpy-0.0.4/hpy/universal/src/ctx_misc.c` & `hpy-0.9.0rc1/hpy/universal/src/ctx_misc.c`

 * *Files 10% similar despite different names*

```diff
@@ -70,7 +70,14 @@
 }
 
 HPyAPI_IMPL void
 ctx_FatalError(HPyContext *ctx, const char *message)
 {
     Py_FatalError(message);
 }
+
+HPyAPI_IMPL int
+ctx_Type_IsSubtype(HPyContext *ctx, HPy sub, HPy type)
+{
+    return PyType_IsSubtype((PyTypeObject *)_h2py(sub),
+            (PyTypeObject *)_h2py(type));
+}
```

### Comparing `hpy-0.0.4/hpy/universal/src/ctx_misc.h` & `hpy-0.9.0rc1/hpy/universal/src/ctx_misc.h`

 * *Files 16% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 HPyAPI_IMPL void ctx_Field_Store(HPyContext *ctx, HPy target_object,
                                  HPyField *target_field, HPy h);
 HPyAPI_IMPL HPy ctx_Field_Load(HPyContext *ctx, HPy source_object,
                                HPyField source_field);
 HPyAPI_IMPL void ctx_Global_Store(HPyContext *ctx, HPyGlobal *global, HPy h);
 HPyAPI_IMPL HPy ctx_Global_Load(HPyContext *ctx, HPyGlobal global);
 HPyAPI_IMPL void ctx_FatalError(HPyContext *ctx, const char *message);
+HPyAPI_IMPL int ctx_Type_IsSubtype(HPyContext *ctx, HPy sub, HPy type);
 
 #endif /* HPY_CTX_MISC_H */
```

### Comparing `hpy-0.0.4/hpy/universal/src/handles.h` & `hpy-0.9.0rc1/hpy/universal/src/handles.h`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy/universal/src/misc_win32.h` & `hpy-0.9.0rc1/hpy/universal/src/misc_win32.h`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/hpy.egg-info/SOURCES.txt` & `hpy-0.9.0rc1/hpy.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,103 @@
 .gitattributes
 .gitignore
 .readthedocs.yml
+AUTHORS
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README-gdb.md
 README.md
 gdb-py.test
 pyproject.toml
+requirements-autogen.txt
 setup.py
+.github/FUNDING.yml
 .github/workflows/ci.yml
 .github/workflows/release-pypi.yml
+.github/workflows/valgrind-tests.yml
 c_test/Makefile
 c_test/acutest.h
 c_test/test_debug_handles.c
 c_test/test_stacktrace.c
 docs/Makefile
-docs/api.md
 docs/api.rst
 docs/changelog.rst
 docs/conf.py
 docs/debug-mode.rst
 docs/index.rst
 docs/leysin-2020-design-decisions.md
 docs/module-state.txt
 docs/overview.rst
 docs/porting-guide.rst
+docs/quickstart.rst
 docs/requirements.txt
+docs/trace-mode.rst
 docs/xxx-unsorted-notes.txt
 docs/_static/README.txt
 docs/_templates/README.txt
 docs/api-reference/argument-parsing.rst
 docs/api-reference/build-value.rst
+docs/api-reference/builder.rst
+docs/api-reference/formatting.rst
+docs/api-reference/function-index.rst
 docs/api-reference/helpers.rst
+docs/api-reference/hpy-call.rst
+docs/api-reference/hpy-ctx.rst
+docs/api-reference/hpy-dict.rst
+docs/api-reference/hpy-err.rst
+docs/api-reference/hpy-eval.rst
 docs/api-reference/hpy-field.rst
 docs/api-reference/hpy-gil.rst
 docs/api-reference/hpy-global.rst
+docs/api-reference/hpy-object.rst
+docs/api-reference/hpy-type.rst
 docs/api-reference/index.rst
+docs/api-reference/inline-helpers.rst
+docs/api-reference/public-api.rst
+docs/api-reference/structseq.rst
+docs/contributing/index.rst
 docs/examples/debug-example.py
 docs/examples/tests.py
+docs/examples/trace-example.py
+docs/examples/hpytype-example/builtin_type.c
+docs/examples/hpytype-example/setup.py
+docs/examples/hpytype-example/simple_type.c
+docs/examples/hpytype-example/simple_type.rst
 docs/examples/mixed-example/mixed.c
 docs/examples/mixed-example/setup.py
+docs/examples/quickstart/quickstart.c
+docs/examples/quickstart/setup.py
 docs/examples/simple-example/setup.py
 docs/examples/simple-example/simple.c
+docs/examples/snippets/hpycall.c
+docs/examples/snippets/hpyinit.c
 docs/examples/snippets/hpyvarargs.c
+docs/examples/snippets/legacyinit.c
 docs/examples/snippets/setup.py
 docs/examples/snippets/snippets.c
+docs/misc/embedding.rst
 docs/misc/index.rst
-docs/misc/str-builder-api.rst
+docs/porting-example/index.rst
+docs/porting-example/steps/.gitignore
+docs/porting-example/steps/conftest.py
+docs/porting-example/steps/setup00.py
+docs/porting-example/steps/setup01.py
+docs/porting-example/steps/setup02.py
+docs/porting-example/steps/setup03.py
+docs/porting-example/steps/step_00_c_api.c
+docs/porting-example/steps/step_00_c_api.rst
+docs/porting-example/steps/step_01_hpy_legacy.c
+docs/porting-example/steps/step_01_hpy_legacy.rst
+docs/porting-example/steps/step_02_hpy_legacy.c
+docs/porting-example/steps/step_02_hpy_legacy.rst
+docs/porting-example/steps/step_03_hpy_final.c
+docs/porting-example/steps/step_03_hpy_final.rst
+docs/porting-example/steps/test_porting_example.py
 hpy.egg-info/PKG-INFO
 hpy.egg-info/SOURCES.txt
 hpy.egg-info/dependency_links.txt
 hpy.egg-info/entry_points.txt
 hpy.egg-info/requires.txt
 hpy.egg-info/top_level.txt
 hpy/debug/__init__.py
@@ -68,70 +113,94 @@
 hpy/debug/src/debug_handles.c
 hpy/debug/src/debug_internal.h
 hpy/debug/src/dhqueue.c
 hpy/debug/src/memprotect.c
 hpy/debug/src/stacktrace.c
 hpy/debug/src/include/hpy_debug.h
 hpy/devel/__init__.py
+hpy/devel/abitag.py
 hpy/devel/version.py
 hpy/devel/include/hpy.h
 hpy/devel/include/hpy/autogen_hpyfunc_declare.h
 hpy/devel/include/hpy/autogen_hpyslot.h
 hpy/devel/include/hpy/cpy_types.h
 hpy/devel/include/hpy/hpydef.h
+hpy/devel/include/hpy/hpyexports.h
 hpy/devel/include/hpy/hpyfunc.h
 hpy/devel/include/hpy/hpymodule.h
 hpy/devel/include/hpy/hpytype.h
 hpy/devel/include/hpy/inline_helpers.h
 hpy/devel/include/hpy/macros.h
 hpy/devel/include/hpy/version.h
 hpy/devel/include/hpy/cpython/autogen_api_impl.h
+hpy/devel/include/hpy/cpython/autogen_ctx.h
 hpy/devel/include/hpy/cpython/autogen_hpyfunc_trampolines.h
 hpy/devel/include/hpy/cpython/hpyfunc_trampolines.h
 hpy/devel/include/hpy/cpython/misc.h
+hpy/devel/include/hpy/forbid_python_h/Python.h
 hpy/devel/include/hpy/runtime/argparse.h
 hpy/devel/include/hpy/runtime/buildvalue.h
 hpy/devel/include/hpy/runtime/ctx_funcs.h
+hpy/devel/include/hpy/runtime/ctx_module.h
 hpy/devel/include/hpy/runtime/ctx_type.h
+hpy/devel/include/hpy/runtime/format.h
 hpy/devel/include/hpy/runtime/helpers.h
+hpy/devel/include/hpy/runtime/structseq.h
 hpy/devel/include/hpy/universal/autogen_ctx.h
 hpy/devel/include/hpy/universal/autogen_hpyfunc_trampolines.h
 hpy/devel/include/hpy/universal/autogen_trampolines.h
 hpy/devel/include/hpy/universal/hpyfunc_trampolines.h
 hpy/devel/include/hpy/universal/misc_trampolines.h
 hpy/devel/src/runtime/argparse.c
 hpy/devel/src/runtime/buildvalue.c
 hpy/devel/src/runtime/ctx_bytes.c
 hpy/devel/src/runtime/ctx_call.c
+hpy/devel/src/runtime/ctx_capsule.c
+hpy/devel/src/runtime/ctx_contextvar.c
 hpy/devel/src/runtime/ctx_err.c
+hpy/devel/src/runtime/ctx_eval.c
 hpy/devel/src/runtime/ctx_listbuilder.c
+hpy/devel/src/runtime/ctx_long.c
 hpy/devel/src/runtime/ctx_module.c
 hpy/devel/src/runtime/ctx_object.c
 hpy/devel/src/runtime/ctx_tracker.c
 hpy/devel/src/runtime/ctx_tuple.c
 hpy/devel/src/runtime/ctx_tuplebuilder.c
 hpy/devel/src/runtime/ctx_type.c
+hpy/devel/src/runtime/format.c
 hpy/devel/src/runtime/helpers.c
+hpy/devel/src/runtime/structseq.c
 hpy/tools/include_path.py
 hpy/tools/autogen/__main__.py
+hpy/tools/autogen/autogen.h
 hpy/tools/autogen/autogenfile.py
 hpy/tools/autogen/conf.py
 hpy/tools/autogen/ctx.py
 hpy/tools/autogen/debug.py
+hpy/tools/autogen/doc.py
 hpy/tools/autogen/hpyfunc.py
 hpy/tools/autogen/hpyslot.py
 hpy/tools/autogen/parse.py
 hpy/tools/autogen/public_api.h
 hpy/tools/autogen/pypy.py
+hpy/tools/autogen/trace.py
 hpy/tools/autogen/trampolines.py
 hpy/tools/autogen/testing/__init__.py
 hpy/tools/autogen/testing/test_autogen.py
 hpy/tools/autogen/testing/test_hpyfunc.py
 hpy/tools/valgrind/hpy.supp
 hpy/tools/valgrind/python.supp
+hpy/trace/__init__.py
+hpy/trace/src/_tracemod.c
+hpy/trace/src/autogen_trace_ctx_init.h
+hpy/trace/src/autogen_trace_func_table.c
+hpy/trace/src/autogen_trace_wrappers.c
+hpy/trace/src/trace_ctx.c
+hpy/trace/src/trace_internal.h
+hpy/trace/src/include/hpy_trace.h
 hpy/universal/src/api.h
 hpy/universal/src/autogen_ctx_call.i
 hpy/universal/src/autogen_ctx_def.h
 hpy/universal/src/autogen_ctx_impl.h
 hpy/universal/src/ctx.c
 hpy/universal/src/ctx_meth.c
 hpy/universal/src/ctx_meth.h
@@ -144,15 +213,14 @@
 microbench/_valgrind_build.py
 microbench/conftest.py
 microbench/pytest_valgrind.sh
 microbench/setup.py
 microbench/test_microbench.py
 microbench/src/cpy_simple.c
 microbench/src/hpy_simple.c
-proof-of-concept/Makefile
 proof-of-concept/pof.c
 proof-of-concept/pofcpp.cpp
 proof-of-concept/requirements.txt
 proof-of-concept/setup.py
 proof-of-concept/test_pof.py
 proof-of-concept/test_pof.sh
 proof-of-concept/pofpackage/bar.cpp
@@ -160,33 +228,46 @@
 test/__init__.py
 test/check_py27_compat.py
 test/conftest.py
 test/support.py
 test/test_00_basic.py
 test/test_argparse.py
 test/test_call.py
+test/test_capsule.py
+test/test_capsule_legacy.py
+test/test_contextvar.py
 test/test_cpy_compat.py
+test/test_eval.py
 test/test_helpers.py
 test/test_hpybuildvalue.py
 test/test_hpybytes.py
 test/test_hpydict.py
 test/test_hpyerr.py
 test/test_hpyfield.py
 test/test_hpyglobal.py
 test/test_hpyimport.py
 test/test_hpylist.py
 test/test_hpylong.py
 test/test_hpymodule.py
+test/test_hpyslice.py
+test/test_hpystructseq.py
 test/test_hpytuple.py
 test/test_hpytype.py
 test/test_hpytype_legacy.py
 test/test_hpyunicode.py
 test/test_importing.py
+test/test_legacy_forbidden.py
 test/test_number.py
 test/test_object.py
 test/test_slots.py
 test/test_slots_legacy.py
 test/test_support.py
 test/test_tracker.py
+test/debug/test_builder_invalid.py
 test/debug/test_charptr.py
+test/debug/test_context_reuse.py
 test/debug/test_handles_invalid.py
-test/debug/test_handles_leak.py
+test/debug/test_handles_leak.py
+test/debug/test_misc.py
+test/hpy_devel/test_abitag.py
+test/hpy_devel/test_distutils.py
+test/trace/test_trace.py
```

### Comparing `hpy-0.0.4/microbench/_valgrind_build.py` & `hpy-0.9.0rc1/microbench/_valgrind_build.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/microbench/conftest.py` & `hpy-0.9.0rc1/microbench/conftest.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/microbench/src/cpy_simple.c` & `hpy-0.9.0rc1/microbench/src/cpy_simple.c`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/microbench/src/hpy_simple.c` & `hpy-0.9.0rc1/microbench/src/hpy_simple.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,83 @@
 #include "hpy.h"
 
 /* module-level functions */
 
-HPyDef_METH(noargs, "noargs", noargs_impl, HPyFunc_NOARGS)
+HPyDef_METH(noargs, "noargs", HPyFunc_NOARGS)
 static HPy noargs_impl(HPyContext *ctx, HPy self)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_METH(onearg, "onearg", onearg_impl, HPyFunc_O)
+HPyDef_METH(onearg, "onearg", HPyFunc_O)
 static HPy onearg_impl(HPyContext *ctx, HPy self, HPy arg)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_METH(varargs, "varargs", varargs_impl, HPyFunc_VARARGS)
-static HPy varargs_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(varargs, "varargs", HPyFunc_VARARGS)
+static HPy varargs_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_METH(call_with_tuple, "call_with_tuple", call_with_tuple_impl, HPyFunc_VARARGS)
-static HPy call_with_tuple_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(call_with_tuple, "call_with_tuple", HPyFunc_VARARGS)
+static HPy call_with_tuple_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     HPy f, f_args;
     if (nargs != 2) {
         HPyErr_SetString(ctx, ctx->h_TypeError, "call_with_tuple requires two arguments");
         return HPy_NULL;
     }
     f = args[0];
     f_args = args[1];
     return HPy_CallTupleDict(ctx, f, f_args, HPy_NULL);
 }
 
-HPyDef_METH(call_with_tuple_and_dict, "call_with_tuple_and_dict", call_with_tuple_and_dict_impl, HPyFunc_VARARGS)
-static HPy call_with_tuple_and_dict_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(call_with_tuple_and_dict, "call_with_tuple_and_dict", HPyFunc_VARARGS)
+static HPy call_with_tuple_and_dict_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     HPy f, f_args, f_kw;
     if (nargs != 3) {
         HPyErr_SetString(ctx, ctx->h_TypeError, "call_with_tuple_and_dict requires three arguments");
         return HPy_NULL;
     }
     f = args[0];
     f_args = args[1];
     f_kw = args[2];
     return HPy_CallTupleDict(ctx, f, f_args, f_kw);
 }
 
-HPyDef_METH(allocate_int, "allocate_int", allocate_int_impl, HPyFunc_NOARGS)
+HPyDef_METH(allocate_int, "allocate_int", HPyFunc_NOARGS)
 static HPy allocate_int_impl(HPyContext *ctx, HPy self)
 {
     return HPyLong_FromLong(ctx, 2048);
 }
 
-HPyDef_METH(allocate_tuple, "allocate_tuple", allocate_tuple_impl, HPyFunc_NOARGS)
+HPyDef_METH(allocate_tuple, "allocate_tuple", HPyFunc_NOARGS)
 static HPy allocate_tuple_impl(HPyContext *ctx, HPy self)
 {
-    //return Py_BuildValue("ii", 2048, 2049);
-    HPyErr_SetString(ctx, ctx->h_Exception, "HPy_BuildValue not implemented yet");
-    return HPy_NULL;
+    return HPy_BuildValue(ctx, "ii", 2048, 2049);
 }
 
 
 /* Foo type */
 
 typedef struct {
-    PyObject_HEAD
+    long x;
+    long y;
 } FooObject;
 
-HPyDef_SLOT(Foo_getitem, Foo_getitem_impl, HPy_sq_item)
+HPyDef_SLOT(Foo_getitem, HPy_sq_item)
 static HPy Foo_getitem_impl(HPyContext *ctx, HPy self, HPy_ssize_t i)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_SLOT(Foo_len, Foo_len_impl, HPy_sq_length)
+HPyDef_SLOT(Foo_len, HPy_sq_length)
 static HPy_ssize_t Foo_len_impl(HPyContext *ctx, HPy self)
 {
     return 42;
 }
 
 
 // note that we can reuse the same HPyDef for both module-level and type-level
@@ -100,39 +99,37 @@
     .flags = HPy_TPFLAGS_DEFAULT,
     .defines = foo_defines
 };
 
 
 /* Module defines */
 
+HPyDef_SLOT(init_hpy_simple, HPy_mod_exec)
+static int init_hpy_simple_impl(HPyContext *ctx, HPy m)
+{
+    HPy h_Foo = HPyType_FromSpec(ctx, &Foo_spec, NULL);
+    if (HPy_IsNull(h_Foo))
+        return -1;
+    HPy_SetAttr_s(ctx, m, "Foo", h_Foo);
+    HPy_SetAttr_s(ctx, m, "HTFoo", h_Foo);
+    return 0;
+}
+
 static HPyDef *module_defines[] = {
     &noargs,
     &onearg,
     &varargs,
     &call_with_tuple,
     &call_with_tuple_and_dict,
     &allocate_int,
     &allocate_tuple,
+    &init_hpy_simple,
     NULL
 };
 
-
 static HPyModuleDef moduledef = {
-    .name = "hpy_simple",
     .doc = "HPy microbenchmarks",
-    .size = -1,
+    .size = 0,
     .defines = module_defines,
 };
 
-HPy_MODINIT(hpy_simple)
-static HPy init_hpy_simple_impl(HPyContext *ctx)
-{
-    HPy m = HPyModule_Create(ctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-    HPy h_Foo = HPyType_FromSpec(ctx, &Foo_spec, NULL);
-    if (HPy_IsNull(h_Foo))
-      return HPy_NULL;
-    HPy_SetAttr_s(ctx, m, "Foo", h_Foo);
-    HPy_SetAttr_s(ctx, m, "HTFoo", h_Foo);
-    return m;
-}
+HPy_MODINIT(hpy_simple, moduledef)
```

### Comparing `hpy-0.0.4/microbench/test_microbench.py` & `hpy-0.9.0rc1/microbench/test_microbench.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,16 +78,14 @@
 
     def test_allocate_int(self, simple, timer, N):
         with timer:
             for i in range(N):
                 simple.allocate_int()
 
     def test_allocate_tuple(self, api, simple, timer, N):
-        if api == 'hpy':
-            pytest.skip('Missing HPy_BuildValue')
         with timer:
             for i in range(N):
                 simple.allocate_tuple()
 
 
 class TestType:
     """ Compares the performance of operations on types.
@@ -96,14 +94,25 @@
 
         * cpy: a static type
         * hpy: a heap type (HPy only has heap types)
 
         The type is named `simple.Foo` in both cases.
     """
 
+    def test_allocate_obj(self, simple, timer, N):
+        import gc
+        Foo = simple.Foo
+        objs = [None] * N
+        gc.collect()
+        with timer:
+            for i in range(N):
+                objs[i] = Foo()
+            del objs
+            gc.collect()
+
     def test_method_lookup(self, simple, timer, N):
         obj = simple.Foo()
         with timer:
             for i in range(N):
                 # note: here we are NOT calling it, we want to measure just
                 # the lookup
                 obj.noargs
@@ -147,14 +156,35 @@
 
 class TestHeapType:
     """ Compares the performance of operations on heap types.
 
         The type is named `simple.HTFoo` and is a heap type in all cases.
     """
 
+    def test_allocate_obj_and_survive(self, simple, timer, N):
+        import gc
+        HTFoo = simple.HTFoo
+        objs = [None] * N
+        gc.collect()
+        with timer:
+            for i in range(N):
+                objs[i] = HTFoo()
+            del objs
+            gc.collect()
+
+    def test_allocate_obj_and_die(self, simple, timer, N):
+        import gc
+        HTFoo = simple.HTFoo
+        gc.collect()
+        with timer:
+            for i in range(N):
+                obj = HTFoo()
+                obj.onearg(None)
+            gc.collect()
+
     def test_method_lookup(self, simple, timer, N):
         obj = simple.HTFoo()
         with timer:
             for i in range(N):
                 # note: here we are NOT calling it, we want to measure just
                 # the lookup
                 obj.noargs
```

### Comparing `hpy-0.0.4/proof-of-concept/pof.c` & `hpy-0.9.0rc1/proof-of-concept/pof.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 #include "hpy.h"
 #include <stdio.h>
 
-HPyDef_METH(do_nothing, "do_nothing", do_nothing_impl, HPyFunc_NOARGS)
+HPyDef_METH(do_nothing, "do_nothing", HPyFunc_NOARGS)
 static HPy do_nothing_impl(HPyContext *ctx, HPy self)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_METH(double_obj, "double", double_obj_impl, HPyFunc_O)
+HPyDef_METH(double_obj, "double", HPyFunc_O)
 static HPy double_obj_impl(HPyContext *ctx, HPy self, HPy obj)
 {
     return HPy_Add(ctx, obj, obj);
 }
 
-HPyDef_METH(add_ints, "add_ints", add_ints_impl, HPyFunc_VARARGS)
-static HPy add_ints_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(add_ints, "add_ints", HPyFunc_VARARGS)
+static HPy add_ints_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     long a, b;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 
-HPyDef_METH(add_ints_kw, "add_ints_kw", add_ints_kw_impl, HPyFunc_KEYWORDS)
-static HPy add_ints_kw_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs,
-                            HPy kw)
+HPyDef_METH(add_ints_kw, "add_ints_kw", HPyFunc_KEYWORDS)
+static HPy add_ints_kw_impl(HPyContext *ctx, HPy self, const HPy *args,
+                           size_t nargs, HPy kwnames)
 {
     long a, b;
     const char* kwlist[] = {"a", "b", NULL};
-    if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kw, "ll", kwlist, &a, &b))
+    if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kwnames, "ll",
+                              kwlist, &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 
 typedef struct {
     double x;
     double y;
 } PointObject;
 
 HPyType_HELPERS(PointObject)
 
-HPyDef_SLOT(Point_new, Point_new_impl, HPy_tp_new)
-static HPy Point_new_impl (HPyContext *ctx, HPy cls, HPy *args,
-                           HPy_ssize_t nargs, HPy Kw)
+HPyDef_SLOT(Point_new, HPy_tp_new)
+static HPy Point_new_impl (HPyContext *ctx, HPy cls, const HPy *args,
+                           HPy_ssize_t nargs, HPy kwnames)
 {
     double x, y;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "dd", &x, &y))
         return HPy_NULL;
     PointObject *point;
     HPy h_point = HPy_New(ctx, cls, &point);
     if (HPy_IsNull(h_point))
         return HPy_NULL;
     point->x = x;
     point->y = y;
     return h_point;
 }
 
-HPyDef_SLOT(Point_repr, Point_repr_impl, HPy_tp_repr)
+HPyDef_SLOT(Point_repr, HPy_tp_repr)
 static HPy Point_repr_impl(HPyContext *ctx, HPy self)
 {
     PointObject *point = PointObject_AsStruct(ctx, self);
     char msg[256];
     snprintf(msg, 256, "Point(%g, %g)", point->x, point->y);
     return HPyUnicode_FromString(ctx, msg);
     //return HPyUnicode_FromFormat("Point(%g, %g)", point->x, point->y);
@@ -75,34 +76,34 @@
 static HPyType_Spec point_type_spec = {
     .name = "pof.Point",
     .basicsize = sizeof(PointObject),
     .flags = HPy_TPFLAGS_DEFAULT,
     .defines = point_type_defines
 };
 
+HPyDef_SLOT(mod_exec, HPy_mod_exec)
+static int mod_exec_impl(HPyContext *ctx, HPy m)
+{
+    HPy h_point_type = HPyType_FromSpec(ctx, &point_type_spec, NULL);
+    if (HPy_IsNull(h_point_type))
+        return -1;
+    HPy_SetAttr_s(ctx, m, "Point", h_point_type);
+    HPy_Close(ctx, h_point_type);
+    return 0;
+}
+
 static HPyDef *module_defines[] = {
     &do_nothing,
     &double_obj,
     &add_ints,
     &add_ints_kw,
+    &mod_exec,
     NULL
 };
+
 static HPyModuleDef moduledef = {
-    .name = "pof",
     .doc = "HPy Proof of Concept",
-    .size = -1,
+    .size = 0,
     .defines = module_defines
 };
 
-HPy_MODINIT(pof)
-static HPy init_pof_impl(HPyContext *ctx)
-{
-    HPy m, h_point_type;
-    m = HPyModule_Create(ctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-    h_point_type = HPyType_FromSpec(ctx, &point_type_spec, NULL);
-    if (HPy_IsNull(h_point_type))
-      return HPy_NULL;
-    HPy_SetAttr_s(ctx, m, "Point", h_point_type);
-    return m;
-}
+HPy_MODINIT(pof, moduledef)
```

### Comparing `hpy-0.0.4/proof-of-concept/pofcpp.cpp` & `hpy-0.9.0rc1/proof-of-concept/pofcpp.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 #include "hpy.h"
 #include <stdio.h>
 
-HPyDef_METH(do_nothing, "do_nothing", do_nothing_impl, HPyFunc_NOARGS)
+HPyDef_METH(do_nothing, "do_nothing", HPyFunc_NOARGS)
 static HPy do_nothing_impl(HPyContext *ctx, HPy self)
 {
     return HPy_Dup(ctx, ctx->h_None);
 }
 
-HPyDef_METH(double_obj, "double", double_obj_impl, HPyFunc_O)
+HPyDef_METH(double_obj, "double", HPyFunc_O)
 static HPy double_obj_impl(HPyContext *ctx, HPy self, HPy obj)
 {
     return HPy_Add(ctx, obj, obj);
 }
 
-HPyDef_METH(add_ints, "add_ints", add_ints_impl, HPyFunc_VARARGS)
-static HPy add_ints_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+HPyDef_METH(add_ints, "add_ints", HPyFunc_VARARGS)
+static HPy add_ints_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
 {
     long a, b;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 
-HPyDef_METH(add_ints_kw, "add_ints_kw", add_ints_kw_impl, HPyFunc_KEYWORDS)
-static HPy add_ints_kw_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs,
-                            HPy kw)
+HPyDef_METH(add_ints_kw, "add_ints_kw", HPyFunc_KEYWORDS)
+static HPy add_ints_kw_impl(HPyContext *ctx, HPy self, const HPy *args,
+                            size_t nargs, HPy kwnames)
 {
     long a, b;
     const char* kwlist[] = {"a", "b", NULL};
-    if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kw, "ll", kwlist, &a, &b))
+    if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kwnames, "ll",
+                              kwlist, &a, &b))
         return HPy_NULL;
     return HPyLong_FromLong(ctx, a+b);
 }
 
 typedef struct {
     double x;
     double y;
 } PointObject;
 
 HPyType_HELPERS(PointObject)
 
-HPyDef_SLOT(Point_new, Point_new_impl, HPy_tp_new)
-static HPy Point_new_impl (HPyContext *ctx, HPy cls, HPy *args,
-                           HPy_ssize_t nargs, HPy Kw)
+HPyDef_SLOT(Point_new, HPy_tp_new)
+static HPy Point_new_impl (HPyContext *ctx, HPy cls, const HPy *args,
+                           HPy_ssize_t nargs, HPy kwnames)
 {
     double x, y;
     if (!HPyArg_Parse(ctx, NULL, args, nargs, "dd", &x, &y))
         return HPy_NULL;
     PointObject *point;
     HPy h_point = HPy_New(ctx, cls, &point);
     if (HPy_IsNull(h_point))
         return HPy_NULL;
     point->x = x;
     point->y = y;
     return h_point;
 }
 
-HPyDef_SLOT(Point_repr, Point_repr_impl, HPy_tp_repr)
+HPyDef_SLOT(Point_repr, HPy_tp_repr)
 static HPy Point_repr_impl(HPyContext *ctx, HPy self)
 {
     PointObject *point = PointObject_AsStruct(ctx, self);
     char msg[256];
     snprintf(msg, 256, "Point(%g, %g)", point->x, point->y);
     return HPyUnicode_FromString(ctx, msg);
     //return HPyUnicode_FromFormat("Point(%g, %g)", point->x, point->y);
@@ -68,49 +69,49 @@
 
 
 static HPyDef *point_type_defines[] = {
     &Point_new,
     &Point_repr,
     NULL
 };
+
 static HPyType_Spec point_type_spec = {
     .name = "pofcpp.Point",
     .basicsize = sizeof(PointObject),
     .flags = HPy_TPFLAGS_DEFAULT,
     .defines = point_type_defines
 };
 
+HPyDef_SLOT(mod_exec, HPy_mod_exec)
+static int mod_exec_impl(HPyContext *ctx, HPy m)
+{
+    HPy h_point_type = HPyType_FromSpec(ctx, &point_type_spec, NULL);
+    if (HPy_IsNull(h_point_type))
+      return -1;
+    HPy_SetAttr_s(ctx, m, "Point", h_point_type);
+    HPy_Close(ctx, h_point_type);
+    return 0;
+}
+
 static HPyDef *module_defines[] = {
     &do_nothing,
     &double_obj,
     &add_ints,
     &add_ints_kw,
+    &mod_exec,
     NULL
 };
 static HPyModuleDef moduledef = {
-    .name = "pofcpp",
     .doc = "HPy c++ Proof of Concept",
-    .size = -1,
+    .size = 0,
     .defines = module_defines
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
-HPy_MODINIT(pofcpp)
-static HPy init_pofcpp_impl(HPyContext *ctx)
-{
-    HPy m, h_point_type;
-    m = HPyModule_Create(ctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-    h_point_type = HPyType_FromSpec(ctx, &point_type_spec, NULL);
-    if (HPy_IsNull(h_point_type))
-      return HPy_NULL;
-    HPy_SetAttr_s(ctx, m, "Point", h_point_type);
-    return m;
-}
+HPy_MODINIT(pofcpp, moduledef)
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `hpy-0.0.4/proof-of-concept/pofpackage/bar.cpp` & `hpy-0.9.0rc1/proof-of-concept/pofpackage/bar.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -11,44 +11,35 @@
 
         int boo(HPyContext *ctx, HPy obj)
         {
             return foo + HPyLong_AsLong(ctx, obj);
         }
 };
 
-HPyDef_METH(hello, "hello", hello_impl, HPyFunc_O)
+HPyDef_METH(hello, "hello", HPyFunc_O)
 static HPy hello_impl(HPyContext *ctx, HPy self, HPy obj)
 {
     Bar b(21);
     return HPyLong_FromLong(ctx, b.boo(ctx, obj));
 }
 
 
 static HPyDef *module_defines[] = {
     &hello,
     NULL
 };
 static HPyModuleDef moduledef = {
-    .name = "bar",
     .doc = "HPy C++ Proof of Concept",
-    .size = -1,
+    .size = 0,
     .defines = module_defines
 };
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 
-HPy_MODINIT(bar)
-static HPy init_bar_impl(HPyContext *ctx)
-{
-    HPy m;
-    m = HPyModule_Create(ctx, &moduledef);
-    if (HPy_IsNull(m))
-        return HPy_NULL;
-    return m;
-}
+HPy_MODINIT(bar, moduledef)
 
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `hpy-0.0.4/proof-of-concept/setup.py` & `hpy-0.9.0rc1/proof-of-concept/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     ]
 else:
     compile_extra_args = ['-Werror']
 
 
 setup(
     name="hpy-pof",
+    packages = ['pofpackage'],
+    zip_safe=False,
     hpy_ext_modules=[
         Extension('pof', 
                     sources=['pof.c'],
                     extra_compile_args=compile_extra_args),
         Extension('pofpackage.foo',
                     sources=['pofpackage/foo.c'],
                     extra_compile_args=compile_extra_args),
```

### Comparing `hpy-0.0.4/proof-of-concept/test_pof.py` & `hpy-0.9.0rc1/proof-of-concept/test_pof.py`

 * *Files identical despite different names*

### Comparing `hpy-0.0.4/proof-of-concept/test_pof.sh` & `hpy-0.9.0rc1/proof-of-concept/test_pof.sh`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 #!/bin/bash
 set -e
 ROOT=`pwd` # we expect this script to be run from the repo root
 
+# Allow the caller to override the Python runtime used
+PYTHON=${PYTHON:-python3}
+
 _install_hpy() {
     echo "Installing hpy"
     # at the moment this install hpy.devel and hpy.universal. Eventually, we
     # will want to split those into two separate packages
     local PYTHON="$1"
     pushd ${ROOT}
+    ${PYTHON} -m pip install -U pip
     ${PYTHON} -m pip install wheel
     ${PYTHON} -m pip install .
     popd
 }
 
 _test_pof() {
     echo "==== testing pof ===="
     # this assumes that pof is already installed, e.g. after calling
     # wheel or setup_py_install
-    python -m pip install pytest pytest-azurepipelines
+    ${PYTHON} -m pip install pytest pytest-azurepipelines
     cd proof-of-concept
-    python -m pytest
+    ${PYTHON} -m pytest
 }
 
 _build_wheel() {
     HPY_ABI="$1"
     local VENV="venv/wheel_builder_$HPY_ABI"
     # we use this venv just to build the wheel, and then we install the wheel
     # in the currently active virtualenv
     echo "Create venv: $VENV"
-    python -m venv "$VENV"
+    ${PYTHON} -m venv "$VENV"
     local PY_BUILDER="`pwd`/$VENV/bin/python3"
     if [ -x "`pwd`/$VENV/Scripts/python.exe" ]
     then
         # Set the correct python executable for Windows
         PY_BUILDER="`pwd`/$VENV/Scripts/python.exe"
     fi
     echo
@@ -83,69 +87,69 @@
     clean
     echo "=== testing setup.py bdist_wheel" $HPY_ABI "==="
     _build_wheel "$HPY_ABI"
     WHEEL=`ls proof-of-concept/dist/*.whl`
     echo "Wheel created: ${WHEEL}"
     echo
     echo "Create venv: $VENV"
-    python -m venv "$VENV"
+    ${PYTHON} -m venv "$VENV"
     if [ -e "$VENV/bin/activate" ] ; then
         source "$VENV/bin/activate"
     else
         source "$VENV/Scripts/activate"
     fi
-    _install_hpy python
+    _install_hpy ${PYTHON}
     echo "Installing wheel"
-    python -m pip install $WHEEL
+    ${PYTHON} -m pip install $WHEEL
     echo
     _test_pof
 }
 
 setup_py_install() {
     # install proof-of-concept using setup.py install and run tests
     HPY_ABI="$1"
     VENV="venv/setup_py_install_$HPY_ABI"
     clean
     echo "=== testing setup.py --hpy-abi=$HPY_ABI install ==="
     echo "Create venv: $VENV"
-    python -m venv "$VENV"
+    ${PYTHON} -m venv "$VENV"
     if [ -e "$VENV/bin/activate" ] ; then
         source "$VENV/bin/activate"
     else
         source "$VENV/Scripts/activate"
     fi
-    _install_hpy python
+    _install_hpy ${PYTHON}
     echo
     echo "Running setup.py"
     pushd proof-of-concept
-    python setup.py --hpy-abi="$HPY_ABI" install
+    ${PYTHON} setup.py --hpy-abi="$HPY_ABI" install
     popd
     echo
     _test_pof
 }
 
 setup_py_build_ext_inplace() {
     # install proof-of-concept using setup.py install and run tests
     HPY_ABI="$1"
     VENV="venv/setup_py_build_ext_inplace_$HPY_ABI"
     clean
     echo "=== testing setup.py --hpy-abi=$HPY_ABI build_ext --inplace ==="
     echo "Create venv: $VENV"
-    python -m venv "$VENV"
+    ${PYTHON} -m venv "$VENV"
     if [ -e "$VENV/bin/activate" ] ; then
         source "$VENV/bin/activate"
     else
         source "$VENV/Scripts/activate"
     fi
-    _install_hpy python
+    _install_hpy ${PYTHON}
     echo
     echo "Running setup.py"
     pushd proof-of-concept
-    echo python is $(which python)
-    python setup.py --hpy-abi="$HPY_ABI" build_ext --inplace
+    echo python is $(which ${PYTHON})
+    ${PYTHON} setup.py --hpy-abi="$HPY_ABI" build_ext --inplace
     popd
     echo
     _test_pof
 }
 
 # ======== main code =======
```

### Comparing `hpy-0.0.4/test/check_py27_compat.py` & `hpy-0.9.0rc1/test/check_py27_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 import traceback
 import py
 
 ROOT = py.path.local(__file__).join('..', '..')
 TEST_DIRS = [ROOT / 'test', ROOT / 'test' / 'debug']
 
 # PyPy does NOT import these files using py2
-PY3_ONLY = ['test_support.py', 'test_handles_invalid.py', 'test_handles_leak.py']
+PY3_ONLY = ['test_support.py',
+            'test_handles_invalid.py',
+            'test_handles_leak.py',
+            'test_builder_invalid.py']
 
 def try_import(name):
     try:
         if isinstance(name, py.path.local):
             print('Trying to import %s... ' % ROOT.bestrelpath(name), end='')
             name.pyimport()
         else:
```

### Comparing `hpy-0.0.4/test/conftest.py` & `hpy-0.9.0rc1/test/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,85 @@
 import pytest
 from .support import ExtensionCompiler, DefaultExtensionTemplate,\
-    PythonSubprocessRunner, HPyDebugCapture
+    PythonSubprocessRunner, HPyDebugCapture, make_hpy_abi_fixture
 from hpy.debug.leakdetector import LeakDetector
+from pathlib import Path
 
 IS_VALGRIND_RUN = False
 
 def pytest_addoption(parser):
     parser.addoption(
         "--compiler-v", action="store_true",
         help="Print to stdout the commands used to invoke the compiler")
     parser.addoption(
         "--subprocess-v", action="store_true",
-        help="Print to stdout the stdout and stderr of Python subprocesses"
+        help="Print to stdout the stdout and stderr of Python subprocesses "
              "executed via run_python_subprocess")
+    parser.addoption(
+        "--dump-dir",
+        help="Enables dump mode and specifies where to write generated test "
+             "sources. This will then only generate the sources and skip "
+             "evaluation of the tests.")
+    parser.addoption(
+        '--reuse-venv', action="store_true",
+        help="Development only: reuse the venv for test_distutils.py instead of "
+             "creating a new one for every test")
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_configure(config):
     global IS_VALGRIND_RUN
     IS_VALGRIND_RUN = config.pluginmanager.hasplugin('valgrind_checker')
     config.addinivalue_line(
         "markers", "syncgc: Mark tests that rely on a synchronous GC."
     )
 
+# this is the default set of hpy_abi for all the tests. Individual files and
+# classes can override it.
+hpy_abi = make_hpy_abi_fixture('default')
+
+
 @pytest.fixture(scope='session')
 def hpy_devel(request):
     from hpy.devel import HPyDevel
     return HPyDevel()
 
-@pytest.fixture(params=['cpython', 'universal', 'debug'])
-def hpy_abi(request):
-    abi = request.param
-    if abi == 'debug':
-        with LeakDetector():
-            yield abi
+@pytest.fixture
+def leakdetector(hpy_abi):
+    """
+    Automatically detect leaks when the hpy_abi == 'debug'
+    """
+    if 'debug' in hpy_abi:
+        with LeakDetector() as ld:
+            yield ld
     else:
-        yield abi
+        yield None
 
 @pytest.fixture
 def ExtensionTemplate():
     return DefaultExtensionTemplate
 
-
 @pytest.fixture
 def compiler(request, tmpdir, hpy_devel, hpy_abi, ExtensionTemplate):
     compiler_verbose = request.config.getoption('--compiler-v')
+    dump_dir = request.config.getoption('--dump-dir')
+    if dump_dir:
+        # Test-specific dump dir in format: dump_dir/[mod_][cls_]func
+        qname_parts = []
+        if request.module:
+            qname_parts.append(request.module.__name__)
+        if request.cls:
+            qname_parts.append(request.cls.__name__)
+        qname_parts.append(request.function.__name__)
+        test_dump_dir = "_".join(qname_parts).replace(".", "_")
+        dump_dir = Path(dump_dir).joinpath(test_dump_dir)
+        dump_dir.mkdir(parents=True, exist_ok=True)
     return ExtensionCompiler(tmpdir, hpy_devel, hpy_abi,
                              compiler_verbose=compiler_verbose,
+                             dump_dir=dump_dir,
                              ExtensionTemplate=ExtensionTemplate)
 
 
 @pytest.fixture(scope="session")
 def fatal_exit_code(request):
     import sys
     return {
```

### Comparing `hpy-0.0.4/test/debug/test_charptr.py` & `hpy-0.9.0rc1/test/debug/test_charptr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,181 @@
-from test.support import SUPPORTS_SYS_EXECUTABLE
 import os
 import pytest
+from test.support import SUPPORTS_SYS_EXECUTABLE, SUPPORTS_MEM_PROTECTION
 
 # Tests detection of usage of char pointers associated with invalid already
 # closed handles. For now, the debug mode does not provide any hook for this
 # error, so we have to run the tests from subprocess and check the return code.
 
-SUPPORTS_MEM_PROTECTION = os.name == 'posix' and \
-                          '_HPY_DEBUG_FORCE_DEFAULT_MEM_PROTECT' not in os.environ
-
 @pytest.fixture
 def hpy_abi():
     from hpy.debug import LeakDetector
     with LeakDetector():
         yield "debug"
 
 
 @pytest.mark.skipif(not SUPPORTS_SYS_EXECUTABLE, reason="needs subprocess")
 def test_charptr_use_after_implicit_arg_handle_close(compiler, python_subprocess):
     mod = compiler.compile_module("""
         const char *keep;
 
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-        static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+        HPyDef_METH(f, "f", HPyFunc_VARARGS)
+        static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t n)
         {
+            if (n != 2) {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "expected exactly two arguments");
+                return HPy_NULL;
+            }
+            long mode = HPyLong_AsLong(ctx, args[1]);
+            if (mode == -1)
+                return HPy_NULL;
+
             HPy_ssize_t size;
-            keep = HPyUnicode_AsUTF8AndSize(ctx, arg, &size);
+            if (mode == 0) {
+                keep = HPyUnicode_AsUTF8AndSize(ctx, args[0], &size);
+            } else if (mode == 1) {
+                keep = HPyBytes_AsString(ctx, args[0]);
+            } else if (mode == 2) {
+                keep = HPyBytes_AS_STRING(ctx, args[0]);
+            } else {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "invalid mode");
+                return HPy_NULL;
+            }
             return HPy_Dup(ctx, ctx->h_None);
         }
 
-        HPyDef_METH(g, "g", g_impl, HPyFunc_NOARGS)
+        HPyDef_METH(g, "g", HPyFunc_NOARGS)
         static HPy g_impl(HPyContext *ctx, HPy self)
         {
             return HPyUnicode_FromString(ctx, keep);
         }
 
         @EXPORT(f)
         @EXPORT(g)
         @INIT
     """)
-    if SUPPORTS_MEM_PROTECTION:
-        code = "mod.f('leak me!'); mod.g()"
-    else:
-        code = "mod.f('leak me!'); assert mod.g() == 'leak me!'"
-    result = python_subprocess.run(mod, code)
-    assert result.returncode != 0
-    assert result.stdout == b""
-    if SUPPORTS_MEM_PROTECTION:
-        assert result.stderr == b""
-    else:
-        # The garbage we override the data with will cause this error
-        assert b"UnicodeDecodeError" in result.stderr
+    content = "'use after close me!'"
+    bcontent = 'b' + content
+    for mode, msg in enumerate((content, bcontent, bcontent)):
+        if SUPPORTS_MEM_PROTECTION and False:
+            code = "mod.f({}, {}); mod.g()".format(msg, mode)
+        else:
+            code = "mod.f({0}, {1}); assert mod.g() == str({0})".format(msg, mode)
+        result = python_subprocess.run(mod, code)
+        assert result.returncode != 0
+        assert result.stdout == b""
+        if SUPPORTS_MEM_PROTECTION:
+            assert result.stderr == b""
+        else:
+            # The garbage we override the data with will cause this error
+            assert b"UnicodeDecodeError" in result.stderr
 
 
 @pytest.mark.skipif(not SUPPORTS_SYS_EXECUTABLE, reason="needs subprocess")
 def test_charptr_use_after_handle_close(compiler, python_subprocess):
     mod = compiler.compile_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-        static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+        HPyDef_METH(f, "f", HPyFunc_VARARGS)
+        static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t n)
         {
-            HPy arg_dup = HPy_Dup(ctx, arg);
+            if (n != 2) {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "expected exactly two arguments");
+                return HPy_NULL;
+            }
+            long mode = HPyLong_AsLong(ctx, args[1]);
+            if (mode == -1)
+                return HPy_NULL;
+
+            HPy arg_dup = HPy_Dup(ctx, args[0]);
             HPy_ssize_t size;
-            const char *keep = HPyUnicode_AsUTF8AndSize(ctx, arg_dup, &size);
+            const char *keep;
+            if (mode == 0) {
+                keep = HPyUnicode_AsUTF8AndSize(ctx, arg_dup, &size);
+            } else if (mode == 1) {
+                keep = HPyBytes_AsString(ctx, arg_dup);
+            } else if (mode == 2) {
+                keep = HPyBytes_AS_STRING(ctx, arg_dup);
+            } else {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "invalid mode");
+                return HPy_NULL;
+            }
             HPy_Close(ctx, arg_dup);
             return HPyUnicode_FromString(ctx, keep);
         }
 
         @EXPORT(f)
         @INIT
     """)
-    if SUPPORTS_MEM_PROTECTION:
-        code = "mod.f('use after close me!')"
-    else:
-        code = "assert mod.f('use after close me!') == 'use after close me!'"
-    result = python_subprocess.run(mod, code)
-    assert result.returncode != 0
-    assert result.stdout == b""
-    if SUPPORTS_MEM_PROTECTION:
-        assert result.stderr == b""
-    else:
-        # The garbage we override the data with will cause this error
-        assert b"UnicodeDecodeError" in result.stderr
+    content = "'use after close me!'"
+    bcontent = "b" + content
+    for mode, msg in enumerate((content, bcontent, bcontent)):
+        if SUPPORTS_MEM_PROTECTION:
+            code = "mod.f({}, {})".format(msg, mode)
+        else:
+            code = "assert mod.f({0}, {1}) == str({0})".format(msg, mode)
+        result = python_subprocess.run(mod, code)
+        assert result.returncode != 0
+        assert result.stdout == b""
+        if SUPPORTS_MEM_PROTECTION:
+            assert result.stderr == b""
+        else:
+            # The garbage we override the data with will cause this error
+            assert b"UnicodeDecodeError" in result.stderr
 
 
 @pytest.mark.skipif(not SUPPORTS_MEM_PROTECTION, reason=
-                    "Could be implemented by checking the contents on "
-                    "close, but long term it would be better to provide"
-                    "proper protection on Windows in the future")
+                    "Could be implemented by checking the contents on close.")
 @pytest.mark.skipif(not SUPPORTS_SYS_EXECUTABLE, reason="needs subprocess")
 def test_charptr_write_ptr(compiler, python_subprocess):
     mod = compiler.compile_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-        static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+        HPyDef_METH(f, "f", HPyFunc_VARARGS)
+        static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t n)
         {
+            if (n != 2) {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "expected exactly two arguments");
+                return HPy_NULL;
+            }
+            long mode = HPyLong_AsLong(ctx, args[1]);
+            if (mode == -1)
+                return HPy_NULL;
+
             HPy_ssize_t size;
-            char *keep = (char*) HPyUnicode_AsUTF8AndSize(ctx, arg, &size);
-            keep[0] = 'a';
+            char *data;
+            if (mode == 0) {
+                data = (char *)HPyUnicode_AsUTF8AndSize(ctx, args[0], &size);
+            } else if (mode == 1) {
+                data = (char *)HPyBytes_AsString(ctx, args[0]);
+            } else if (mode == 2) {
+                data = (char *)HPyBytes_AS_STRING(ctx, args[0]);
+            } else {
+                HPyErr_SetString(ctx, ctx->h_ValueError, "invalid mode");
+                return HPy_NULL;
+            }
+            // write to read-only memory
+            data[0] = 'a';
             return HPy_Dup(ctx, ctx->h_None);
         }
 
         @EXPORT(f)
         @INIT
     """)
-    result = python_subprocess.run(mod, "mod.f('try writing me!');")
-    assert result.returncode != 0
-    assert result.stdout == b""
-    assert result.stderr == b""
+    content = "'try writing me!'"
+    bcontent = "b" + content
+    for mode, msg in enumerate((content, bcontent, bcontent)):
+        result = python_subprocess.run(mod, "mod.f({}, {});".format(msg, mode))
+        assert result.returncode != 0
+        assert result.stdout == b""
+        assert result.stderr == b""
 
 
 def test_charptr_correct_usage(compiler):
     mod = compiler.make_module("""
         #include <string.h>
         #include <stdio.h>
 
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy arg_dup = HPy_Dup(ctx, arg);
             HPy_ssize_t size;
             const char *keep = HPyUnicode_AsUTF8AndSize(ctx, arg_dup, &size);
             char *copy = (char*) malloc(size + 1);
             memcpy(copy, keep, size + 1);
@@ -132,28 +190,28 @@
     """)
     assert mod.f('I wont be leaked!') == 'I wont be leaked!';
 
 
 def test_charptr_limit_stress_test(compiler):
     from hpy.universal import _debug
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy_ssize_t size;
             HPyUnicode_AsUTF8AndSize(ctx, arg, &size);
             if (size == 0) {
                 return HPy_NULL;
             }
             return HPy_Dup(ctx, ctx->h_None);
         }
 
         // Dummy function just to force handle creation, but should not create
         // any raw data attached to those handles
-        HPyDef_METH(g, "g", g_impl, HPyFunc_O)
+        HPyDef_METH(g, "g", HPyFunc_O)
         static HPy g_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             int len = HPyLong_AsLong(ctx, arg);
             for (int i = 0; i < len; ++i) {
                 HPy h = HPyLong_FromLong(ctx, i);
                 HPy_Close(ctx, h);
             }
```

### Comparing `hpy-0.0.4/test/debug/test_handles_invalid.py` & `hpy-0.9.0rc1/test/debug/test_handles_invalid.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with LeakDetector():
         yield "debug"
 
 
 def test_no_invalid_handle(compiler, hpy_debug_capture):
     # Basic sanity check that valid code does not trigger any error reports
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy x = HPyLong_FromLong(ctx, 42);
             HPy y = HPyLong_FromLong(ctx, 2);
             HPy arg_dup = HPy_Dup(ctx, arg);
             HPy_Close(ctx, y);
             HPy b = HPy_Dup(ctx, x);
@@ -31,55 +31,55 @@
     assert mod.f("hello") == 42
     assert mod.f("world") == 42
     assert hpy_debug_capture.invalid_handles_count == 0
 
 
 def test_cant_use_closed_handle(compiler, hpy_debug_capture):
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O, .doc="double close")
+        HPyDef_METH(f, "f", HPyFunc_O, .doc="double close")
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy h = HPy_Dup(ctx, arg);
             HPy_Close(ctx, h);
             HPy_Close(ctx, h); // double close
             return HPy_Dup(ctx, ctx->h_None);
         }
 
-        HPyDef_METH(g, "g", g_impl, HPyFunc_O, .doc="use after close")
+        HPyDef_METH(g, "g", HPyFunc_O, .doc="use after close")
         static HPy g_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy h = HPy_Dup(ctx, arg);
             HPy_Close(ctx, h);
             return HPy_Repr(ctx, h);
         }
 
-        HPyDef_METH(h, "h", h_impl, HPyFunc_O, .doc="closing argument")
+        HPyDef_METH(h, "h", HPyFunc_O, .doc="closing argument")
         static HPy h_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             // Argument is implicitly closed by the caller
             HPy_Close(ctx, arg);
             return HPy_Dup(ctx, ctx->h_None);
         }
 
-        HPyDef_METH(f_noargs, "f_noargs", f_noargs_impl, HPyFunc_NOARGS, .doc="returns arg w/o dupping it")
+        HPyDef_METH(f_noargs, "f_noargs", HPyFunc_NOARGS, .doc="returns arg w/o dupping it")
         static HPy f_noargs_impl(HPyContext *ctx, HPy self)
         {
             // should be: return HPy_Dup(ctx, self);
             return self;
         }
 
-        HPyDef_METH(f0, "f0", f0_impl, HPyFunc_O, .doc="returns arg w/o dupping it")
+        HPyDef_METH(f0, "f0", HPyFunc_O, .doc="returns arg w/o dupping it")
         static HPy f0_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             // should be: return HPy_Dup(ctx, arg);
             return arg;
         }
 
-        HPyDef_METH(f_varargs, "f_varargs", f_varargs_impl, HPyFunc_VARARGS, .doc="returns arg w/o dupping it")
-        static HPy f_varargs_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+        HPyDef_METH(f_varargs, "f_varargs", HPyFunc_VARARGS, .doc="returns arg w/o dupping it")
+        static HPy f_varargs_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
         {
             // should be: return HPy_Dup(ctx, args[0]);
             return args[0];
         }
 
         @EXPORT(f)
         @EXPORT(g)
@@ -106,22 +106,22 @@
         assert hpy_debug_capture.invalid_handles_count == 6
 
 
 def test_keeping_and_reusing_argument_handle(compiler, hpy_debug_capture):
     mod = compiler.make_module("""
         HPy keep;
 
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             keep = arg;
             return HPy_Dup(ctx, ctx->h_None);
         }
 
-        HPyDef_METH(g, "g", g_impl, HPyFunc_NOARGS)
+        HPyDef_METH(g, "g", HPyFunc_NOARGS)
         static HPy g_impl(HPyContext *ctx, HPy self)
         {
             HPy_ssize_t len = HPy_Length(ctx, keep);
             return HPyLong_FromSsize_t(ctx, len);
         }
 
         @EXPORT(f)
@@ -131,26 +131,70 @@
     s = "hello leaks!"
     mod.f(s)
     assert hpy_debug_capture.invalid_handles_count == 0
     assert mod.g() == len(s)
     assert hpy_debug_capture.invalid_handles_count == 1
 
 
+def test_return_ctx_constant_without_dup(compiler, python_subprocess, fatal_exit_code):
+    # Since this puts the context->h_None into an inconsistent state, we run
+    # this test in a subprocess and check fatal error instead
+    if not SUPPORTS_SYS_EXECUTABLE:
+        pytest.skip("no sys.executable")
+
+    mod = compiler.compile_module("""
+        HPyDef_METH(f, "f", HPyFunc_NOARGS)
+        static HPy f_impl(HPyContext *ctx, HPy self)
+        {
+            return ctx->h_None;
+        }
+
+        @EXPORT(f)
+        @INIT
+    """)
+    result = python_subprocess.run(mod, "mod.f();")
+    assert result.returncode == fatal_exit_code
+    assert b"Invalid usage of already closed handle" in result.stderr
+
+
+def test_close_ctx_constant(compiler, python_subprocess, fatal_exit_code):
+    # Since this puts the context->h_True into an inconsistent state, we run
+    # this test in a subprocess and check fatal error instead
+    if not SUPPORTS_SYS_EXECUTABLE:
+        pytest.skip("no sys.executable")
+
+    mod = compiler.compile_module("""
+        HPyDef_METH(f, "f", HPyFunc_NOARGS)
+        static HPy f_impl(HPyContext *ctx, HPy self)
+        {
+            HPy_Close(ctx, ctx->h_True);
+            return HPy_Dup(ctx, ctx->h_False);
+        }
+
+        @EXPORT(f)
+        @INIT
+    """)
+    result = python_subprocess.run(mod, "mod.f();")
+    assert result.returncode == fatal_exit_code
+    assert b"Invalid usage of already closed handle" in result.stderr
+
+
 def test_invalid_handle_crashes_python_if_no_hook(compiler, python_subprocess, fatal_exit_code):
     if not SUPPORTS_SYS_EXECUTABLE:
         pytest.skip("no sys.executable")
 
     mod = compiler.compile_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O, .doc="double close")
+        HPyDef_METH(f, "f", HPyFunc_O, .doc="double close")
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy h = HPy_Dup(ctx, arg);
             HPy_Close(ctx, h);
             HPy_Close(ctx, h); // double close
             return HPy_Dup(ctx, ctx->h_None);
         }
 
         @EXPORT(f)
         @INIT
     """)
     result = python_subprocess.run(mod, "mod.f(42);")
-    assert result.returncode == fatal_exit_code
+    assert result.returncode == fatal_exit_code
+    assert b"Invalid usage of already closed handle" in result.stderr
```

### Comparing `hpy-0.0.4/test/debug/test_handles_leak.py` & `hpy-0.9.0rc1/test/debug/test_handles_leak.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     else:
         yield
 
 
 def make_leak_module(compiler):
     # for convenience
     return compiler.make_module("""
-        HPyDef_METH(leak, "leak", leak_impl, HPyFunc_O)
+        HPyDef_METH(leak, "leak", HPyFunc_O)
         static HPy leak_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy_Dup(ctx, arg); // leak!
             return HPy_Dup(ctx, ctx->h_None);
         }
         @EXPORT(leak)
         @INIT
@@ -40,15 +40,15 @@
 def test_debug_ctx_name(compiler):
     # this is very similar to the one in test_00_basic, but:
     #   1. by doing the same here, we ensure that we are actually using
     #      the debug ctx in these tests
     #   2. in pypy we run HPyTest with only hpy_abi==universal, so this
     #      tests something which is NOT tested by test_00_basic
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+        HPyDef_METH(f, "f", HPyFunc_NOARGS)
         static HPy f_impl(HPyContext *ctx, HPy self)
         {
             return HPyUnicode_FromString(ctx, ctx->name);
         }
 
         @EXPORT(f)
         @INIT
@@ -70,15 +70,15 @@
     leaks2 = [dh.obj for dh in leaks2]
     assert leaks1 == ['hello', 'world', 'a younger leak']
     assert leaks2 == ['a younger leak']
 
 def test_leak_from_method(compiler):
     from hpy.universal import _debug
     mod = compiler.make_module("""
-        HPyDef_METH(Dummy_leak, "leak", Dummy_leak_impl, HPyFunc_O)
+        HPyDef_METH(Dummy_leak, "leak", HPyFunc_O)
         static HPy Dummy_leak_impl(HPyContext *ctx, HPy self, HPy arg) {
             HPy_Dup(ctx, arg); // leak!
             return HPy_Dup(ctx, ctx->h_None);
         }
         static HPyDef *Dummy_defines[] = {
             &Dummy_leak,
             NULL
@@ -188,15 +188,15 @@
     assert _debug.get_open_handles(gen) == []
     assert h_hello in _debug.get_closed_handles()
     assert repr(h_hello).startswith("<DebugHandle 0x%x CLOSED>" % h_hello.id)
 
 def test_closed_handles_queue_max_size(compiler):
     from hpy.universal import _debug
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             return HPy_Dup(ctx, ctx->h_None);
         }
         @EXPORT(f)
         @INIT
     """)
@@ -227,20 +227,20 @@
         assert n5 == n1+7
     finally:
         _debug.set_closed_handles_queue_max_size(old_size)
 
 def test_reuse_closed_handles(compiler):
     from hpy.universal import _debug
     mod = compiler.make_module("""
-        HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+        HPyDef_METH(f, "f", HPyFunc_O)
         static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             return HPy_Dup(ctx, ctx->h_None);
         }
-        HPyDef_METH(leak, "leak", leak_impl, HPyFunc_O)
+        HPyDef_METH(leak, "leak", HPyFunc_O)
         static HPy leak_impl(HPyContext *ctx, HPy self, HPy arg)
         {
             HPy_Dup(ctx, arg); // leak!
             return HPy_Dup(ctx, ctx->h_None);
         }
         @EXPORT(f)
         @EXPORT(leak)
```

### Comparing `hpy-0.0.4/test/support.py` & `hpy-0.9.0rc1/test/support.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,119 @@
 import os, sys
-import pytest, py
+from filelock import FileLock
+import pytest
+from pathlib import Path
 import re
+import subprocess
 import textwrap
+import distutils
 
 PY2 = sys.version_info[0] == 2
 
+HPY_ROOT = Path(__file__).parent.parent
+LOCK = FileLock(HPY_ROOT / ".hpy.lock")
+
 # True if `sys.executable` is set to a value that allows a Python equivalent to
 # the current Python to be launched via, e.g., `python_subprocess.run(...)`.
 # By default is `True` if sys.executable is set to a true value.
 SUPPORTS_SYS_EXECUTABLE = bool(getattr(sys, "executable", None))
 # True if we are running on the CPython debug build
 IS_PYTHON_DEBUG_BUILD = hasattr(sys, 'gettotalrefcount')
 
+# pytest marker to run tests only on linux
+ONLY_LINUX = pytest.mark.skipif(sys.platform!='linux', reason='linux only')
+
+SUPPORTS_MEM_PROTECTION = '_HPY_DEBUG_FORCE_DEFAULT_MEM_PROTECT' not in os.environ
+
 def reindent(s, indent):
     s = textwrap.dedent(s)
     return ''.join(' '*indent + line if line.strip() else line
         for line in s.splitlines(True))
 
+def atomic_run(*args, **kwargs):
+    with LOCK:
+        return subprocess.run(*args, **kwargs)
+
+
+def make_hpy_abi_fixture(ABIs, class_fixture=False):
+    """
+    Make an hpy_abi fixture.
+
+    conftest.py defines a default hpy_abi for all tests, but individual files
+    and classes can override the set of ABIs they want to use. The indented
+    usage is the following:
+
+    # at the top of a file
+    hpy_abi = make_hpy_abi_fixture(['universal', 'debug'])
+
+    # in a class
+    class TestFoo(HPyTest):
+        hpy_abi = make_hpy_abi_fixture('with hybrid', class_fixture=True)
+    """
+    if ABIs == 'default':
+        ABIs = ['cpython', 'universal', 'debug']
+    elif ABIs == 'with hybrid':
+        ABIs = ['cpython', 'hybrid', 'hybrid+debug']
+    elif isinstance(ABIs, list):
+        pass
+    else:
+        raise ValueError("ABIs must be 'default', 'with hybrid' "
+                         "or a list of strings. Got: %s" % ABIs)
+
+    if class_fixture:
+        @pytest.fixture(params=ABIs)
+        def hpy_abi(self, request):
+            abi = request.param
+            yield abi
+    else:
+        @pytest.fixture(params=ABIs)
+        def hpy_abi(request):
+            abi = request.param
+            yield abi
+
+    return hpy_abi
+
+
 class DefaultExtensionTemplate(object):
 
-    INIT_TEMPLATE = textwrap.dedent("""
+    INIT_TEMPLATE = textwrap.dedent(
+    """
     static HPyDef *moduledefs[] = {
         %(defines)s
         NULL
     };
     %(globals_defs)s
     static HPyModuleDef moduledef = {
-        .name = "%(name)s",
         .doc = "some test for hpy",
-        .size = -1,
+        .size = 0,
         .legacy_methods = %(legacy_methods)s,
         .defines = moduledefs,
         %(globals_field)s
     };
 
-    HPy_MODINIT(%(name)s)
-    static HPy init_%(name)s_impl(HPyContext *ctx)
-    {
-        HPy m = HPy_NULL;
-        m = HPyModule_Create(ctx, &moduledef);
-        if (HPy_IsNull(m))
-            goto MODINIT_ERROR;
-        %(init_types)s
-        return m;
-
-        MODINIT_ERROR:
-
-        if (!HPy_IsNull(m))
-            HPy_Close(ctx, m);
-        return HPy_NULL;
-    }
+    HPy_MODINIT(%(name)s, moduledef)
     """)
 
+    INIT_TEMPLATE_WITH_TYPES_INIT = textwrap.dedent(
+        """
+        HPyDef_SLOT(generated_init, HPy_mod_exec)
+        static int generated_init_impl(HPyContext *ctx, HPy m)
+        {
+            // Shouldn't really happen, but jut to silence the unused label warning
+            if (HPy_IsNull(m))
+                goto MODINIT_ERROR;
+
+            %(init_types)s
+            return 0;
+
+            MODINIT_ERROR:
+            return -1;
+        }
+        """ + INIT_TEMPLATE)
+
     r_marker = re.compile(r"^\s*@([A-Za-z_]+)(\(.*\))?$")
 
     def __init__(self, src, name):
         self.src = textwrap.dedent(src)
         self.name = name
         self.defines_table = None
         self.legacy_methods = 'NULL'
@@ -102,18 +160,23 @@
         globals_defs = ''
         globals_field = ''
         if self.globals_table:
             globals_defs = \
                 textwrap.dedent('''
                 static HPyGlobal *module_globals[] = {
                     %s
+                    NULL
                 };''') % NL_INDENT.join(self.globals_table)
             globals_field = '.globals = module_globals'
 
-        exp = self.INIT_TEMPLATE % {
+        template = self.INIT_TEMPLATE
+        if init_types:
+            template = self.INIT_TEMPLATE_WITH_TYPES_INIT
+            self.EXPORT('generated_init')
+        exp = template % {
             'legacy_methods': self.legacy_methods,
             'defines': NL_INDENT.join(self.defines_table),
             'init_types': init_types,
             'name': self.name,
             'globals_defs': globals_defs,
             'globals_field': globals_field}
         self.output.append(exp)
@@ -146,14 +209,17 @@
             {func}(ctx, m);
             if (HPyErr_Occurred(ctx))
                 goto MODINIT_ERROR;
             """
         src = reindent(src, 4)
         self.type_table.append(src.format(func=func))
 
+    def HPy_MODINIT(self, mod):
+        return "HPy_MODINIT({}, {})".format(self.name, mod)
+
 
 class Spec(object):
     def __init__(self, name, origin):
         self.name = name
         self.origin = origin
 
 
@@ -161,44 +227,51 @@
     def __init__(self, name, so_file):
         self.name = name
         self.so_filename = so_file
 
 
 class ExtensionCompiler:
     def __init__(self, tmpdir, hpy_devel, hpy_abi, compiler_verbose=False,
+                 dump_dir=None,
                  ExtensionTemplate=DefaultExtensionTemplate,
                  extra_include_dirs=None):
         """
         hpy_devel is an instance of HPyDevel which specifies where to find
         include/, runtime/src, etc. Usually it will point to hpy/devel/, but
         alternate implementations can point to their own place (e.g. pypy puts
         it into pypy/module/_hpy_universal/_vendored)
 
         extra_include_dirs is a list of include dirs which is put BEFORE all
         others. By default it is empty, but it is used e.g. by PyPy to make
         sure that #include <Python.h> picks its own version, instead of the
         system-wide one.
         """
         self.tmpdir = tmpdir
+        self.dump_dir = dump_dir
         self.hpy_devel = hpy_devel
         self.hpy_abi = hpy_abi
         self.compiler_verbose = compiler_verbose
-        self.ExtensionTemplate=ExtensionTemplate
+        self.ExtensionTemplate = ExtensionTemplate
         self.extra_include_dirs = extra_include_dirs
 
     def _expand(self, ExtensionTemplate, name, template):
         source = ExtensionTemplate(template, name).expand()
         filename = self.tmpdir.join(name + '.c')
+        dump_file = self.dump_dir.joinpath(name + '.c') if self.dump_dir else None
         if PY2:
             # this code is used also by pypy tests, which run on python2. In
             # this case, we need to write as binary, because source is
             # "bytes". If we don't and source contains a non-ascii char, we
             # get an UnicodeDecodeError
+            if dump_file:
+                dump_file.write_text(source)
             filename.write(source, mode='wb')
         else:
+            if dump_file:
+                dump_file.write_text(source)
             filename.write(source)
         return name + '.c'
 
     def _fixup_template(self, ExtensionTemplate):
         return self.ExtensionTemplate if ExtensionTemplate is None else ExtensionTemplate
 
     def compile_module(self, main_src, ExtensionTemplate=None, name='mytest', extra_sources=()):
@@ -209,20 +282,22 @@
         from distutils.core import Extension
         filename = self._expand(ExtensionTemplate, name, main_src)
         sources = [str(filename)]
         for i, src in enumerate(extra_sources):
             extra_filename = self._expand(ExtensionTemplate, 'extmod_%d' % i, src)
             sources.append(extra_filename)
         #
+        if self.dump_dir:
+            pytest.skip("dumping test sources only")
         if sys.platform == 'win32':
             # not strictly true, could be mingw
             compile_args = [
                 '/Od',
                 '/WX',               # turn warnings into errors (all, for now)
-                # '/Wall',           # this is too aggresive, makes windows itself fail
+                # '/Wall',           # this is too aggressive, makes windows itself fail
                 '/Zi',
                 '-D_CRT_SECURE_NO_WARNINGS', # something about _snprintf and _snprintf_s
                 '/FS',               # Since the tests run in parallel
             ]
             link_args = [
                 '/DEBUG',
                 '/LTCG',
@@ -241,18 +316,20 @@
             name,
             sources=sources,
             include_dirs=self.extra_include_dirs,
             extra_compile_args=compile_args,
             extra_link_args=link_args)
 
         hpy_abi = self.hpy_abi
-        if hpy_abi == 'debug':
+        if hpy_abi == 'debug' or hpy_abi == 'trace':
             # there is no compile-time difference between universal and debug
             # extensions. The only difference happens at load time
             hpy_abi = 'universal'
+        elif hpy_abi in ('hybrid+debug', 'hybrid+trace'):
+            hpy_abi = 'hybrid'
         so_filename = c_compile(str(self.tmpdir), ext,
                                 hpy_devel=self.hpy_devel,
                                 hpy_abi=hpy_abi,
                                 compiler_verbose=self.compiler_verbose)
         return HPyModule(name, so_filename)
 
     def make_module(self, main_src, ExtensionTemplate=None, name='mytest',
@@ -266,30 +343,37 @@
         use make_module but explicitly use compile_module and import it
         manually as required by your test.
         """
         ExtensionTemplate = self._fixup_template(ExtensionTemplate)
         module = self.compile_module(
             main_src, ExtensionTemplate, name, extra_sources)
         so_filename = module.so_filename
-        if self.hpy_abi == 'universal':
-            return self.load_universal_module(name, so_filename, debug=False)
-        elif self.hpy_abi == 'debug':
-            return self.load_universal_module(name, so_filename, debug=True)
+        from hpy.universal import MODE_UNIVERSAL, MODE_DEBUG, MODE_TRACE
+        if self.hpy_abi in ('universal', 'hybrid'):
+            return self.load_universal_module(name, so_filename, mode=MODE_UNIVERSAL)
+        elif self.hpy_abi in ('debug', 'hybrid+debug'):
+            return self.load_universal_module(name, so_filename, mode=MODE_DEBUG)
+        elif self.hpy_abi in ('trace', 'hybrid+trace'):
+            return self.load_universal_module(name, so_filename, mode=MODE_TRACE)
         elif self.hpy_abi == 'cpython':
             return self.load_cpython_module(name, so_filename)
         else:
             assert False
 
-    def load_universal_module(self, name, so_filename, debug):
-        assert self.hpy_abi in ('universal', 'debug')
+    def load_universal_module(self, name, so_filename, mode):
+        assert self.hpy_abi in ('universal', 'hybrid', 'debug', 'hybrid+debug',
+                                'trace', 'hybrid+trace')
         import sys
         import hpy.universal
+        import importlib.util
         assert name not in sys.modules
-        mod = hpy.universal.load(name, so_filename, debug=debug)
+        spec = importlib.util.spec_from_file_location(name, so_filename)
+        mod = hpy.universal.load(name, so_filename, spec, mode=mode)
         mod.__file__ = so_filename
+        mod.__spec__ = spec
         return mod
 
     def load_cpython_module(self, name, so_filename):
         assert self.hpy_abi == 'cpython'
         # we've got a normal CPython module compiled with the CPython API/ABI,
         # let's load it normally. It is important to do the imports only here,
         # because this file will be imported also by PyPy tests which runs on
@@ -314,36 +398,37 @@
         self.hpy_abi = hpy_abi
 
     def run(self, mod, code):
         """ Starts new subprocess that loads given module as 'mod' using the
             correct ABI mode and then executes given code snippet. Use
             "--subprocess-v" to enable logging from this.
         """
-        import subprocess
         env = os.environ.copy()
         pythonpath = [os.path.dirname(mod.so_filename)]
         if 'PYTHONPATH' in env:
             pythonpath.append(env['PYTHONPATH'])
         env["PYTHONPATH"] = os.pathsep.join(pythonpath)
         if self.hpy_abi in ['universal', 'debug']:
             # HPy module
             load_module = "import sys;" + \
                           "import hpy.universal;" + \
-                          "mod = hpy.universal.load('{name}', '{so_filename}', debug={debug});"
+                          "import importlib.util;" + \
+                          "spec = importlib.util.spec_from_file_location('{name}', '{so_filename}');" + \
+                          "mod = hpy.universal.load('{name}', '{so_filename}', spec, debug={debug});"
             escaped_filename = mod.so_filename.replace("\\", "\\\\")  # Needed for Windows paths
             load_module = load_module.format(name=mod.name, so_filename=escaped_filename,
                                              debug=self.hpy_abi == 'debug')
         else:
             # CPython module
             assert self.hpy_abi == 'cpython'
             load_module = "import {} as mod;".format(mod.name)
         if self.verbose:
             print("\n---\nExecuting in subprocess: {}".format(load_module + code))
-        result = subprocess.run([sys.executable, "-c", load_module + code], env=env,
-                                stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        result = atomic_run([sys.executable, "-c", load_module + code], env=env,
+                            stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         if self.verbose:
             print("stdout/stderr:")
             try:
                 out = result.stdout.decode('latin-1')
                 err = result.stderr.decode('latin-1')
                 print("----\n{out}--\n{err}-----".format(out=out, err=err))
             except UnicodeDecodeError:
@@ -352,68 +437,104 @@
 
 
 @pytest.mark.usefixtures('initargs')
 class HPyTest:
     ExtensionTemplate = DefaultExtensionTemplate
 
     @pytest.fixture()
-    def initargs(self, compiler):
+    def initargs(self, compiler, leakdetector, capfd):
         self.compiler = compiler
+        self.leakdetector = leakdetector
+        self.capfd = capfd
 
     def make_module(self, main_src, name='mytest', extra_sources=()):
         ExtensionTemplate = self.ExtensionTemplate
         return self.compiler.make_module(main_src, ExtensionTemplate, name,
                                          extra_sources)
 
     def compile_module(self, main_src, name='mytest', extra_sources=()):
         ExtensionTemplate = self.ExtensionTemplate
         return self.compiler.compile_module(main_src, ExtensionTemplate, name,
                                      extra_sources)
 
+    def expect_make_error(self, main_src, error):
+        with pytest.raises(distutils.errors.CompileError):
+            self.make_module(main_src)
+        #
+        # capfd.readouterr() "eats" the output, but we want to still see it in
+        # case of failure. Just print it again
+        cap = self.capfd.readouterr()
+        sys.stdout.write(cap.out)
+        sys.stderr.write(cap.err)
+        #
+        # gcc prints compiler errors to stderr, but MSVC seems to print them
+        # to stdout. Let's just check both
+        if error in cap.out or error in cap.err:
+            # the error was found, we are good
+            return
+        raise Exception("The following error message was not found in the compiler "
+                        "output:\n    " + error)
+
+
     def supports_refcounts(self):
         """ Returns True if the underlying Python implementation supports
             reference counts.
 
-            By default returns True on CPython and False on other
+            By default, returns True on CPython and False on other
             implementations.
         """
         return sys.implementation.name == "cpython"
 
     def supports_ordinary_make_module_imports(self):
         """ Returns True if `.make_module(...)` loads modules using a
             standard Python import mechanism (e.g. `importlib.import_module`).
 
-            By default returns True because the base implementation of
+            By default, returns True because the base implementation of
             `.make_module(...)` uses an ordinary import. Sub-classes that
             override `.make_module(...)` may also want to override this
             method.
         """
         return True
 
+    def supports_refcounts(self):
+        """ Returns True if the underlying Python implementation supports
+            the vectorcall protocol.
+
+            By default, this returns True for Python version 3.8+ on all
+            implementations.
+        """
+        return sys.version_info >= (3, 8)
+
 
 class HPyDebugCapture:
     """
     Context manager that sets HPy debug invalid handle hook and remembers the
     number of invalid handles reported. Once closed, sets the invalid handle
     hook back to None.
     """
     def __init__(self):
         self.invalid_handles_count = 0
+        self.invalid_builders_count = 0
 
     def _capture_report(self):
         self.invalid_handles_count += 1
 
+    def _capture_builder_report(self):
+        self.invalid_builders_count += 1
+
     def __enter__(self):
         from hpy.universal import _debug
         _debug.set_on_invalid_handle(self._capture_report)
+        _debug.set_on_invalid_builder_handle(self._capture_builder_report)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         from hpy.universal import _debug
         _debug.set_on_invalid_handle(None)
+        _debug.set_on_invalid_builder_handle(None)
 
 
 # the few functions below are copied and adapted from cffi/ffiplatform.py
 
 def c_compile(tmpdir, ext, hpy_devel, hpy_abi, compiler_verbose=0, debug=None):
     """Compile a C extension module using distutils."""
     saved_environ = os.environ.copy()
@@ -445,15 +566,21 @@
     options_build_ext['build_lib'] = ('ffiplatform', tmpdir)
     options_build_ext['build_temp'] = ('ffiplatform', tmpdir)
     options_build_py = dist.get_option_dict('build_py')
     options_build_py['build_lib'] = ('ffiplatform', tmpdir)
 
     # this is the equivalent of passing --hpy-abi from setup.py's command line
     dist.hpy_abi = hpy_abi
+    # For testing, we want to use static libs to avoid repeated compilation
+    # of the same sources which slows down testing.
+    dist.hpy_use_static_libs = True
     dist.hpy_ext_modules = [ext]
+    # We need to explicitly specify which Python modules we expect because some
+    # test cases create several distributions in the same temp directory.
+    dist.py_modules = [ext.name]
     hpy_devel.fix_distribution(dist)
 
     old_level = distutils.log.set_threshold(0) or 0
     old_dir = os.getcwd()
     try:
         os.chdir(tmpdir)
         distutils.log.set_verbosity(compiler_verbose)
@@ -470,8 +597,8 @@
 
     return soname
 
 
 # For situations when one wants to have "support.py" on the call stack.
 # For example, for asserting that it is in a stack trace.
 def trampoline(fun, *args, **kwargs):
-    fun(*args, **kwargs)
+    fun(*args, **kwargs)
```

### Comparing `hpy-0.0.4/test/test_00_basic.py` & `hpy-0.9.0rc1/test/test_hpylong.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,456 +1,440 @@
-"""
-NOTE: this tests are also meant to be run as PyPy "applevel" tests.
+from .support import HPyTest, DefaultExtensionTemplate
 
-This means that global imports will NOT be visible inside the test
-functions. In particular, you have to "import pytest" inside the test in order
-to be able to use e.g. pytest.raises (which on PyPy will be implemented by a
-"fake pytest module")
-"""
-from .support import HPyTest
-
-
-class TestBasic(HPyTest):
-
-    def test_get_version(self):
-        if self.compiler.hpy_abi != 'universal':
-            return
-        import hpy.universal
-        version, gitrev = hpy.universal.get_version()
-        # it's a bit hard to test the CONTENT of these values. Let's just
-        # check that they are strings...
-        assert isinstance(version, str)
-        assert isinstance(gitrev, str)
-
-    def test_empty_module(self):
+class HPyLongTemplate(DefaultExtensionTemplate):
+    def DEFINE_Long_From(self, type, api_suffix, val):
+        self.EXPORT("from_{type}_{val}".format(type=type, val=val))
+        return """
+            HPyDef_METH(from_{type}_{val}, "from_{type}_{val}", HPyFunc_NOARGS)
+            static HPy from_{type}_{val}_impl(HPyContext *ctx, HPy self)
+            {{
+                {type} a = {val};
+                return HPyLong_From{api_suffix}(ctx, a);
+            }}
+        """.format(type=type, val=val, api_suffix=api_suffix)
+
+    def DEFINE_Long_As(self, type, api_suffix, from_suffix=None):
+        self.EXPORT("as_{api_suffix}".format(api_suffix=api_suffix))
+        if not from_suffix:
+            from_suffix = api_suffix
+        return """
+            HPyDef_METH(as_{api_suffix}, "as_{api_suffix}", HPyFunc_O)
+            static HPy as_{api_suffix}_impl(HPyContext *ctx, HPy self, HPy arg)
+            {{
+                {type} a = HPyLong_As{api_suffix}(ctx, arg);
+                if (a == (({type})-1) && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_From{from_suffix}(ctx, a * 2);
+            }}
+        """.format(type=type, api_suffix=api_suffix, from_suffix=from_suffix)
+
+class TestLong(HPyTest):
+
+    ExtensionTemplate = HPyLongTemplate
+
+    def unsigned_long_bits(self):
+        """ Return the number of bits in an unsigned long. """
+        import struct
+        unsigned_long_bytes = len(struct.pack('l', 0))
+        return 8 * unsigned_long_bytes
+
+    def magic_int(self, v):
+        """ Return an instance of a class that implements __int__
+            and returns value v.
+        """
+        class MagicInt(object):
+            def __int__(self):
+                return v
+        return MagicInt()
+
+    def magic_index(self, v):
+        """ Return an instance of a class that implements __index__
+            and returns value v.
+        """
+        class MagicIndex(object):
+            def __index__(self):
+                return v
+        return MagicIndex()
+
+    def python_supports_magic_index(self):
+        """ Return True if the Python version is 3.8 or later and thus
+            should support calling __index__ in the various HPyLong_As...
+            methods.
+        """
         import sys
-        mod = self.make_module("""
-            @INIT
-        """)
-        assert type(mod) is type(sys)
+        vi = sys.version_info
+        return (vi.major > 3 or (vi.major == 3 and vi.minor >= 8))
 
-    def test_different_name(self):
-        mod = self.make_module("""
-            @INIT
-        """, name="foo")
-        assert mod.__name__ == "foo"
+    def python_supports_magic_int(self):
+        """ Return True if the Python version is 3.9 or earlier and thus
+            should support calling __int__ on non-int based types in some
+            HPyLong_As... methods.
+        """
+        import sys
+        vi = sys.version_info
+        assert vi.major >= 3
+        return (vi.major == 3 and vi.minor <= 9)
+
+    def test_Long_FromFixedWidth(self):
+        mod = self.make_module("""
+            @DEFINE_Long_From(int32_t, Int32_t, INT32_MAX)
+            @DEFINE_Long_From(int32_t, Int32_t, INT32_MIN)
+            @DEFINE_Long_From(uint32_t, UInt32_t, UINT32_MAX)
+            @DEFINE_Long_From(int64_t, Int64_t, INT64_MAX)
+            @DEFINE_Long_From(int64_t, Int64_t, INT64_MIN)
+            @DEFINE_Long_From(uint64_t, UInt64_t, UINT64_MAX)
+            @INIT
+        """)
+        assert mod.from_int32_t_INT32_MAX() == 2147483647
+        assert mod.from_int32_t_INT32_MIN() == -2147483648
+        assert mod.from_uint32_t_UINT32_MAX() == 4294967295
+        assert mod.from_int64_t_INT64_MAX() == 9223372036854775807
+        assert mod.from_int64_t_INT64_MIN() == -9223372036854775808
+        assert mod.from_uint64_t_UINT64_MAX() == 18446744073709551615
 
-    def test_noop_function(self):
+    def test_Long_FromLong(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS, .doc="hello world")
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                return HPy_Dup(ctx, ctx->h_None);
+                long a = 500;
+                return HPyLong_FromLong(ctx, a);
             }
-
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f() is None
-        assert mod.f.__doc__ == 'hello world'
+        assert mod.f() == 500
 
-    def test_self_is_module(self):
+    def test_Long_AsFixedWidth(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self)
-            {
-                return HPy_Dup(ctx, self);
-            }
-            @EXPORT(f)
+            @DEFINE_Long_As(int32_t, Int32_t)
+            @DEFINE_Long_As(uint32_t, UInt32_t)
+            @DEFINE_Long_As(uint32_t, UInt32_tMask, UInt32_t)
+            @DEFINE_Long_As(int64_t, Int64_t)
+            @DEFINE_Long_As(uint64_t, UInt64_t)
+            @DEFINE_Long_As(uint64_t, UInt64_tMask, UInt64_t)
             @INIT
         """)
-        assert mod.f() is mod
 
-    def test_identity_function(self):
+        assert mod.as_Int32_t(45) == 90
+        assert mod.as_Int32_t(-45) == -90
+        # doubling INT32_MAX is like a left-shift and will result in a negative value
+        assert mod.as_Int32_t(2147483647) < 0
+        with pytest.raises(TypeError):
+            mod.as_Int32_t("this is not a number")
+        if self.python_supports_magic_int():
+            assert mod.as_Int32_t(self.magic_int(2)) == 4
+        if self.python_supports_magic_index():
+            assert mod.as_Int32_t(self.magic_index(2)) == 4
+
+        assert mod.as_UInt32_t(45) == 90
+        with pytest.raises(OverflowError):
+            mod.as_UInt32_t(-45)
+        assert mod.as_UInt32_t(2147483647) == 4294967294
+
+        assert mod.as_UInt32_tMask(0xffffffffffffffff) == 0xfffffffe
+
+        assert mod.as_Int64_t(45) == 90
+        assert mod.as_Int64_t(-45) == -90
+        # doubling INT32_MAX is like a left-shift and will result in a negative value
+        assert mod.as_Int64_t(2147483647) == 4294967294
+        assert mod.as_Int64_t(9223372036854775807) < 0
+        with pytest.raises(TypeError):
+            mod.as_Int64_t("this is not a number")
+
+        assert mod.as_UInt64_t(45) == 90
+        with pytest.raises(OverflowError):
+            mod.as_UInt64_t(-45)
+        assert mod.as_UInt64_t(9223372036854775807) == 18446744073709551614
+
+        assert mod.as_UInt64_tMask(0xffffffffffffffffff) == 0xfffffffffffffffe
+
+    def test_Long_AsLong(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                return HPy_Dup(ctx, arg);
+                long a = HPyLong_AsLong(ctx, arg);
+                if (a == -1 && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_FromLong(ctx, a * 2);
             }
             @EXPORT(f)
             @INIT
         """)
-        x = object()
-        assert mod.f(x) is x
+        assert mod.f(45) == 90
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        if self.python_supports_magic_int():
+            assert mod.f(self.magic_int(2)) == 4
+        if self.python_supports_magic_index():
+            assert mod.f(self.magic_index(2)) == 4
 
-    def test_float_asdouble(self):
+    def test_Long_FromUnsignedLong(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                double a = HPyFloat_AsDouble(ctx, arg);
-                return HPyFloat_FromDouble(ctx, a * 2.);
+                unsigned long a = 500;
+                return HPyLong_FromUnsignedLong(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(1.) == 2.
+        assert mod.f() == 500
 
-    def test_wrong_number_of_arguments(self):
+    def test_Long_AsUnsignedLong(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f_noargs, "f_noargs", f_noargs_impl, HPyFunc_NOARGS)
-            static HPy f_noargs_impl(HPyContext *ctx, HPy self)
-            {
-                return HPy_Dup(ctx, ctx->h_None);
-            }
-            HPyDef_METH(f_o, "f_o", f_o_impl, HPyFunc_O)
-            static HPy f_o_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                return HPy_Dup(ctx, ctx->h_None);
+                unsigned long a = HPyLong_AsUnsignedLong(ctx, arg);
+                if ((a == (unsigned long) -1) && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_FromUnsignedLong(ctx, a);
             }
-            @EXPORT(f_noargs)
-            @EXPORT(f_o)
+            @EXPORT(f)
             @INIT
         """)
+        assert mod.f(45) == 45
+        with pytest.raises(OverflowError):
+            mod.f(-91)
         with pytest.raises(TypeError):
-            mod.f_noargs(1)
+            mod.f("this is not a number")
         with pytest.raises(TypeError):
-            mod.f_o()
+            mod.f(self.magic_int(2))
         with pytest.raises(TypeError):
-            mod.f_o(1, 2)
+            mod.f(self.magic_index(2))
 
-    def test_close(self):
+    def test_Long_AsUnsignedLongMask(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                HPy one = HPyLong_FromLong(ctx, 1);
-                if (HPy_IsNull(one))
+                unsigned long a = HPyLong_AsUnsignedLongMask(ctx, arg);
+                if ((a == (unsigned long) -1) && HPyErr_Occurred(ctx))
                     return HPy_NULL;
-                HPy res = HPy_Add(ctx, arg, one);
-                HPy_Close(ctx, one);
-                return res;
+                return HPyLong_FromUnsignedLong(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(41.5) == 42.5
+        assert mod.f(45) == 45
+        assert mod.f(-1) == 2**self.unsigned_long_bits() - 1
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        if self.python_supports_magic_int():
+            assert mod.f(self.magic_int(2)) == 2
+        if self.python_supports_magic_index():
+            assert mod.f(self.magic_index(2)) == 2
 
-    def test_bool(self):
+    def test_Long_FromLongLong(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                int cond = HPyLong_AsLong(ctx, arg) > 5;
-                return HPy_Dup(ctx, cond ? ctx->h_True : ctx->h_False);
+                // take a value which doesn't fit in 32 bit
+                long long val = 2147483648;
+                return HPyLong_FromLongLong(ctx, val);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(4) is False
-        assert mod.f(6) is True
+        assert mod.f() == 2147483648
 
-    def test_exception(self):
+    def test_Long_AsLongLong(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                long x = HPyLong_AsLong(ctx, arg);
-                if (x < 5) {
-                    return HPyLong_FromLong(ctx, -x);
-                }
-                else {
-                    HPyErr_SetString(ctx, ctx->h_ValueError, "hello world");
+                long long a = HPyLong_AsLongLong(ctx, arg);
+                if ((a == (long long) -1) && HPyErr_Occurred(ctx))
                     return HPy_NULL;
-                }
+                return HPyLong_FromLongLong(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(-10) == 10
-        with pytest.raises(ValueError) as exc:
-            mod.f(20)
-        assert str(exc.value) == 'hello world'
+        assert mod.f(2147483648) == 2147483648
+        assert mod.f(-2147483648) == -2147483648
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        if self.python_supports_magic_int():
+            assert mod.f(self.magic_int(2)) == 2
+        if self.python_supports_magic_index():
+            assert mod.f(self.magic_index(2)) == 2
 
-    def test_varargs(self):
+    def test_Long_FromUnsignedLongLong(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                long a, b;
-                if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
-                    return HPy_NULL;
-                return HPyLong_FromLong(ctx, 10*a + b);
+                // take a value which doesn't fit in unsigned 32 bit
+                unsigned long long val = 4294967296;
+                return HPyLong_FromUnsignedLongLong(ctx, val);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(4, 5) == 45
+        assert mod.f() == 4294967296
 
-    def test_builtin_handles(self):
+    def test_Long_AsUnsignedLongLong(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                long i = HPyLong_AsLong(ctx, arg);
-                HPy h;
-                switch(i) {
-                    case 1: h = ctx->h_None; break;
-                    case 2: h = ctx->h_False; break;
-                    case 3: h = ctx->h_True; break;
-                    case 4: h = ctx->h_ValueError; break;
-                    case 5: h = ctx->h_TypeError; break;
-                    case 6: h = ctx->h_IndexError; break;
-                    case 7: h = ctx->h_SystemError; break;
-                    case 8: h = ctx->h_BaseObjectType; break;
-                    case 9: h = ctx->h_TypeType; break;
-                    case 10: h = ctx->h_BoolType; break;
-                    case 11: h = ctx->h_LongType; break;
-                    case 12: h = ctx->h_FloatType; break;
-                    case 13: h = ctx->h_UnicodeType; break;
-                    case 14: h = ctx->h_TupleType; break;
-                    case 15: h = ctx->h_ListType; break;
-                    case 16: h = ctx->h_NotImplemented; break;
-                    case 17: h = ctx->h_Ellipsis; break;
-                    default:
-                        HPyErr_SetString(ctx, ctx->h_ValueError, "invalid choice");
-                        return HPy_NULL;
-                }
-                return HPy_Dup(ctx, h);
-            }
-            @EXPORT(f)
-            @INIT
-        """)
-        builtin_objs = (
-            '<NULL>', None, False, True, ValueError, TypeError, IndexError,
-            SystemError, object, type, bool, int, float, str, tuple, list, NotImplemented, Ellipsis,
-        )
-        for i, obj in enumerate(builtin_objs):
-            if i == 0:
-                continue
-            assert mod.f(i) is obj
-
-    def test_extern_def(self):
-        import pytest
-        main = """
-            extern HPyDef f;
-            extern HPyDef g;
-            extern HPyDef h;
-            extern HPyDef i;
-
-            @EXPORT(f)
-            @EXPORT(g)
-            @EXPORT(h)
-            @EXPORT(i)
-            @INIT
-        """
-        extra = """
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self)
-            {
-                return HPyLong_FromLong(ctx, 12345);
-            }
-            HPyDef_METH(g, "g", g_impl, HPyFunc_O)
-            static HPy g_impl(HPyContext *ctx, HPy self, HPy arg)
-            {
-                return HPy_Dup(ctx, arg);
-            }
-            HPyDef_METH(h, "h", h_impl, HPyFunc_VARARGS)
-            static HPy h_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
-            {
-                long a, b;
-                if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &a, &b))
-                    return HPy_NULL;
-                return HPyLong_FromLong(ctx, 10*a + b);
-            }
-            HPyDef_METH(i, "i", i_impl, HPyFunc_KEYWORDS)
-            static HPy i_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs,
-                              HPy kw)
-            {
-                long a, b;
-                static const char *kwlist[] = { "a", "b", NULL };
-                if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kw, "ll", kwlist, &a, &b))
+                unsigned long long a = HPyLong_AsUnsignedLongLong(ctx, arg);
+                if ((a == (unsigned long long) -1) && HPyErr_Occurred(ctx))
                     return HPy_NULL;
-                return HPyLong_FromLong(ctx, 10*a + b);
-            }
-        """
-        mod = self.make_module(main, extra_sources=[extra])
-        assert mod.f() == 12345
-        assert mod.g(42) == 42
-        assert mod.h(5, 6) == 56
-        assert mod.i(4, 3) == 43
-        assert mod.i(a=2, b=5) == 25
-        with pytest.raises(TypeError):
-            mod.h("not an integer", "not an integer either")
-
-    def test_Float_FromDouble(self):
-        mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self)
-            {
-                return HPyFloat_FromDouble(ctx, 123.45);
+                return HPyLong_FromUnsignedLongLong(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f() == 123.45
+        assert mod.f(4294967296) == 4294967296
+        with pytest.raises(OverflowError):
+            mod.f(-4294967296)
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        with pytest.raises(TypeError):
+            mod.f(self.magic_int(2))
+        with pytest.raises(TypeError):
+            mod.f(self.magic_index(2))
 
-    def test_unsupported_signature(self):
+    def test_Long_AsUnsignedLongLongMask(self):
         import pytest
-        with pytest.raises(ValueError) as exc:
-            self.make_module("""
-                HPyDef f = {
-                    .kind = HPyDef_Kind_Meth,
-                    .meth = {
-                        .name = "f",
-                        .signature = (HPyFunc_Signature)1234,
-                    }
-                };
-                @EXPORT(f)
-                @INIT
-            """)
-        assert str(exc.value) == 'Unsupported HPyMeth signature'
-
-    def test_repr_str_ascii_bytes(self):
         mod = self.make_module("""
-            HPyDef_METH(f1, "f1", f1_impl, HPyFunc_O)
-            static HPy f1_impl(HPyContext *ctx, HPy self, HPy arg)
-            {
-                return HPy_Repr(ctx, arg);
-            }
-            HPyDef_METH(f2, "f2", f2_impl, HPyFunc_O)
-            static HPy f2_impl(HPyContext *ctx, HPy self, HPy arg)
-            {
-                return HPy_Str(ctx, arg);
-            }
-            HPyDef_METH(f3, "f3", f3_impl, HPyFunc_O)
-            static HPy f3_impl(HPyContext *ctx, HPy self, HPy arg)
-            {
-                return HPy_ASCII(ctx, arg);
-            }
-            HPyDef_METH(f4, "f4", f4_impl, HPyFunc_O)
-            static HPy f4_impl(HPyContext *ctx, HPy self, HPy arg)
-            {
-                return HPy_Bytes(ctx, arg);
-            }
-            @EXPORT(f1)
-            @EXPORT(f2)
-            @EXPORT(f3)
-            @EXPORT(f4)
-            @INIT
-        """)
-        assert mod.f1("\u1234") == "'\u1234'"
-        assert mod.f2(42) == "42"
-        assert mod.f3("\u1234") == "'\\u1234'"
-        assert mod.f4(bytearray(b"foo")) == b"foo"
-
-    def test_is_true(self):
-        mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                int cond = HPy_IsTrue(ctx, arg);
-                return HPy_Dup(ctx, cond ? ctx->h_True : ctx->h_False);
+                unsigned long long a = HPyLong_AsUnsignedLongLongMask(ctx, arg);
+                if ((a == (unsigned long long) -1) && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_FromUnsignedLongLong(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f("1234") is True
-        assert mod.f("") is False
+        assert mod.f(45) == 45
+        assert mod.f(-1) == 2**64 - 1
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        if self.python_supports_magic_int():
+            assert mod.f(self.magic_int(2)) == 2
+        if self.python_supports_magic_index():
+            assert mod.f(self.magic_index(2)) == 2
 
-    def test_richcompare(self):
+    def test_Long_FromSize_t(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                HPy arg2 = HPyLong_FromLong(ctx, 100);
-                HPy result = HPy_RichCompare(ctx, arg, arg2, HPy_GT);
-                HPy_Close(ctx, arg2);
-                return result;
+                // take a value which doesn't fit in 32 bit
+                size_t a = 2147483648;
+                return HPyLong_FromSize_t(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(100) is False
-        assert mod.f(150) is True
+        assert mod.f() == 2147483648
 
-    def test_richcomparebool(self):
+    def test_Long_AsSize_t(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                HPy arg2 = HPyLong_FromLong(ctx, 100);
-                int result = HPy_RichCompareBool(ctx, arg, arg2, HPy_GE);
-                HPy_Close(ctx, arg2);
-                return HPyLong_FromLong(ctx, -result);
+                size_t a = HPyLong_AsSize_t(ctx, arg);
+                if ((a == (size_t) -1) && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_FromSize_t(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(50) == 0
-        assert mod.f(100) == -1
+        assert mod.f(2147483648) == 2147483648
+        with pytest.raises(OverflowError):
+            mod.f(-2147483648)
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        with pytest.raises(TypeError):
+            mod.f(self.magic_int(2))
+        with pytest.raises(TypeError):
+            mod.f(self.magic_index(2))
 
-    def test_hash(self):
+    def test_Long_FromSsize_t(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
             {
-                HPy_hash_t hash = HPy_Hash(ctx, arg);
-                return HPyLong_FromSsize_t(ctx, hash);
+                HPy_ssize_t a = -42;
+                return HPyLong_FromSsize_t(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        x = object()
-        assert mod.f(x) == hash(x)
+        assert mod.f() == -42
 
-    def test_ctx_name(self):
+    def test_Long_AsSsize_t(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self)
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                return HPyUnicode_FromString(ctx, ctx->name);
+                HPy_ssize_t a = HPyLong_AsSsize_t(ctx, arg);
+                if ((a == (HPy_ssize_t) -1) && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyLong_FromSsize_t(ctx, a);
             }
-
             @EXPORT(f)
             @INIT
         """)
-        ctx_name = mod.f()
-        hpy_abi = self.compiler.hpy_abi
-        if hpy_abi == 'cpython':
-            assert ctx_name == 'HPy CPython ABI'
-        elif hpy_abi == 'universal':
-            # this can be "HPy Universal ABI (CPython backend)" or
-            # "... (PyPy backend)", etc.
-            assert ctx_name.startswith('HPy Universal ABI')
-        elif hpy_abi == 'debug':
-            assert ctx_name.startswith('HPy Debug Mode ABI')
-        else:
-            assert False, 'unexpected hpy_abi: %s' % hpy_abi
+        assert mod.f(41) == 41
+        assert mod.f(-41) == -41
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
+        with pytest.raises(TypeError):
+            mod.f(self.magic_int(2))
+        with pytest.raises(TypeError):
+            mod.f(self.magic_index(2))
 
-    def test_FromVoidP_AsVoidP(self):
+    def test_Long_AsVoidPtr(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "is_null", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy val)
             {
-                void *p = HPy_AsVoidP(arg);
-                HPy h = HPy_FromVoidP(p);
-                return HPy_Dup(ctx, h);
+                void* ptr = HPyLong_AsVoidPtr(ctx, val);
+                if (!ptr) {
+                    return HPy_Dup(ctx, ctx->h_True);
+                } else {
+                    return HPy_Dup(ctx, ctx->h_False);
+                }
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f(42) == 42
+        assert mod.is_null(0) == True
+        assert mod.is_null(10) == False
 
-    def test_leave_python(self):
+    def test_Long_AsDouble(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                HPy_ssize_t data_len;
-                const char* data = HPyUnicode_AsUTF8AndSize(ctx, arg, &data_len);
-                HPy_ssize_t acount = 0;
-                HPy_BEGIN_LEAVE_PYTHON(ctx);
-                for (HPy_ssize_t i = 0; i < data_len; ++i) {
-                    if (data[i] == 'a')
-                        acount++;
-                }
-                HPy_END_LEAVE_PYTHON(ctx);
-                return HPyLong_FromSize_t(ctx, acount);
+                double a = HPyLong_AsDouble(ctx, arg);
+                if (a == -1.0 && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                return HPyFloat_FromDouble(ctx, a);
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f("abraka") == 3
+        assert mod.f(45) == 45.0
+        with pytest.raises(TypeError):
+            mod.f("this is not a number")
```

### Comparing `hpy-0.0.4/test/test_argparse.py` & `hpy-0.9.0rc1/test/test_argparse.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             __attribute__((unused))
             #endif
             static inline
             HPy char_to_hpybytes(HPyContext *ctx, char a) {{
                 return HPyBytes_FromStringAndSize(ctx, &a, 1);
             }}
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {{
                 {type} a;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "{fmt}", &a))
                     return HPy_NULL;
                 return {hpy_converter}(ctx, a);
             }}
             @EXPORT(f)
@@ -294,17 +294,17 @@
         assert mod.f("") == 0
         assert mod.f("0") == 1
 
 
 class TestArgParse(HPyTest):
     def make_two_arg_add(self, fmt="OO"):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {{
                 HPy a;
                 HPy b = HPy_NULL;
                 HPy res;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "{fmt}", &a, &b))
                     return HPy_NULL;
                 if (HPy_IsNull(b)) {{
@@ -319,17 +319,17 @@
             @EXPORT(f)
             @INIT
         """.format(fmt=fmt))
         return mod
 
     def test_many_int_arguments(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 long a, b, c, d, e;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "lllll",
                                   &a, &b, &c, &d, &e))
                     return HPy_NULL;
                 return HPyLong_FromLong(ctx,
                     10000*a + 1000*b + 100*c + 10*d + e);
@@ -337,33 +337,33 @@
             @EXPORT(f)
             @INIT
         """)
         assert mod.f(4, 5, 6, 7, 8) == 45678
 
     def test_many_handle_arguments(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 return HPy_Add(ctx, a, b);
             }
             @EXPORT(f)
             @INIT
         """)
         assert mod.f("a", "b") == "ab"
 
     def test_supplying_hpy_tracker(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b, result;
                 HPyTracker ht;
                 if (!HPyArg_Parse(ctx, &ht, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 result = HPy_Add(ctx, a, b);
                 HPyTracker_Close(ctx, ht);
@@ -428,23 +428,23 @@
             mod.f(1, 2)
         assert str(exc.value) == "my-error-message"
 
 
 class TestArgParseKeywords(HPyTest):
     def make_two_arg_add(self, fmt="O+O+"):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_KEYWORDS)
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs, HPy kw)
+                              const HPy *args, size_t nargs, HPy kwnames)
             {{
                 HPy a, b, result;
                 HPyTracker ht;
                 static const char *kwlist[] = {{ "a", "b", NULL }};
-                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "{fmt}",
-                                          kwlist, &a, &b)) {{
+                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kwnames,
+                                          "{fmt}", kwlist, &a, &b)) {{
                     return HPy_NULL;
                 }}
                 result = HPy_Add(ctx, a, b);
                 HPyTracker_Close(ctx, ht);
                 return result;
             }}
             @EXPORT(f)
@@ -454,45 +454,47 @@
 
     def test_handle_two_arguments(self):
         mod = self.make_two_arg_add("OO")
         assert mod.f("x", b="y") == "xy"
 
     def test_handle_reordered_arguments(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_KEYWORDS)
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs, HPy kw)
+                              const HPy *args, size_t nargs, HPy kwnames)
             {
                 HPy a, b, result;
                 HPyTracker ht;
                 static const char *kwlist[] = { "a", "b", NULL };
-                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "OO", kwlist, &a, &b)) {
+                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kwnames, "OO",
+                                          kwlist, &a, &b)) {
                     return HPy_NULL;
                 }
                 result = HPy_Add(ctx, a, b);
                 HPyTracker_Close(ctx, ht);
                 return result;
             }
             @EXPORT(f)
             @INIT
         """)
         assert mod.f(b="y", a="x") == "xy"
 
     def test_handle_optional_arguments(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_KEYWORDS)
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs, HPy kw)
+                              const HPy *args, size_t nargs, HPy kwnames)
             {
                 HPy a;
                 HPy b = HPy_NULL;
                 HPyTracker ht;
                 HPy res;
                 static const char *kwlist[] = { "a", "b", NULL };
-                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "O|O", kwlist, &a, &b)) {
+                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kwnames, "O|O",
+                                          kwlist, &a, &b)) {
                     return HPy_NULL;
                 }
                 if (HPy_IsNull(b)) {
                     b = HPyLong_FromLong(ctx, 5);
                     HPyTracker_Add(ctx, ht, b);
                 }
                 res = HPy_Add(ctx, a, b);
@@ -534,45 +536,46 @@
         with pytest.raises(TypeError) as exc:
             mod.f(1, 2)
         assert str(exc.value) == "add_two() mismatched args (too many keywords for fmt)"
 
     def test_blank_keyword_argument_exception(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_KEYWORDS)
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs, HPy kw)
+                              const HPy *args, size_t nargs, HPy kwnames)
             {
                 long a, b, c;
                 static const char *kwlist[] = { "", "b", "", NULL };
-                if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kw, "lll", kwlist,
-                                          &a, &b, &c))
+                if (!HPyArg_ParseKeywords(ctx, NULL, args, nargs, kwnames,
+                                          "lll", kwlist, &a, &b, &c))
                     return HPy_NULL;
                 return HPy_Dup(ctx, ctx->h_None);
             }
             @EXPORT(f)
             @INIT
         """)
         with pytest.raises(SystemError) as exc:
             mod.f()
         assert str(exc.value) == "function empty keyword parameter name"
 
     def test_positional_only_argument(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_KEYWORDS)
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs, HPy kw)
+                              const HPy *args, size_t nargs, HPy kwnames)
             {
                 HPy a;
                 HPy b = HPy_NULL;
                 HPyTracker ht;
                 HPy res;
                 static const char *kwlist[] = { "", "b", NULL };
-                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "O|O", kwlist, &a, &b)) {
+                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kwnames,
+                                          "O|O", kwlist, &a, &b)) {
                     return HPy_NULL;
                 }
                 if (HPy_IsNull(b)) {
                     b = HPyLong_FromLong(ctx, 5);
                     HPyTracker_Add(ctx, ht, b);
                 }
                 res = HPy_Add(ctx, a, b);
@@ -615,7 +618,61 @@
 
     def test_error_with_overridden_message(self):
         import pytest
         mod = self.make_two_arg_add(fmt="OOO;my-error-message")
         with pytest.raises(TypeError) as exc:
             mod.f(1, 2)
         assert str(exc.value) == "my-error-message"
+
+    def test_keywords_dict(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_KEYWORDS)
+            static HPy f_impl(HPyContext *ctx, HPy self,
+                              const HPy *args, size_t nargs, HPy kwnames)
+            {
+                HPy args_tuple, kwdict;
+                HPy a, b = HPy_NULL, res;
+                HPyTracker ht;
+                HPy_ssize_t n_args_tuple, i;
+                HPy *args_arr;
+                int status;
+                static const char *kwlist[] = { "a", "b", NULL };
+
+                if (nargs != 2) {
+                    HPyErr_SetString(ctx, ctx->h_SystemError,
+                                     "expected exactly two args");
+                    return HPy_NULL;
+                }
+                args_tuple = args[0];
+                kwdict = args[1];
+                n_args_tuple = HPy_Length(ctx, args_tuple);
+                args_arr = (HPy *)malloc(n_args_tuple * sizeof(HPy));
+                for (i=0; i < n_args_tuple; i++)
+                    args_arr[i] = HPy_GetItem_i(ctx, args_tuple, i);
+
+                status = HPyArg_ParseKeywordsDict(ctx, &ht, args_arr,
+                             n_args_tuple, kwdict, "O|O", kwlist, &a, &b);
+
+                for (i=0; i < n_args_tuple; i++)
+                    HPy_Close(ctx, args_arr[i]);
+                free(args_arr);
+                if (!status) {
+                    return HPy_NULL;
+                }
+                if (HPy_IsNull(b)) {
+                    b = HPyLong_FromLong(ctx, 5);
+                    HPyTracker_Add(ctx, ht, b);
+                }
+                res = HPy_Add(ctx, a, b);
+                HPyTracker_Close(ctx, ht);
+                return res;
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        assert mod.f(tuple(), dict(a=3, b=2)) == 5
+        assert mod.f((3, 2), {}) == 5
+        assert mod.f(tuple(), dict(a=3)) == 8
+        assert mod.f((3,), {}) == 8
+        with pytest.raises(TypeError):
+            mod.f(tuple(), {})
```

### Comparing `hpy-0.0.4/test/test_call.py` & `hpy-0.9.0rc1/test/test_hpybytes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,131 @@
 from .support import HPyTest
 
+class TestBytes(HPyTest):
 
-class TestCall(HPyTest):
-    def argument_combinations(self, **items):
-        """ Returns all possible ways of expressing the given items as
-            arguments to a function.
-        """
-        items = list(items.items())
-        for i in range(len(items) + 1):
-            args = tuple(item[1] for item in items[:i])
-            kw = dict(items[i:])
-            yield {"args": args, "kw": kw}
-            if not args:
-                yield {"kw": kw}
-            if not kw:
-                yield {"args": args}
-            if not args and not kw:
-                yield {}
+    def test_Check(self):
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                if (HPyBytes_Check(ctx, arg))
+                    return HPy_Dup(ctx, ctx->h_True);
+                return HPy_Dup(ctx, ctx->h_False);
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        class MyBytes(bytes):
+            pass
 
-    def test_hpy_calltupledict(self):
-        import pytest
+        assert mod.f(b'hello') is True
+        assert mod.f('hello') is False
+        assert mod.f(MyBytes(b'hello')) is True
+
+    def test_Size(self):
         mod = self.make_module("""
-            HPyDef_METH(call, "call", call_impl, HPyFunc_KEYWORDS)
-            static HPy call_impl(HPyContext *ctx, HPy self,
-                                 HPy *args, HPy_ssize_t nargs, HPy kw)
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
+                HPy_ssize_t a = HPyBytes_Size(ctx, arg);
+                HPy_ssize_t b = HPyBytes_GET_SIZE(ctx, arg);
+                return HPyLong_FromLongLong(ctx, 10 * a + b);
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        assert mod.f(b'hello') == 55
 
-                HPy f, result;
-                HPy f_args = HPy_NULL;
-                HPy f_kw = HPy_NULL;
-                HPyTracker ht;
-                static const char *kwlist[] = { "f", "args", "kw", NULL };
-                if (!HPyArg_ParseKeywords(ctx, &ht, args, nargs, kw, "O|OO",
-                                          kwlist, &f, &f_args, &f_kw)) {
-                    return HPy_NULL;
-                }
-                result = HPy_CallTupleDict(ctx, f, f_args, f_kw);
-                HPyTracker_Close(ctx, ht);
-                return result;
-            }
-            @EXPORT(call)
+    def test_AsString(self):
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                long res = 0;
+                HPy_ssize_t n = HPyBytes_Size(ctx, arg);
+                const char *buf = HPyBytes_AsString(ctx, arg);
+                for(int i=0; i<n; i++)
+                    res = (res * 10) + buf[i];
+                return HPyLong_FromLong(ctx, res);
+            }
+            @EXPORT(f)
             @INIT
         """)
+        assert mod.f(b'ABC') == 100*ord('A') + 10*ord('B') + ord('C')
 
-        def f(a, b):
-            return a + b
-
-        def g():
-            return "this is g"
-
-        # test passing arguments with handles of the correct type --
-        # i.e. args is a tuple or a null handle, kw is a dict or a null handle.
-        for d in self.argument_combinations(a=1, b=2):
-            assert mod.call(f, **d) == 3
-        for d in self.argument_combinations(a=1):
-            with pytest.raises(TypeError):
-                mod.call(f, **d)
-        for d in self.argument_combinations():
-            with pytest.raises(TypeError):
-                mod.call(f, **d)
-        for d in self.argument_combinations():
-            assert mod.call(g, **d) == "this is g"
-        for d in self.argument_combinations(object=2):
-            assert mod.call(str, **d) == "2"
-        for d in self.argument_combinations():
-            with pytest.raises(TypeError):
-                mod.call("not callable", **d)
-        for d in self.argument_combinations(unknown=2):
-            with pytest.raises(TypeError):
-                mod.call("not callable", **d)
-
-        # test passing handles of the incorrect type as arguments
-        with pytest.raises(TypeError):
-            mod.call(f, args=[1, 2])
-        with pytest.raises(TypeError):
-            mod.call(f, args="string")
-        with pytest.raises(TypeError):
-            mod.call(f, args=1)
-        with pytest.raises(TypeError):
-            mod.call(f, args=None)
-        with pytest.raises(TypeError):
-            mod.call(f, kw=[1, 2])
-        with pytest.raises(TypeError):
-            mod.call(f, kw="string")
-        with pytest.raises(TypeError):
-            mod.call(f, kw=1)
-        with pytest.raises(TypeError):
-            mod.call(f, kw=None)
+    def test_AS_STRING(self):
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                long res = 0;
+                HPy_ssize_t n = HPyBytes_Size(ctx, arg);
+                const char *buf = HPyBytes_AS_STRING(ctx, arg);
+                for(int i=0; i<n; i++)
+                    res = (res * 10) + buf[i];
+                return HPyLong_FromLong(ctx, res);
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        assert mod.f(b'ABC') == 100*ord('A') + 10*ord('B') + ord('C')
 
-    def test_hpycallable_check(self):
+    def test_FromString(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                if (HPyCallable_Check(ctx, arg))
-                    return HPy_Dup(ctx, ctx->h_True);
-                return HPy_Dup(ctx, ctx->h_False);
+                const char *buf;
+                buf = HPyBytes_AsString(ctx, arg);
+                return HPyBytes_FromString(ctx, buf);
             }
+
             @EXPORT(f)
             @INIT
         """)
+        assert mod.f(b"aaa") == b"aaa"
+        assert mod.f(b"") == b""
+
+    def test_FromStringAndSize(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args,
+                              size_t nargs)
+            {
+                HPy src;
+                long len;
+                const char *buf;
+                if (!HPyArg_Parse(ctx, NULL, args, nargs, "Ol", &src, &len)) {
+                    return HPy_NULL;
+                }
+                buf = HPyBytes_AsString(ctx, src);
+                return HPyBytes_FromStringAndSize(ctx, buf, len);
+            }
+
+            HPyDef_METH(f_null, "f_null", HPyFunc_VARARGS)
+            static HPy f_null_impl(HPyContext *ctx, HPy self, const HPy *args,
+                                   size_t nargs)
+            {
+                long len;
+                if (!HPyArg_Parse(ctx, NULL, args, nargs, "l", &len)) {
+                    return HPy_NULL;
+                }
 
-        def f():
-            return "this is f"
+                return HPyBytes_FromStringAndSize(ctx, NULL, len);
+            }
 
-        assert mod.f(f) is True
-        assert mod.f(str) is True
-        assert mod.f("a") is False
-        assert mod.f(3) is False
+            @EXPORT(f)
+            @EXPORT(f_null)
+            @INIT
+        """)
+        assert mod.f(b"aaa", 3) == b"aaa"
+        assert mod.f(b"abc", 2) == b"ab"
+        assert mod.f(b"", 0) == b""
+        with pytest.raises(SystemError):
+            # negative size passed to HPyBytes_FromStringAndSize
+            mod.f(b"abc", -1)
+        for i in (-1, 0, 1):
+            with pytest.raises(ValueError) as err:
+                mod.f_null(i)
+            assert str(err.value) == (
+                "NULL char * passed to HPyBytes_FromStringAndSize")
```

### Comparing `hpy-0.0.4/test/test_cpy_compat.py` & `hpy-0.9.0rc1/test/test_cpy_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,43 @@
-from .support import HPyTest
-
+from .support import HPyTest, make_hpy_abi_fixture
 
 class TestCPythonCompatibility(HPyTest):
 
+    hpy_abi = make_hpy_abi_fixture('with hybrid', class_fixture=True)
+
     # One note about the supports_refcounts() in the tests below: on
     # CPython, handles are actually implemented as INCREF/DECREF, so we can
     # check e.g. after an HPy_Dup the refcnt is += 1. However, on PyPy they
     # are implemented in a completely different way which is unrelated to the
     # refcnt (this is the whole point of HPy, after all :)). So in many of the
-    # following ttests, checking the actual result of the function doesn't
+    # following tests, checking the actual result of the function doesn't
     # really make sens on PyPy. We still run the functions to ensure they do
     # not crash, though.
 
+    def test_abi(self):
+        mod = self.make_module("""
+            #include <Python.h>
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self)
+            {
+                return HPyUnicode_FromString(ctx, HPY_ABI);
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        hpy_abi = mod.f()
+        expected = self.compiler.hpy_abi
+        if expected in ('hybrid+debug', 'hybrid+trace'):
+            expected = 'hybrid'
+        assert hpy_abi == expected
+
     def test_frompyobject(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 PyObject *o = PyList_New(0);
                 Py_ssize_t initial_refcount = o->ob_refcnt;
                 HPy h = HPy_FromPyObject(ctx, o);
                 Py_ssize_t final_refcount = o->ob_refcnt;
 
@@ -37,15 +55,15 @@
         assert len(x) == 2
         if self.supports_refcounts():
             assert x == [1234, +1]
 
     def test_frompyobject_null(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 HPy h = HPy_FromPyObject(ctx, NULL);
                 if (HPy_IsNull(h)) {
                     return HPy_Dup(ctx, ctx->h_True);
                 }
                 else {
@@ -56,15 +74,15 @@
             @INIT
         """)
         assert mod.f()
 
     def test_aspyobject(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 PyObject *o = HPy_AsPyObject(ctx, arg);
                 long val = PyLong_AsLong(o);
                 Py_DecRef(o);
                 return HPyLong_FromLong(ctx, val*2);
             }
@@ -72,15 +90,15 @@
             @INIT
         """)
         assert mod.f(21) == 42
 
     def test_aspyobject_null(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 PyObject *o = HPy_AsPyObject(ctx, HPy_NULL);
                 if (o == NULL) {
                     return HPy_Dup(ctx, ctx->h_True);
                 }
                 else {
@@ -91,15 +109,15 @@
             @INIT
         """)
         assert mod.f()
 
     def test_aspyobject_custom_class(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 PyObject *o = HPy_AsPyObject(ctx, arg);
                 PyObject *o_res = PyObject_CallMethod(o, "foo", "");
                 HPy h_res = HPy_FromPyObject(ctx, o_res);
                 Py_DecRef(o);
                 Py_DecRef(o_res);
@@ -113,15 +131,15 @@
                 return 1234
         obj = MyClass()
         assert mod.f(obj) == 1234
 
     def test_hpy_close(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 PyObject *o = PyList_New(0);
 
                 HPy h = HPy_FromPyObject(ctx, o);
                 Py_ssize_t initial_refcount = o->ob_refcnt;
                 HPy_Close(ctx, h);
@@ -137,15 +155,15 @@
         x = mod.f()
         if self.supports_refcounts():
             assert x == -1
 
     def test_hpy_dup(self):
         mod = self.make_module("""
             #include <Python.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 PyObject *o = PyList_New(0);
 
                 HPy h = HPy_FromPyObject(ctx, o);
                 Py_ssize_t initial_refcount = o->ob_refcnt;
                 HPy h2 = HPy_Dup(ctx, h);
@@ -165,15 +183,15 @@
             assert x == +1
 
     def test_many_handles(self):
         mod = self.make_module("""
             #include <Python.h>
             #define NUM_HANDLES  10000
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 PyObject *o = PyList_New(0);
                 Py_ssize_t final_refcount;
 
                 Py_ssize_t result = -42;
                 HPy handles[NUM_HANDLES];
```

### Comparing `hpy-0.0.4/test/test_hpybuildvalue.py` & `hpy-0.9.0rc1/test/test_hpybuildvalue.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         # to execute. Argument test_cases should be a tuple with first item
         # being C code of the test case.
         # Generates, e.g.: case 0: return HPy_BuildValue(...);
         test_cases_c_code = ["case {}: {}; break;".format(i, case[0]) for i, case in enumerate(test_cases)]
         return self.make_module("""
             #include <limits.h>
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {{
                 switch (HPyLong_AsLong(ctx, arg)) {{
                     {test_cases}
                     default:
                         HPyErr_SetString(ctx, ctx->h_ValueError, "Wrong test case number");
                         return HPy_NULL;
@@ -32,14 +32,15 @@
             ('return HPy_BuildValue(ctx, "");', None),
             ('return HPy_BuildValue(ctx, "i", 42);', 42),
             ('return HPy_BuildValue(ctx, "i", 0);', 0),
             ('return HPy_BuildValue(ctx, "i", -1);', -1),
             ('return HPy_BuildValue(ctx, "I", 33);', 33),
             ('return HPy_BuildValue(ctx, "k", 1);', 1),
             ('return HPy_BuildValue(ctx, "K", 6543);', 6543),
+            ('return HPy_BuildValue(ctx, "n", 9876);', 9876),
             ('return HPy_BuildValue(ctx, "l", 345L);', 345),
             ('return HPy_BuildValue(ctx, "l", -876L);', -876),
             ('return HPy_BuildValue(ctx, "L", 545LL);', 545),
             ('return HPy_BuildValue(ctx, "L", -344LL);', -344),
             ('return HPy_BuildValue(ctx, "f", 0.25f);', 0.25),
             ('return HPy_BuildValue(ctx, "d", 0.25);', 0.25),
             ('return HPy_BuildValue(ctx, "ii", -1, 1);', (-1, 1)),
@@ -97,21 +98,21 @@
         for i, (code, expected_error) in enumerate(test_cases):
             with pytest.raises(SystemError) as e:
                 mod.f(i)
             assert expected_error in str(e), code
 
     def test_O_and_aliases(self):
         mod = self.make_module("""
-            HPyDef_METH(fo, "fo", fo_impl, HPyFunc_O)
+            HPyDef_METH(fo, "fo", HPyFunc_O)
             static HPy fo_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 return HPy_BuildValue(ctx, "O", arg);
             }
 
-            HPyDef_METH(fs, "fs", fs_impl, HPyFunc_O)
+            HPyDef_METH(fs, "fs", HPyFunc_O)
             static HPy fs_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 return HPy_BuildValue(ctx, "S", arg);
             }
 
             @EXPORT(fo)
             @EXPORT(fs)
@@ -125,15 +126,15 @@
         assert mod.fs(obj) == obj
 
     def test_O_with_new_object(self):
         # HPy_BuildValue does not steal the reference to the object passed as 'O',
         # the caller still needs to close it, otherwise -> handle leak
         mod = self.make_module("""
             #include <stdio.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy o = HPyLong_FromLong(ctx, 42);
                 HPy result;
                 if (HPyLong_AsLong(ctx, arg)) {
                     result = HPy_BuildValue(ctx, "O", o);
                 } else {
@@ -147,25 +148,25 @@
         """)
         assert mod.f(0) == (0.25, 42)
         assert mod.f(1) == 42
 
     def test_O_with_null(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(no_msg, "no_msg", no_msg_impl, HPyFunc_O)
+            HPyDef_METH(no_msg, "no_msg", HPyFunc_O)
             static HPy no_msg_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 if (HPyLong_AsLong(ctx, arg)) {
                     return HPy_BuildValue(ctx, "O", HPy_NULL);
                 } else {
                     return HPy_BuildValue(ctx, "(iO)", 42, HPy_NULL);
                 }
             }
 
-            HPyDef_METH(with_msg, "with_msg", with_msg_impl, HPyFunc_O)
+            HPyDef_METH(with_msg, "with_msg", HPyFunc_O)
             static HPy with_msg_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPyErr_SetString(ctx, ctx->h_ValueError, "Some err msg that will be asserted");
                 return no_msg_impl(ctx, self, arg);
             }
 
             @EXPORT(with_msg)
@@ -181,15 +182,15 @@
                 mod.no_msg(i)
             assert 'HPy_NULL object passed to HPy_BuildValue' in str(e)
 
 
     def test_OO_pars_with_new_objects(self):
         mod = self.make_module("""
             #include <stdio.h>
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy o1 = HPyLong_FromLong(ctx, 1);
                 HPy o2 = HPyLong_FromLong(ctx, 2);
                 HPy result = HPy_BuildValue(ctx, "(OO)", o1, o2);
                 HPy_Close(ctx, o1);
                 HPy_Close(ctx, o2);
@@ -204,13 +205,14 @@
         test_cases = [
             ('return HPy_BuildValue(ctx, "(ii)", INT_MIN, INT_MAX);',),
             ('return HPy_BuildValue(ctx, "(ll)", LONG_MIN, LONG_MAX);',),
             ('return HPy_BuildValue(ctx, "(LL)", LLONG_MIN, LLONG_MAX);',),
             ('return HPy_BuildValue(ctx, "(iI)", -1, UINT_MAX);',),
             ('return HPy_BuildValue(ctx, "(ik)", -1, ULONG_MAX);',),
             ('return HPy_BuildValue(ctx, "(iK)", -1, ULLONG_MAX);',),
+            ('return HPy_BuildValue(ctx, "(nn)", HPY_SSIZE_T_MIN, HPY_SSIZE_T_MAX);',),
         ]
         mod = self.make_tests_module(test_cases)
         for i, (test,) in enumerate(test_cases):
             result = mod.f(i)
             assert result[0] < 0, test
             assert result[1] > 0, test
```

### Comparing `hpy-0.0.4/test/test_hpydict.py` & `hpy-0.9.0rc1/test/test_hpytuple.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 from .support import HPyTest
 
-class TestDict(HPyTest):
+class TestTuple(HPyTest):
 
     def test_Check(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                if (HPyDict_Check(ctx, arg))
+                if (HPyTuple_Check(ctx, arg))
                     return HPy_Dup(ctx, ctx->h_True);
                 return HPy_Dup(ctx, ctx->h_False);
             }
             @EXPORT(f)
             @INIT
         """)
-        class MyDict(dict):
+        class MyTuple(tuple):
             pass
 
-        assert mod.f({}) is True
+        assert mod.f(()) is True
         assert mod.f([]) is False
-        assert mod.f(MyDict()) is True
+        assert mod.f(MyTuple()) is True
 
-    def test_New(self):
+    def test_FromArray(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self)
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                return HPyDict_New(ctx);
+                HPy x = HPyLong_FromLong(ctx, 42);
+                if (HPy_IsNull(x))
+                     return HPy_NULL;
+                HPy items[] = {self, arg, x};
+                HPy res = HPyTuple_FromArray(ctx, items, 3);
+                HPy_Close(ctx, x);
+                return res;
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f() == {}
+        assert mod.f('hello') == (mod, 'hello', 42)
 
-    def test_set_item(self):
+    def test_Pack(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
-                HPy dict = HPyDict_New(ctx);
-                if (HPy_IsNull(dict))
-                    return HPy_NULL;
-                HPy val = HPyLong_FromLong(ctx, 1234);
-                if (HPy_SetItem(ctx, dict, arg, val) == -1)
-                    return HPy_NULL;
-                HPy_Close(ctx, val);
-                return dict;
+                HPy x = HPyLong_FromLong(ctx, 42);
+                if (HPy_IsNull(x))
+                     return HPy_NULL;
+                HPy result = HPyTuple_Pack(ctx, 3, self, arg, x);
+                HPy_Close(ctx, x);
+                return result;
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f('hello') == {'hello': 1234}
+        assert mod.f('hello') == (mod, 'hello', 42)
 
-    def test_get_item(self):
+    def test_TupleBuilder(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy h_self, HPy h_arg)
             {
-                HPy key = HPyUnicode_FromString(ctx, "hello");
-                if (HPy_IsNull(key))
+                HPyTupleBuilder builder = HPyTupleBuilder_New(ctx, 3);
+                HPyTupleBuilder_Set(ctx, builder, 0, h_arg);
+                HPyTupleBuilder_Set(ctx, builder, 1, ctx->h_True);
+                HPy h_num = HPyLong_FromLong(ctx, -42);
+                if (HPy_IsNull(h_num))
+                {
+                    HPyTupleBuilder_Cancel(ctx, builder);
                     return HPy_NULL;
-                HPy val = HPy_GetItem(ctx, arg, key);
-                HPy_Close(ctx, key);
-                if (HPy_IsNull(val)) {
-                    HPyErr_Clear(ctx);
-                    return HPy_Dup(ctx, ctx->h_None);
                 }
-                return val;
+                HPyTupleBuilder_Set(ctx, builder, 2, h_num);
+                HPy_Close(ctx, h_num);
+                HPy h_tuple = HPyTupleBuilder_Build(ctx, builder);
+                return h_tuple;
             }
             @EXPORT(f)
             @INIT
         """)
-        assert mod.f({'hello': 1}) == 1
-        assert mod.f({}) is None
+        assert mod.f("xy") == ("xy", True, -42)
```

### Comparing `hpy-0.0.4/test/test_hpyerr.py` & `hpy-0.9.0rc1/test/test_hpyerr.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 
 class TestErr(HPyTest):
 
     def test_NoMemory(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 return HPyErr_NoMemory(ctx);
             }
             @EXPORT(f)
             @INIT
         """)
         with pytest.raises(MemoryError):
             mod.f()
 
     def test_FatalError(self, python_subprocess, fatal_exit_code):
         mod = self.compile_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 HPy_FatalError(ctx, "boom!");
                 // note: no 'return' statement.  This also tests that
                 // the call above is known to never return---otherwise,
                 // we get a warning from the missing 'return' and it is
                 // turned into an error.
@@ -45,15 +45,15 @@
         stderr_msg = result.stderr.splitlines()[0]
         assert stderr_msg.startswith(b"Fatal Python error: ")
         assert stderr_msg.endswith(b": boom!")
 
     def test_HPyErr_Occurred(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPyLong_AsLong(ctx, arg);
                 if (HPyErr_Occurred(ctx)) {
                     return HPyErr_SetString(ctx, ctx->h_ValueError, "hello world");
                 }
                 return HPyLong_FromLong(ctx, -1002);
@@ -65,15 +65,15 @@
         with pytest.raises(ValueError) as exc:
             mod.f("not an integer")
         assert str(exc.value) == 'hello world'
 
     def test_HPyErr_Cleared(self):
         import sys
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 HPyErr_SetString(ctx, ctx->h_ValueError, "hello world");
                 HPyErr_Clear(ctx);
                 return HPy_Dup(ctx, ctx->h_None);
             }
             @EXPORT(f)
@@ -81,21 +81,21 @@
         """)
         assert mod.f() is None
         assert sys.exc_info() == (None, None, None)
 
     def test_HPyErr_SetString(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 return HPyErr_SetString(ctx, ctx->h_ValueError, "error message");
             }
 
-            HPyDef_METH(g, "g", g_impl, HPyFunc_NOARGS)
+            HPyDef_METH(g, "g", HPyFunc_NOARGS)
             static HPy g_impl(HPyContext *ctx, HPy self)
             {
                 HPyErr_SetString(ctx, ctx->h_ValueError, "error message");
                 return HPy_NULL;
             }
 
             @EXPORT(g)
@@ -109,15 +109,15 @@
         with pytest.raises(ValueError) as err:
             mod.g()
         assert str(err.value) == "error message"
 
     def test_HPyErr_SetObject(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 return HPyErr_SetObject(ctx, ctx->h_ValueError, arg);
             }
             @EXPORT(f)
             @INIT
         """)
@@ -127,15 +127,15 @@
 
     def test_HPyErr_SetFromErrno(self):
         import pytest
         import errno
         mod = self.make_module("""
             #include <errno.h>
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy type)
             {{
                 errno = {errno};
                 return HPyErr_SetFromErrno(ctx, type);
             }}
             @EXPORT(f)
             @INIT
@@ -148,17 +148,17 @@
 
     def test_HPyErr_SetFromErrnoWithFilenameObjects(self):
         import pytest
         import errno
         mod = self.make_module("""
             #include <errno.h>
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {{
                 HPy type, file1, file2;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OOO", &type, &file1, &file2))
                     return HPy_NULL;
 
                 errno = {errno};
                 if (HPy_Is(ctx, file2, ctx->h_None)) {{
@@ -185,15 +185,15 @@
 
     def test_HPyErr_SetFromErrnoWithFilename(self):
         import pytest
         import errno
         mod = self.make_module("""
             #include <errno.h>
 
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy type)
             {{
                 errno = {errno};
                 return HPyErr_SetFromErrnoWithFilename(ctx, type, "Some message that will be asserted");
             }}
             @EXPORT(f)
             @INIT
@@ -203,15 +203,15 @@
 
         assert err.value.errno == errno.EINVAL
         assert "Some message that will be asserted" in str(err.value)
 
     def test_h_exceptions(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy h_dict, h_err;
                 h_dict = HPyDict_New(ctx);
                 HPy_SetItem_s(ctx, h_dict, "BaseException", ctx->h_BaseException);
                 HPy_SetItem_s(ctx, h_dict, "Exception", ctx->h_Exception);
                 HPy_SetItem_s(ctx, h_dict, "StopAsyncIteration", ctx->h_StopAsyncIteration);
@@ -331,17 +331,17 @@
         # but they work because they are actually OSError.
         check_exception(EnvironmentError)
         check_exception(IOError)
 
     def test_h_unicode_exceptions(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy h_key, h_args, h_kw;
                 HPy h_dict, h_err, h_err_value;
 
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OOO", &h_key, &h_args, &h_kw))
                     return HPy_NULL;
 
@@ -388,15 +388,15 @@
             UnicodeDecodeError, "utf-8", b"object", 0, 2, "reason"
         )
         check_exception(UnicodeTranslateError, "object", 0, 2, "reason")
 
     def test_h_warnings(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy h_dict, h_err;
                 h_dict = HPyDict_New(ctx);
                 HPy_SetItem_s(ctx, h_dict, "Warning", ctx->h_Warning);
                 HPy_SetItem_s(ctx, h_dict, "UserWarning", ctx->h_UserWarning);
                 HPy_SetItem_s(ctx, h_dict, "DeprecationWarning", ctx->h_DeprecationWarning);
@@ -436,15 +436,15 @@
         check_warning(UnicodeWarning)
         check_warning(BytesWarning)
         check_warning(ResourceWarning)
 
     def test_HPyErr_WarnEx(self):
         import warnings
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 switch (HPyLong_AsLong(ctx, arg)) {
                     case 0:
                       HPyErr_WarnEx(ctx, ctx->h_RuntimeWarning, "warn qzp", 1);
                       break;
                     case 1:
@@ -473,16 +473,16 @@
         check_warning(0, RuntimeWarning, "warn qzp", "support.py")
         check_warning(1, FutureWarning, "warn rtq", "test_hpyerr.py")
         check_warning(2, Warning, "warn null", "support.py")
 
 
     def test_errorval_returned_by_api_functions_hpy(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 HPy a = HPy_NULL;
                 HPy b = HPy_NULL;
                 HPy res;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 res = HPy_TrueDivide(ctx, a, b);
@@ -499,15 +499,15 @@
             @INIT
         """)
         assert mod.f(21, 3) == 7
         assert mod.f(21, 0) == -42
 
     def test_errorval_returned_by_api_functions_int(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy_ssize_t length = HPy_Length(ctx, arg);
                 if (length == -1) {
                     HPyErr_Clear(ctx);
                     return HPyLong_FromLong(ctx, -42);
                 }
@@ -518,16 +518,16 @@
         """)
         assert mod.f([100, 200, 300]) == 3
         assert mod.f(None) == -42
 
     def test_HPyErr_NewException(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 // MSVC doesn't allow "static HPy h_FooErr = HPy_NULL"
                 // so we do an initialization dance instead.
                 static int foo_error_initialized = 0;
                 static HPy h_FooError;
                 HPy arg;
                 HPy h_base = HPy_NULL;
@@ -598,16 +598,16 @@
         check(base=RuntimeError, dict_=None, doc=b'mytest')
         check(base=RuntimeError, dict_={"test": "pass"}, doc=None)
         check(base=RuntimeError, dict_={"test": "pass"}, doc=b'mytest')
 
     def test_exception_matches(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 HPyTracker ht;
                 HPy fun, fun_args;
                 HPy expected_exc_type;
                 HPy tmp;
                 HPy result;
 
@@ -670,15 +670,15 @@
         for exc_type in exc_types:
             res = mod.f(raise_exception, (exc_type, ), exc_types)
         with pytest.raises(DummyException):
             mod.f(raise_exception, (DummyException, ), exc_types)
 
     def test_HPyErr_WriteUnraisable(self, python_subprocess):
         mod = self.compile_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 HPyErr_SetString(ctx, ctx->h_ValueError, "error message");
                 HPyErr_WriteUnraisable(ctx, HPy_NULL);
                 return HPyBool_FromLong(ctx, HPyErr_Occurred(ctx));
             }
             @EXPORT(f)
@@ -688,7 +688,21 @@
             # if sys.executable is not available (e.g. inside pypy app-level)
             # tests, then skip the rest of this test
             return
         # subprocess is not importable in pypy app-level tests
         result = python_subprocess.run(mod, "mod.f()")
         assert result.returncode == 0
 
+
+    def test_HPyErr_Format(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(f, "f", HPyFunc_O)
+            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                return HPyErr_Format(ctx, ctx->h_ValueError, "Formatted '%S' and %d", arg, 42);
+            }
+            @EXPORT(f)
+            @INIT
+        """)
+        with pytest.raises(ValueError, match="Formatted 'error message' and 42"):
+            mod.f("error message")
```

### Comparing `hpy-0.0.4/test/test_hpyfield.py` & `hpy-0.9.0rc1/test/test_hpyfield.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
             } PairObject;
 
             HPyType_HELPERS(PairObject);
         """
 
     def DEFINE_Pair_new(self):
         return """
-            HPyDef_SLOT(Pair_new, Pair_new_impl, HPy_tp_new)
-            static HPy Pair_new_impl(HPyContext *ctx, HPy cls, HPy *args,
+            HPyDef_SLOT(Pair_new, HPy_tp_new)
+            static HPy Pair_new_impl(HPyContext *ctx, HPy cls, const HPy *args,
                                       HPy_ssize_t nargs, HPy kw)
             {
                 HPy a;
                 HPy b;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 PairObject *pair;
@@ -37,47 +37,47 @@
                 HPyField_Store(ctx, h_obj, &pair->b, b);
                 return h_obj;
             }
         """
 
     def DEFINE_Pair_traverse(self):
         return """
-            HPyDef_SLOT(Pair_traverse, Pair_traverse_impl, HPy_tp_traverse)
+            HPyDef_SLOT(Pair_traverse, HPy_tp_traverse)
             static int Pair_traverse_impl(void *self, HPyFunc_visitproc visit, void *arg)
             {
                 PairObject *p = (PairObject *)self;
                 HPy_VISIT(&p->a);
                 HPy_VISIT(&p->b);
                 return 0;
             }
         """
 
     def DEFINE_Pair_set_a(self):
         return """
-            HPyDef_METH(Pair_set_a, "set_a", Pair_set_a_impl, HPyFunc_O)
+            HPyDef_METH(Pair_set_a, "set_a", HPyFunc_O)
             static HPy Pair_set_a_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 PairObject *pair = PairObject_AsStruct(ctx, self);
                 HPyField_Store(ctx, self, &pair->a, arg);
                 return HPy_Dup(ctx, ctx->h_None);
             }
         """
 
     def DEFINE_Pair_get_ab(self):
         return """
-            HPyDef_METH(Pair_get_a, "get_a", Pair_get_a_impl, HPyFunc_NOARGS)
+            HPyDef_METH(Pair_get_a, "get_a", HPyFunc_NOARGS)
             static HPy Pair_get_a_impl(HPyContext *ctx, HPy self)
             {
                 PairObject *pair = PairObject_AsStruct(ctx, self);
                 if (HPy_IsNull(pair->a))
                     return HPyUnicode_FromString(ctx, "<NULL>");
                 return HPyField_Load(ctx, self, pair->a);
             }
 
-            HPyDef_METH(Pair_get_b, "get_b", Pair_get_b_impl, HPyFunc_NOARGS)
+            HPyDef_METH(Pair_get_b, "get_b", HPyFunc_NOARGS)
             static HPy Pair_get_b_impl(HPyContext *ctx, HPy self)
             {
                 PairObject *pair = PairObject_AsStruct(ctx, self);
                 if (HPy_IsNull(pair->b))
                     return HPyUnicode_FromString(ctx, "<NULL>");
                 return HPyField_Load(ctx, self, pair->b);
             }
@@ -204,15 +204,15 @@
             #include <assert.h>
             @DEFINE_PairObject
             @DEFINE_Pair_new
             @DEFINE_Pair_get_ab
             @DEFINE_Pair_traverse
             @DEFINE_Pair_set_a
 
-            HPyDef_METH(Pair_clear_a, "clear_a", Pair_clear_a_impl, HPyFunc_NOARGS)
+            HPyDef_METH(Pair_clear_a, "clear_a", HPyFunc_NOARGS)
             static HPy Pair_clear_a_impl(HPyContext *ctx, HPy self)
             {
                 PairObject *pair = PairObject_AsStruct(ctx, self);
                 HPyField_Store(ctx, self, &pair->a, HPy_NULL);
                 return HPy_Dup(ctx, ctx->h_None);
             }
 
@@ -329,15 +329,15 @@
             static void on_unexpected_finalize_call() {
                 if (test_finished)
                     abort();
                 else
                     unexpected_finalize_call = true;
             }
 
-            HPyDef_SLOT(Pair_finalize, Pair_finalize_impl, HPy_tp_finalize)
+            HPyDef_SLOT(Pair_finalize, HPy_tp_finalize)
             static void Pair_finalize_impl(HPyContext *ctx, HPy to_be_finalized)
             {
                 PairObject *pair = PairObject_AsStruct(ctx, to_be_finalized);
 
                 // Check that we were called on the right object: 'to_be_finalized'
                 HPy to_be_finalized_b = HPyField_Load(ctx, to_be_finalized, pair->b);
                 if (!HPy_Is(ctx, to_be_finalized_b, ctx->h_True)) {
@@ -388,15 +388,15 @@
                 on_unexpected_finalize_call();
             owner_cleanup:
                 HPy_Close(ctx, owner);
                 HPy_Close(ctx, owner_a);
                 HPy_Close(ctx, owner_b);
             }
 
-            HPyDef_METH(check_finalize_calls, "check_finalize_calls", check_finalize_calls_impl, HPyFunc_NOARGS)
+            HPyDef_METH(check_finalize_calls, "check_finalize_calls", HPyFunc_NOARGS)
             static HPy check_finalize_calls_impl(HPyContext *ctx, HPy self)
             {
                 test_finished = true;
                 if (!unexpected_finalize_call && saw_expected_finalize_call)
                     return HPy_Dup(ctx, ctx->h_True);
                 else
                     return HPy_Dup(ctx, ctx->h_False);
```

### Comparing `hpy-0.0.4/test/test_hpyglobal.py` & `hpy-0.9.0rc1/test/test_hpyglobal.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 class TestHPyGlobal(HPyTest):
 
     def test_basics(self):
         mod = self.make_module("""
             HPyGlobal myglobal;
 
-            HPyDef_METH(setg, "setg", setg_impl, HPyFunc_O)
+            HPyDef_METH(setg, "setg", HPyFunc_O)
             static HPy setg_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPyGlobal_Store(ctx, &myglobal, arg);
                 return HPy_Dup(ctx, ctx->h_None);
             }
 
-            HPyDef_METH(getg, "getg", getg_impl, HPyFunc_NOARGS)
+            HPyDef_METH(getg, "getg", HPyFunc_NOARGS)
             static HPy getg_impl(HPyContext *ctx, HPy self)
             {
                 return HPyGlobal_Load(ctx, myglobal);
             }
 
             @EXPORT(setg)
             @EXPORT(getg)
```

### Comparing `hpy-0.0.4/test/test_hpyimport.py` & `hpy-0.9.0rc1/test/test_hpyimport.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 class TestImport(HPyTest):
 
     def test_ImportModule(self):
         import pytest
         import sys
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy h_name)
             {
                 // we use bytes because ATM we don't have HPyUnicode_AsUTF8 or similar
-                char *name = HPyBytes_AsString(ctx, h_name);
+                const char *name = HPyBytes_AsString(ctx, h_name);
                 if (name == NULL)
                     return HPy_NULL;
                 return HPyImport_ImportModule(ctx, name);
             }
             @EXPORT(f)
             @INIT
         """)
```

### Comparing `hpy-0.0.4/test/test_hpylist.py` & `hpy-0.9.0rc1/test/test_hpylist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .support import HPyTest
 
 class TestList(HPyTest):
 
     def test_Check(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 if (HPyList_Check(ctx, arg))
                     return HPy_Dup(ctx, ctx->h_True);
                 return HPy_Dup(ctx, ctx->h_False);
             }
             @EXPORT(f)
@@ -19,27 +19,27 @@
 
         assert mod.f([]) is True
         assert mod.f('hello') is False
         assert mod.f(MyList()) is True
 
     def test_New(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_NOARGS)
+            HPyDef_METH(f, "f", HPyFunc_NOARGS)
             static HPy f_impl(HPyContext *ctx, HPy self)
             {
                 return HPyList_New(ctx, 0);
             }
             @EXPORT(f)
             @INIT
         """)
         assert mod.f() == []
 
     def test_Append(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy list = HPyList_New(ctx, 0);
                 if (HPy_IsNull(list))
                     return HPy_NULL;
                 if (HPyList_Append(ctx, list, arg) == -1)
                     return HPy_NULL;
@@ -50,15 +50,15 @@
             @EXPORT(f)
             @INIT
         """)
         assert mod.f(42) == [42, 42]
 
     def test_ListBuilder(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy h_self, HPy h_arg)
             {
                 HPyListBuilder builder = HPyListBuilder_New(ctx, 3);
                 HPyListBuilder_Set(ctx, builder, 0, h_arg);
                 HPyListBuilder_Set(ctx, builder, 1, ctx->h_True);
                 HPy h_num = HPyLong_FromLong(ctx, -42);
                 if (HPy_IsNull(h_num))
```

### Comparing `hpy-0.0.4/test/test_hpytype_legacy.py` & `hpy-0.9.0rc1/test/test_slots_legacy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,230 +1,265 @@
-""" HPyType tests on legacy types. """
+""" HPyType slot tests on legacy types. """
 
-import pytest
-from .support import HPyTest
-from .test_hpytype import PointTemplate, TestType as _TestType
+from .support import HPyTest, make_hpy_abi_fixture
+from .test_hpytype_legacy import LegacyPointTemplate
+from .test_slots import TestSlots as _TestSlots, TestSqSlots as _TestSqSlots
 
+hpy_abi = make_hpy_abi_fixture('with hybrid')
 
-class LegacyPointTemplate(PointTemplate):
-    """
-    Override PointTemplate to instead define a legacy point type that
-    still provides access to PyObject_HEAD.
-    """
-
-    _STRUCT_BEGIN_FORMAT = """
-        #include <Python.h>
-        typedef struct {{
-            PyObject_HEAD
-    """
-
-    _STRUCT_END_FORMAT = """
-        }} {struct_name};
-        HPyType_LEGACY_HELPERS({struct_name})
-    """
+class TestLegacySlots(_TestSlots):
+    ExtensionTemplate = LegacyPointTemplate
 
-    _IS_LEGACY = ".legacy = true,"
 
+class TestLegacySqSlots(_TestSqSlots):
+    ExtensionTemplate = LegacyPointTemplate
 
-class TestLegacyType(_TestType):
 
-    ExtensionTemplate = LegacyPointTemplate
+class TestCustomLegacySlotsFeatures(HPyTest):
 
-    @pytest.mark.syncgc
-    def test_legacy_dealloc(self):
+    def test_legacy_slots(self):
         mod = self.make_module("""
-            static long dealloc_counter = 0;
+            #include <Python.h>
 
-            HPyDef_METH(get_counter, "get_counter", get_counter_impl, HPyFunc_NOARGS)
-            static HPy get_counter_impl(HPyContext *ctx, HPy self)
+            static PyObject *Dummy_repr(PyObject *self)
             {
-                return HPyLong_FromLong(ctx, dealloc_counter);
+                return PyUnicode_FromString("myrepr");
             }
 
-            @DEFINE_PointObject
-            @DEFINE_Point_new
-            static void Point_dealloc(PyObject *self)
+            static PyObject *Dummy_add(PyObject *self, PyObject *other)
             {
-                dealloc_counter++;
-                Py_TYPE(self)->tp_free(self);
+                return Py_BuildValue("OO", self, other);
             }
 
-            static HPyDef *Point_defines[] = {&Point_new, NULL};
-            static PyType_Slot Point_slots[] = {
-                {Py_tp_dealloc, (void*)Point_dealloc},
-                {0, NULL},
+            HPyDef_SLOT(Dummy_abs, HPy_nb_absolute);
+            static HPy Dummy_abs_impl(HPyContext *ctx, HPy self)
+            {
+                return HPyLong_FromLong(ctx, 1234);
+            }
+
+            static HPyDef *Dummy_defines[] = {
+                &Dummy_abs,
+                NULL
             };
-            static HPyType_Spec Point_spec = {
-                .name = "mytest.Point",
-                .basicsize = sizeof(PointObject),
-                .legacy = true,
-                .legacy_slots = Point_slots,
-                .defines = Point_defines,
+            static PyType_Slot Dummy_type_slots[] = {
+                {Py_tp_repr, (void*)Dummy_repr},
+                {Py_nb_add, (void*)Dummy_add},
+                {0, 0},
+            };
+            static HPyType_Spec Dummy_spec = {
+                .name = "mytest.Dummy",
+                .builtin_shape = HPyType_BuiltinShape_Legacy,
+                .legacy_slots = Dummy_type_slots,
+                .defines = Dummy_defines
             };
 
-            @EXPORT(get_counter)
-            @EXPORT_TYPE("Point", Point_spec)
+            @EXPORT_TYPE("Dummy", Dummy_spec)
             @INIT
         """)
-        assert mod.get_counter() == 0
-        p = mod.Point(0, 0)
-        del p
-        import gc; gc.collect()
-        assert mod.get_counter() == 1
+        d = mod.Dummy()
+        assert repr(d) == 'myrepr'
+        assert d + 42 == (d, 42)
+        assert abs(d) == 1234
 
-    def test_legacy_dealloc_and_HPy_tp_traverse(self):
-        import pytest
-        mod_src = """
-            @DEFINE_PointObject
-            @DEFINE_Point_new
-            HPyDef_SLOT(Point_traverse, Point_traverse_impl, HPy_tp_traverse)
-            static int Point_traverse_impl(void *self, HPyFunc_visitproc visit, void *arg)
+    def test_legacy_slots_methods(self):
+        mod = self.make_module("""
+            #include <Python.h>
+
+            static PyObject *Dummy_foo(PyObject *self, PyObject *arg)
             {
-                return 0;
+                Py_INCREF(arg);
+                return arg;
             }
-            static void Point_dealloc(PyObject *self)
+
+            HPyDef_METH(Dummy_bar, "bar", HPyFunc_NOARGS)
+            static HPy Dummy_bar_impl(HPyContext *ctx, HPy self)
             {
-                return;
+                return HPyLong_FromLong(ctx, 1234);
             }
 
-            static HPyDef *Point_defines[] = {&Point_new, &Point_traverse, NULL};
-            static PyType_Slot Point_slots[] = {
-                {Py_tp_dealloc, (void*)Point_dealloc},
-                {0, NULL},
+            static PyMethodDef dummy_methods[] = {
+               {"foo", Dummy_foo, METH_O},
+               {NULL, NULL}         /* Sentinel */
             };
-            static HPyType_Spec Point_spec = {
-                .name = "mytest.Point",
-                .basicsize = sizeof(PointObject),
-                .legacy = true,
-                .legacy_slots = Point_slots,
-                .defines = Point_defines,
+
+            static PyType_Slot dummy_type_slots[] = {
+                {Py_tp_methods, dummy_methods},
+                {0, 0},
             };
-            @EXPORT_TYPE("Point", Point_spec)
+
+            static HPyDef *dummy_type_defines[] = {
+                    &Dummy_bar,
+                    NULL
+            };
+
+            static HPyType_Spec dummy_type_spec = {
+                .name = "mytest.Dummy",
+                .builtin_shape = HPyType_BuiltinShape_Legacy,
+                .legacy_slots = dummy_type_slots,
+                .defines = dummy_type_defines
+            };
+
+            @EXPORT_TYPE("Dummy", dummy_type_spec)
             @INIT
-        """
-        with pytest.raises(TypeError) as err:
-            mod = self.make_module(mod_src)
-        assert "legacy tp_dealloc" in str(err.value)
+        """)
+        d = mod.Dummy()
+        assert d.foo(21) == 21
+        assert d.bar() == 1234
 
-    def test_legacy_dealloc_and_HPy_tp_destroy(self):
+    def test_legacy_slots_members(self):
         import pytest
-        mod_src = """
-            @DEFINE_PointObject
-            @DEFINE_Point_new
-            HPyDef_SLOT(Point_destroy, Point_destroy_impl, HPy_tp_destroy)
-            static void Point_destroy_impl(void *obj)
-            {
-                return;
-            }
-            static void Point_dealloc(PyObject *self)
-            {
-                return;
-            }
+        mod = self.make_module("""
+            #include <Python.h>
+            #include "structmember.h"
 
-            static HPyDef *Point_defines[] = {&Point_new, &Point_destroy, NULL};
-            static PyType_Slot Point_slots[] = {
-                {Py_tp_dealloc, (void*)Point_dealloc},
-                {0, NULL},
+            typedef struct {
+                PyObject_HEAD
+                long x;
+                long y;
+            } PointObject;
+
+            HPyDef_SLOT(Point_new, HPy_tp_new)
+            static HPy Point_new_impl(HPyContext *ctx, HPy cls, const HPy *args,
+                                      HPy_ssize_t nargs, HPy kw)
+            {
+                PointObject *point;
+                HPy h_point = HPy_New(ctx, cls, &point);
+                if (HPy_IsNull(h_point))
+                    return HPy_NULL;
+                point->x = 7;
+                point->y = 3;
+                return h_point;
+            }
+
+            HPyDef_MEMBER(Point_x, "x", HPyMember_LONG, offsetof(PointObject, x))
+
+            // legacy members
+            static PyMemberDef legacy_members[] = {
+                {"y", T_LONG, offsetof(PointObject, y), 0},
+                {"y_ro", T_LONG, offsetof(PointObject, y), READONLY},
+                {NULL}
+            };
+
+            static PyType_Slot legacy_slots[] = {
+                {Py_tp_members, legacy_members},
+                {0, NULL}
+            };
+
+            static HPyDef *Point_defines[] = {
+                &Point_new,
+                &Point_x,
+                NULL
             };
             static HPyType_Spec Point_spec = {
                 .name = "mytest.Point",
                 .basicsize = sizeof(PointObject),
-                .legacy = true,
-                .legacy_slots = Point_slots,
-                .defines = Point_defines,
+                .builtin_shape = HPyType_BuiltinShape_Legacy,
+                .legacy_slots = legacy_slots,
+                .defines = Point_defines
             };
+
             @EXPORT_TYPE("Point", Point_spec)
             @INIT
-        """
-        with pytest.raises(TypeError) as err:
-            mod = self.make_module(mod_src)
-        assert "legacy tp_dealloc" in str(err.value)
-
-
-class TestCustomLegacyFeatures(HPyTest):
+        """)
+        p = mod.Point()
+        assert p.x == 7
+        assert p.y == 3
+        assert p.y_ro == 3
+        p.x = 123
+        p.y = 456
+        with pytest.raises(AttributeError):
+            p.y_ro = 789
+        assert p.x == 123
+        assert p.y == 456
 
-    def test_legacy_methods(self):
+    def test_legacy_slots_getsets(self):
         mod = self.make_module("""
             #include <Python.h>
 
-            static PyObject *f(PyObject *self, PyObject *args)
-            {
-                return PyLong_FromLong(1234);
-            }
-            static PyObject *g(PyObject *self, PyObject *arg)
-            {
-                long x = PyLong_AsLong(arg);
-                return PyLong_FromLong(x * 2);
-            }
-            static PyObject *h(PyObject *self, PyObject *args)
-            {
-                long a, b, c;
-                if (!PyArg_ParseTuple(args, "lll", &a, &b, &c))
-                    return NULL;
-                return PyLong_FromLong(100*a + 10*b + c);
-            }
-            static PyObject *k(PyObject *self, PyObject *args, PyObject *kwargs)
-            {
-                static const char *kwlist[] = { "a", "b", "c", NULL };
-                long a, b, c;
-                if (!PyArg_ParseTupleAndKeywords(args, kwargs, "lll", (char **)kwlist, &a, &b, &c))
-                    return NULL;
-                return PyLong_FromLong(100*a + 10*b + c);
-            }
-
-            static PyMethodDef my_legacy_methods[] = {
-                {"f", (PyCFunction)f, METH_NOARGS},
-                {"g", (PyCFunction)g, METH_O},
-                {"h", (PyCFunction)h, METH_VARARGS},
-                {"k", (PyCFunction)k, METH_VARARGS | METH_KEYWORDS},
+            typedef struct {
+                PyObject_HEAD
+                long x;
+                long y;
+            } PointObject;
+
+            HPyDef_SLOT(Point_new, HPy_tp_new)
+            static HPy Point_new_impl(HPyContext *ctx, HPy cls, const HPy *args,
+                                      HPy_ssize_t nargs, HPy kw)
+            {
+                PointObject *point;
+                HPy h_point = HPy_New(ctx, cls, &point);
+                if (HPy_IsNull(h_point))
+                    return HPy_NULL;
+                point->x = 7;
+                point->y = 3;
+                return h_point;
+            }
+
+            static PyObject *z_get(PointObject *point, void *closure)
+            {
+                long z = point->x*10 + point->y + (long)(HPy_ssize_t)closure;
+                return PyLong_FromLong(z);
+            }
+
+            // legacy getsets
+            static PyGetSetDef legacy_getsets[] = {
+                {"z", (getter)z_get, NULL, NULL, (void *)2000},
                 {NULL}
             };
 
-            @EXPORT_LEGACY(my_legacy_methods)
+            static PyType_Slot legacy_slots[] = {
+                {Py_tp_getset, legacy_getsets},
+                {0, NULL}
+            };
+
+            static HPyDef *Point_defines[] = {
+                &Point_new,
+                NULL
+            };
+            static HPyType_Spec Point_spec = {
+                .name = "mytest.Point",
+                .basicsize = sizeof(PointObject),
+                .builtin_shape = HPyType_BuiltinShape_Legacy,
+                .legacy_slots = legacy_slots,
+                .defines = Point_defines
+            };
+
+            @EXPORT_TYPE("Point", Point_spec)
             @INIT
         """)
-        assert mod.f() == 1234
-        assert mod.g(45) == 90
-        assert mod.h(4, 5, 6) == 456
-        assert mod.k(c=6, b=5, a=4) == 456
+        p = mod.Point()
+        assert p.z == 2073
 
-    def test_legacy_inherits_from_pure_raises(self):
+    def test_legacy_slots_fails_without_legacy(self):
         import pytest
         mod_src = """
-            static HPyType_Spec PureType_spec = {
-                .name = "mytest.PureType",
-                .flags = HPy_TPFLAGS_DEFAULT | HPy_TPFLAGS_BASETYPE,
-            };
-
-            static HPyType_Spec LegacyType_spec = {
-                .name = "mytest.LegacyType",
-                .legacy = true,
-            };
-
-            static void make_Types(HPyContext *ctx, HPy module)
-            {
-                HPy h_PureType = HPyType_FromSpec(ctx, &PureType_spec, NULL);
-                if (HPy_IsNull(h_PureType)) {
-                    return;
-                }
-
-                HPyType_SpecParam LegacyType_param[] = {
-                    { HPyType_SpecParam_Base, h_PureType },
-                    { (HPyType_SpecParam_Kind)0 }
-                };
-                HPy h_LegacyType = HPyType_FromSpec(
-                    ctx, &LegacyType_spec, LegacyType_param);
-                if (HPy_IsNull(h_LegacyType)) {
-                    HPy_Close(ctx, h_PureType);
-                    return;
-                }
-                HPy_Close(ctx, h_LegacyType);
-                HPy_Close(ctx, h_PureType);
+            #include <Python.h>
+
+            static PyObject *Dummy_foo(PyObject *self, PyObject *arg)
+            {
+                Py_INCREF(arg);
+                return arg;
             }
-            @EXTRA_INIT_FUNC(make_Types)
+
+            static PyMethodDef dummy_methods[] = {
+               {"foo", Dummy_foo, METH_O},
+               {NULL, NULL}         /* Sentinel */
+            };
+
+            static PyType_Slot dummy_type_slots[] = {
+                {Py_tp_methods, dummy_methods},
+                {0, 0},
+            };
+
+            static HPyType_Spec dummy_type_spec = {
+                .name = "mytest.Dummy",
+                .builtin_shape = HPyType_BuiltinShape_Object,
+                .legacy_slots = dummy_type_slots,
+            };
+
+            @EXPORT_TYPE("Dummy", dummy_type_spec)
             @INIT
         """
         with pytest.raises(TypeError) as err:
             self.make_module(mod_src)
         assert str(err.value) == (
-            "A legacy type should not inherit its memory layout from a"
-            " pure type")
+            "cannot specify .legacy_slots without setting .builtin_shape=HPyType_BuiltinShape_Legacy")
```

### Comparing `hpy-0.0.4/test/test_importing.py` & `hpy-0.9.0rc1/test/test_importing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,15 @@
+import pytest
 from .support import HPyTest
+from hpy.devel.abitag import get_hpy_ext_suffix
+
+@pytest.fixture(params=['cpython', 'universal', 'hybrid', 'debug'])
+def hpy_abi(request):
+    abi = request.param
+    yield abi
 
 
 class TestImporting(HPyTest):
 
     def full_import(self, name, mod_filename):
         import importlib
         import sys
@@ -37,15 +44,12 @@
         assert mod.__package__ == ''
         assert mod.__doc__ == 'some test for hpy'
         assert mod.__loader__.name == 'mytest'
         assert mod.__spec__.loader is mod.__loader__
         assert mod.__spec__.name == 'mytest'
         assert mod.__file__
 
-        if hpy_abi == 'cpython':
-            from sysconfig import get_config_var
-            ext = get_config_var('EXT_SUFFIX')
-        else:
-            ext = '.hpy.so'
-
+        if hpy_abi == 'debug':
+            hpy_abi = 'universal'
+        ext_suffix = get_hpy_ext_suffix(hpy_abi)
         assert repr(mod) == '<module \'mytest\' from {}>'.format(
-            repr(str(tmpdir.join('mytest' + ext))))
+            repr(str(tmpdir.join('mytest' + ext_suffix))))
```

### Comparing `hpy-0.0.4/test/test_number.py` & `hpy-0.9.0rc1/test/test_number.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,62 @@
 from .support import HPyTest
 
 
 class TestNumber(HPyTest):
 
-    def test_bool_from_long(self):
+    def test_bool_from_bool_and_long(self):
+        import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
+            HPyDef_METH(from_bool, "from_bool", HPyFunc_O)
+            static HPy from_bool_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                int32_t x = HPyLong_AsInt32_t(ctx, arg);
+                if (x == -1 && HPyErr_Occurred(ctx))
+                    return HPy_NULL;
+                if (x != 0 && x != 1) {
+                    HPyErr_SetString(ctx, ctx->h_ValueError,
+                                         "value must be 0 or 1");
+                    return HPy_NULL;
+                }
+                return HPyBool_FromBool(ctx, (x ? true : false));
+            }
+
+            HPyDef_METH(from_long, "from_long", HPyFunc_O)
+            static HPy from_long_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 long x = HPyLong_AsLong(ctx, arg);
-                if (HPyErr_Occurred(ctx))
+                if (x == -1 && HPyErr_Occurred(ctx))
                     return HPy_NULL;
                 return HPyBool_FromLong(ctx, x);
             }
-            @EXPORT(f)
+            @EXPORT(from_bool)
+            @EXPORT(from_long)
             @INIT
         """)
-        assert mod.f(0) is False
-        assert mod.f(42) is True
+        assert mod.from_bool(0) is False
+        assert mod.from_bool(1) is True
+        with pytest.raises(ValueError):
+            mod.from_bool(2)
+        assert mod.from_long(0) is False
+        assert mod.from_long(42) is True
 
     def test_unary(self):
         import pytest
         import operator
         for c_name, op in [
                 ('Negative', operator.neg),
                 ('Positive', operator.pos),
                 ('Absolute', abs),
                 ('Invert', operator.invert),
                 ('Index', operator.index),
                 ('Long', int),
                 ('Float', float),
                 ]:
             mod = self.make_module("""
-                HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+                HPyDef_METH(f, "f", HPyFunc_O)
                 static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
                 {
                     return HPy_%s(ctx, arg);
                 }
                 @EXPORT(f)
                 @INIT
             """ % (c_name,), name='number_'+c_name)
@@ -63,34 +83,34 @@
                 ('Lshift', operator.lshift),
                 ('Rshift', operator.rshift),
                 ('And', operator.and_),
                 ('Xor', operator.xor),
                 ('Or', operator.or_),
                 ]:
             mod = self.make_module("""
-                HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+                HPyDef_METH(f, "f", HPyFunc_VARARGS)
                 static HPy f_impl(HPyContext *ctx, HPy self,
-                                  HPy *args, HPy_ssize_t nargs)
+                                  const HPy *args, size_t nargs)
                 {
                     HPy a, b;
                     if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                         return HPy_NULL;
                     return HPy_%s(ctx, a, b);
                 }
                 @EXPORT(f)
                 @INIT
             """ % (c_name,), name='number_'+c_name)
             assert mod.f(5, 4) == op(5, 4)
             assert mod.f(6, 3) == op(6, 3)
 
     def test_power(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b, c;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OOO", &a, &b, &c))
                     return HPy_NULL;
                 return HPy_Power(ctx, a, b, c);
             }
             @EXPORT(f)
@@ -102,17 +122,17 @@
     def test_matmul(self):
         class Mat:
             def __matmul__(self, other):
                 return ('matmul', self, other)
         m1 = Mat()
         m2 = Mat()
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 return HPy_MatrixMultiply(ctx, a, b);
             }
             @EXPORT(f)
@@ -132,17 +152,17 @@
                 ('Lshift', '__ilshift__'),
                 ('Rshift', '__irshift__'),
                 ('And', '__iand__'),
                 ('Xor', '__ixor__'),
                 ('Or', '__ior__'),
                 ]:
             mod = self.make_module("""
-                HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+                HPyDef_METH(f, "f", HPyFunc_VARARGS)
                 static HPy f_impl(HPyContext *ctx, HPy self,
-                                  HPy *args, HPy_ssize_t nargs)
+                                  const HPy *args, size_t nargs)
                 {
                     HPy a, b;
                     if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                         return HPy_NULL;
                     return HPy_InPlace%s(ctx, a, b);
                 }
                 @EXPORT(f)
@@ -152,17 +172,17 @@
                 def mymethod(self, b):
                     return (py_name, b)
             setattr(A, py_name, A.mymethod)
             assert mod.f(A(), 12.34) == A().mymethod(12.34)
 
     def test_inplace_power(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b, c;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OOO", &a, &b, &c))
                     return HPy_NULL;
                 return HPy_InPlacePower(ctx, a, b, c);
             }
             @EXPORT(f)
@@ -181,31 +201,31 @@
     def test_inplace_matmul(self):
         class Mat:
             def __imatmul__(self, other):
                 return ('imatmul', self, other)
         m1 = Mat()
         m2 = Mat()
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 HPy a, b;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 return HPy_InPlaceMatrixMultiply(ctx, a, b);
             }
             @EXPORT(f)
             @INIT
         """)
         assert mod.f(m1, m2) == m1.__imatmul__(m2)
 
     def test_number_check(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 int cond = HPyNumber_Check(ctx, arg);
                 return HPyLong_FromLong(ctx, cond);
             }
             @EXPORT(f)
             @INIT
```

### Comparing `hpy-0.0.4/test/test_object.py` & `hpy-0.9.0rc1/test/test_object.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .support import HPyTest
 
 
 class TestObject(HPyTest):
     def test_getattr(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy name, result;
                 name = HPyUnicode_FromString(ctx, "foo");
                 if (HPy_IsNull(name))
                     return HPy_NULL;
                 result = HPy_GetAttr(ctx, arg, name);
@@ -51,15 +51,15 @@
         assert mod.f(ClassAttr) == 10
         assert mod.f(ClassAttr()) == 10
         assert mod.f(PropAttr()) == 11
 
     def test_getattr_s(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy result;
                 result = HPy_GetAttr_s(ctx, arg, "foo");
                 if (HPy_IsNull(result))
                     return HPy_NULL;
                 return result;
@@ -88,15 +88,15 @@
             mod.f(42)
         assert mod.f(ClassAttr) == 10
         assert mod.f(ClassAttr()) == 10
         assert mod.f(PropAttr()) == 11
 
     def test_hasattr(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy name;
                 int result;
                 name = HPyUnicode_FromString(ctx, "foo");
                 if (HPy_IsNull(name))
                     return HPy_NULL;
@@ -138,15 +138,15 @@
         assert mod.f(ClassAttr()) is True
         assert mod.f(PropAttr()) is True
         assert mod.f(PropAttrRaising()) is False
 
 
     def test_hasattr_s(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 int result;
                 result = HPy_HasAttr_s(ctx, arg, "foo");
                 if (result == -1)
                     return HPy_NULL;
                 if (result)
@@ -182,15 +182,15 @@
         assert mod.f(ClassAttr()) is True
         assert mod.f(PropAttr()) is True
         assert mod.f(PropAttrRaising()) is False
 
     def test_setattr(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy name;
                 int result;
                 name = HPyUnicode_FromString(ctx, "foo");
                 if (HPy_IsNull(name))
                     return HPy_NULL;
@@ -241,15 +241,15 @@
         b = WritablePropAttr()
         mod.f(b)
         assert b.foo is True
 
     def test_setattr_s(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 int result;
                 result = HPy_SetAttr_s(ctx, arg, "foo", ctx->h_True);
                 if (result < 0)
                     return HPy_NULL;
                 return HPy_Dup(ctx, ctx->h_None);
@@ -292,18 +292,177 @@
         with pytest.raises(AttributeError):
             mod.f(ReadOnlyPropAttr())
 
         b = WritablePropAttr()
         mod.f(b)
         assert b.foo is True
 
+    def test_delattr(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(del_foo, "del_foo", HPyFunc_O)
+            static HPy del_foo_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                HPy name;
+                int result;
+                name = HPyUnicode_FromString(ctx, "foo");
+                if (HPy_IsNull(name))
+                    return HPy_NULL;
+                result = HPy_DelAttr(ctx, arg, name);
+                HPy_Close(ctx, name);
+                if (result < 0)
+                    return HPy_NULL;
+                return HPy_Dup(ctx, ctx->h_None);
+            }
+            @EXPORT(del_foo)
+            @INIT
+        """)
+
+        class Attrs:
+            pass
+
+        class ClassAttr:
+            pass
+
+        class WritablePropAttr:
+            @property
+            def foo(self):
+                return self._foo
+
+            @foo.setter
+            def foo(self, value):
+                self._foo = value
+
+        class DeletablePropAttr:
+            @property
+            def foo(self):
+                return self._foo
+
+            @foo.setter
+            def foo(self, value):
+                self._foo = value
+
+            @foo.deleter
+            def foo(self):
+                del self._foo
+
+        def set_foo(obj):
+            obj.foo = True
+
+        a = Attrs()
+        set_foo(a)
+        assert a.foo is True
+        mod.del_foo(a)
+        with pytest.raises(AttributeError):
+            a.foo
+
+        set_foo(ClassAttr)
+        assert ClassAttr.foo is True
+        assert ClassAttr().foo is True
+        mod.del_foo(ClassAttr)
+        with pytest.raises(AttributeError):
+            ClassAttr.foo
+        with pytest.raises(AttributeError):
+            ClassAttr().foo
+
+        b = WritablePropAttr()
+        set_foo(b)
+        assert b.foo is True
+        with pytest.raises(AttributeError):
+            # does not provide a delete function, so it fails
+            mod.del_foo(b)
+
+        c = DeletablePropAttr()
+        set_foo(c)
+        assert c.foo is True
+        mod.del_foo(c)
+        with pytest.raises(AttributeError):
+            c.foo
+
+    def test_delattr_s(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(del_foo, "del_foo", HPyFunc_O)
+            static HPy del_foo_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                int result;
+                result = HPy_DelAttr_s(ctx, arg, "foo");
+                if (result < 0)
+                    return HPy_NULL;
+                return HPy_Dup(ctx, ctx->h_None);
+            }
+            @EXPORT(del_foo)
+            @INIT
+        """)
+
+        class Attrs:
+            pass
+
+        class ClassAttr:
+            pass
+
+        class WritablePropAttr:
+            @property
+            def foo(self):
+                return self._foo
+
+            @foo.setter
+            def foo(self, value):
+                self._foo = value
+
+        class DeletablePropAttr:
+            @property
+            def foo(self):
+                return self._foo
+
+            @foo.setter
+            def foo(self, value):
+                self._foo = value
+
+            @foo.deleter
+            def foo(self):
+                del self._foo
+
+        def set_foo(obj):
+            obj.foo = True
+
+        a = Attrs()
+        set_foo(a)
+        assert a.foo is True
+        mod.del_foo(a)
+        with pytest.raises(AttributeError):
+            a.foo
+
+        set_foo(ClassAttr)
+        assert ClassAttr.foo is True
+        assert ClassAttr().foo is True
+        mod.del_foo(ClassAttr)
+        with pytest.raises(AttributeError):
+            ClassAttr.foo
+        with pytest.raises(AttributeError):
+            ClassAttr().foo
+
+        b = WritablePropAttr()
+        set_foo(b)
+        assert b.foo is True
+        with pytest.raises(AttributeError):
+            # does not provide a delete function, so it fails
+            mod.del_foo(b)
+
+        c = DeletablePropAttr()
+        set_foo(c)
+        assert c.foo is True
+        mod.del_foo(c)
+        with pytest.raises(AttributeError):
+            c.foo
+
     def test_getitem(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy key, result;
                 key = HPyLong_FromLong(ctx, 3);
                 if (HPy_IsNull(key))
                     return HPy_NULL;
                 result = HPy_GetItem(ctx, arg, key);
@@ -323,15 +482,15 @@
         assert mod.f([0, 1, 2, "hello"]) == "hello"
         with pytest.raises(IndexError):
             mod.f([])
 
     def test_getitem_i(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy result;
                 result = HPy_GetItem_i(ctx, arg, 3);
                 if (HPy_IsNull(result))
                     return HPy_NULL;
                 return result;
@@ -347,15 +506,15 @@
         assert mod.f([0, 1, 2, "hello"]) == "hello"
         with pytest.raises(IndexError):
             mod.f([])
 
     def test_getitem_s(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy result;
                 result = HPy_GetItem_s(ctx, arg, "limes");
                 if (HPy_IsNull(result))
                     return HPy_NULL;
                 return result;
@@ -370,15 +529,15 @@
 
         with pytest.raises(TypeError):
             mod.f([])
 
     def test_setitem(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy key;
                 int result;
                 key = HPyLong_FromLong(ctx, 3);
                 if (HPy_IsNull(key))
                     return HPy_NULL;
@@ -398,15 +557,15 @@
         assert mod.f([0, 1, 2, False]) == [0, 1, 2, True]
         with pytest.raises(IndexError):
             mod.f([])
 
     def test_setitem_i(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 int result;
                 result = HPy_SetItem_i(ctx, arg, 3, ctx->h_True);
                 if (result < 0)
                     return HPy_NULL;
                 return HPy_Dup(ctx, arg);
@@ -421,15 +580,15 @@
         assert mod.f([0, 1, 2, False]) == [0, 1, 2, True]
         with pytest.raises(IndexError):
             mod.f([])
 
     def test_setitem_s(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 int result;
                 result = HPy_SetItem_s(ctx, arg, "limes", ctx->h_True);
                 if (result < 0)
                     return HPy_NULL;
                 return HPy_Dup(ctx, arg);
@@ -440,17 +599,89 @@
         assert mod.f({}) == {"limes": True}
         assert mod.f({"a": 1}) == {"a": 1, "limes": True}
         assert mod.f({"limes": False}) == {"limes": True}
 
         with pytest.raises(TypeError):
             mod.f([])
 
+    def test_delitem(self):
+        import pytest
+        mod = self.make_module("""
+            HPyDef_METH(delitem3, "delitem3", HPyFunc_O)
+            static HPy delitem3_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                HPy key;
+                int result;
+                key = HPyLong_FromLong(ctx, 3);
+                if (HPy_IsNull(key))
+                    return HPy_NULL;
+                result = HPy_DelItem(ctx, arg, key);
+                HPy_Close(ctx, key);
+                if (result < 0)
+                    return HPy_NULL;
+                return HPy_Dup(ctx, arg);
+            }
+            
+            HPyDef_METH(delitem_i3, "delitem_i3", HPyFunc_O)
+            static HPy delitem_i3_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                int result;
+                result = HPy_DelItem_i(ctx, arg, 3);
+                if (result < 0)
+                    return HPy_NULL;
+                return HPy_Dup(ctx, arg);
+            }
+            
+            HPyDef_METH(delitem_s3, "delitem_s3", HPyFunc_O)
+            static HPy delitem_s3_impl(HPyContext *ctx, HPy self, HPy arg)
+            {
+                int result;
+                result = HPy_DelItem_s(ctx, arg, "3");
+                if (result < 0)
+                    return HPy_NULL;
+                return HPy_Dup(ctx, arg);
+            }
+            
+            @EXPORT(delitem3)
+            @EXPORT(delitem_i3)
+            @EXPORT(delitem_s3)
+            @INIT
+        """)
+        # HPy_DelItem
+        assert mod.delitem3({3: False, 4: True}) == {4: True}
+        with pytest.raises(KeyError):
+            mod.delitem3({})
+        with pytest.raises(TypeError):
+            mod.delitem3((1, 2, 3, 4))
+        assert mod.delitem3([0, 1, 2, False]) == [0, 1, 2]
+        with pytest.raises(IndexError):
+            mod.delitem3([])
+
+        # HPy_DelItem_i
+        assert mod.delitem_i3({3: False, 4: True}) == {4: True}
+        with pytest.raises(KeyError):
+            mod.delitem_i3({})
+        with pytest.raises(TypeError):
+            mod.delitem_i3((1, 2, 3, 4))
+        assert mod.delitem_i3([0, 1, 2, False]) == [0, 1, 2]
+        with pytest.raises(IndexError):
+            mod.delitem_i3([])
+
+        # HPy_DelItem_s
+        assert mod.delitem_s3({'3': False, '4': True}) == {'4': True}
+        with pytest.raises(KeyError):
+            mod.delitem_s3({})
+        with pytest.raises(TypeError):
+            mod.delitem_s3((1, 2, 3, 4))
+        with pytest.raises(TypeError):
+            mod.delitem_s3([1, 2, 3, 4])
+
     def test_length(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 HPy_ssize_t result;
                 result = HPy_Length(ctx, arg);
                 if (result < 0)
                     return HPy_NULL;
                 return HPyLong_FromSsize_t(ctx, result);
@@ -459,16 +690,16 @@
             @INIT
         """)
         assert mod.f([5,6,7,8]) == 4
         assert mod.f({"a": 1}) == 1
 
     def test_contains(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 int result = HPy_Contains(ctx, args[0], args[1]);
                 if (result == -1) {
                     return HPy_NULL;
                 }
                 return HPyLong_FromLong(ctx, result);
             }
@@ -512,42 +743,42 @@
 
     def test_dump(self):
         # _HPy_Dump is supposed to be used e.g. inside a gdb session: it
         # prints various about the given handle to stdout, and it's
         # implementation-specific. As such, it's hard to write a meaningful
         # test: let's just call it an check it doesn't crash.
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 _HPy_Dump(ctx, arg);
                 return HPy_Dup(ctx, ctx->h_None);
             }
             @EXPORT(f)
             @INIT
         """)
         mod.f('hello')
 
     def test_type(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_O)
+            HPyDef_METH(f, "f", HPyFunc_O)
             static HPy f_impl(HPyContext *ctx, HPy self, HPy arg)
             {
                 return HPy_Type(ctx, arg);
             }
             @EXPORT(f)
             @INIT
         """)
         assert mod.f('hello') is str
         assert mod.f(42) is int
 
     def test_typecheck(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 HPy a, b;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &a, &b))
                     return HPy_NULL;
                 int res = HPy_TypeCheck(ctx, a, b);
                 return HPyBool_FromLong(ctx, res);
             }
@@ -558,16 +789,16 @@
             pass
         assert mod.f('hello', str)
         assert not mod.f('hello', int)
         assert mod.f(MyStr('hello'), str)
 
     def test_is(self):
         mod = self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
-            static HPy f_impl(HPyContext *ctx, HPy self, HPy *args, HPy_ssize_t nargs)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
+            static HPy f_impl(HPyContext *ctx, HPy self, const HPy *args, size_t nargs)
             {
                 HPy obj, other;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "OO", &obj, &other))
                     return HPy_NULL;
                 int res = HPy_Is(ctx, obj, other);
                 return HPyBool_FromLong(ctx, res);
             }
```

### Comparing `hpy-0.0.4/test/test_slots.py` & `hpy-0.9.0rc1/test/test_slots.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
     ExtensionTemplate = PointTemplate
 
     def test_tp_init(self):
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_xy
-            HPyDef_SLOT(Point_new, HPyType_GenericNew, HPy_tp_new)
+            HPyDef_SLOT_IMPL(Point_new, HPyType_GenericNew, HPy_tp_new)
 
-            HPyDef_SLOT(Point_init, Point_init_impl, HPy_tp_init)
-            static int Point_init_impl(HPyContext *ctx, HPy self, HPy *args,
+            HPyDef_SLOT(Point_init, HPy_tp_init)
+            static int Point_init_impl(HPyContext *ctx, HPy self, const HPy *args,
                                        HPy_ssize_t nargs, HPy kw)
             {
                 long x, y;
                 if (!HPyArg_Parse(ctx, NULL, args, nargs, "ll", &x, &y))
                     return -1;
 
                 PointObject *p = PointObject_AsStruct(ctx, self);
@@ -39,22 +39,22 @@
         import gc
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
 
             static long destroyed_x;
 
-            HPyDef_SLOT(Point_destroy, Point_destroy_impl, HPy_tp_destroy)
+            HPyDef_SLOT(Point_destroy, HPy_tp_destroy)
             static void Point_destroy_impl(void *obj)
             {
                 PointObject *point = (PointObject *)obj;
                 destroyed_x += point->x;
             }
 
-            HPyDef_METH(get_destroyed_x, "get_destroyed_x", get_destroyed_x_impl, HPyFunc_NOARGS)
+            HPyDef_METH(get_destroyed_x, "get_destroyed_x", HPyFunc_NOARGS)
             static HPy get_destroyed_x_impl(HPyContext *ctx, HPy self)
             {
                 return HPyLong_FromLong(ctx, destroyed_x);
             }
 
             @EXPORT_POINT_TYPE(&Point_new, &Point_destroy)
             @EXPORT(get_destroyed_x)
@@ -73,22 +73,22 @@
         import gc
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
 
             static long finalized_x;
 
-            HPyDef_SLOT(Point_finalize, Point_finalize_impl, HPy_tp_finalize)
+            HPyDef_SLOT(Point_finalize, HPy_tp_finalize)
             static void Point_finalize_impl(HPyContext *ctx, HPy obj)
             {
                 PointObject *point = PointObject_AsStruct(ctx, obj);
                 finalized_x += point->x;
             }
 
-            HPyDef_METH(get_finalized_x, "get_finalized_x", get_finalized_x_impl, HPyFunc_NOARGS)
+            HPyDef_METH(get_finalized_x, "get_finalized_x", HPyFunc_NOARGS)
             static HPy get_finalized_x_impl(HPyContext *ctx, HPy self)
             {
                 return HPyLong_FromLong(ctx, finalized_x);
             }
 
             @EXPORT_POINT_TYPE(&Point_new, &Point_finalize)
             @EXPORT(get_finalized_x)
@@ -107,39 +107,39 @@
         import gc
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
 
             static long finalized_x;
 
-            HPyDef_SLOT(Point_finalize, Point_finalize_impl, HPy_tp_finalize)
+            HPyDef_SLOT(Point_finalize, HPy_tp_finalize)
             static void Point_finalize_impl(HPyContext *ctx, HPy obj)
             {
                 PointObject *point = PointObject_AsStruct(ctx, obj);
                 finalized_x += point->x;
             }
 
-            HPyDef_SLOT(Point_traverse, Point_traverse_impl, HPy_tp_traverse)
+            HPyDef_SLOT(Point_traverse, HPy_tp_traverse)
             static int Point_traverse_impl(void *self, HPyFunc_visitproc visit, void *arg)
             {
                 return 0;
             }
 
             static HPyDef *Point_defines[] = {
                 &Point_new, &Point_finalize, &Point_traverse, NULL};
             static HPyType_Spec Point_spec = {
                 .name = "mytest.Point",
                 .basicsize = sizeof(PointObject),
                 .flags = HPy_TPFLAGS_DEFAULT | HPy_TPFLAGS_HAVE_GC,
-                .legacy = PointObject_IS_LEGACY,
+                .builtin_shape = SHAPE(PointObject),
                 .defines = Point_defines,
             };
             @EXPORT_TYPE("Point", Point_spec)
 
-            HPyDef_METH(get_finalized_x, "get_finalized_x", get_finalized_x_impl, HPyFunc_NOARGS)
+            HPyDef_METH(get_finalized_x, "get_finalized_x", HPyFunc_NOARGS)
             static HPy get_finalized_x_impl(HPyContext *ctx, HPy self)
             {
                 return HPyLong_FromLong(ctx, finalized_x);
             }
 
             @EXPORT(get_finalized_x)
             @INIT
@@ -154,15 +154,15 @@
 
     def test_nb_ops_binary(self):
         import operator
         mod = self.make_module(r"""
             @DEFINE_PointObject
 
             #define MYSLOT(NAME)                                               \
-                HPyDef_SLOT(p_##NAME, NAME##_impl, HPy_nb_##NAME);             \
+                HPyDef_SLOT_IMPL(p_##NAME, NAME##_impl, HPy_nb_##NAME)             \
                 static HPy NAME##_impl(HPyContext *ctx, HPy self, HPy other)    \
                 {                                                              \
                     HPy s = HPyUnicode_FromString(ctx, #NAME);                 \
                     HPy res = HPyTuple_Pack(ctx, 3, self, s, other);           \
                     HPy_Close(ctx, s);                                         \
                     return res;                                                \
                 }
@@ -202,15 +202,15 @@
 
     def test_nb_ops_inplace(self):
         import operator
         mod = self.make_module(r"""
             @DEFINE_PointObject
 
             #define MYSLOT(NAME)                                               \
-                HPyDef_SLOT(p_##NAME, NAME##_impl, HPy_nb_##NAME);             \
+                HPyDef_SLOT_IMPL(p_##NAME, NAME##_impl, HPy_nb_##NAME);             \
                 static HPy NAME##_impl(HPyContext *ctx, HPy self, HPy other)    \
                 {                                                              \
                     HPy s = HPyUnicode_FromString(ctx, #NAME);                 \
                     HPy res = HPyTuple_Pack(ctx, 3, self, s, other);           \
                     HPy_Close(ctx, s);                                         \
                     return res;                                                \
                 }
@@ -250,15 +250,15 @@
         assert tmp == (p, "inplace_matrix_multiply", 42)
 
     def test_nb_ops_unary(self):
         mod = self.make_module(r"""
             @DEFINE_PointObject
 
             #define MYSLOT(NAME)                                               \
-                HPyDef_SLOT(p_##NAME, NAME##_impl, HPy_nb_##NAME);             \
+                HPyDef_SLOT_IMPL(p_##NAME, NAME##_impl, HPy_nb_##NAME);             \
                 static HPy NAME##_impl(HPyContext *ctx, HPy self)               \
                 {                                                              \
                     HPy s = HPyUnicode_FromString(ctx, #NAME);                 \
                     HPy res = HPyTuple_Pack(ctx, 2, s, self);                  \
                     HPy_Close(ctx, s);                                         \
                     return res;                                                \
                 }
@@ -279,33 +279,33 @@
 
     def test_nb_ops_type_conversion(self):
         import operator
         mod = self.make_module(r"""
             @DEFINE_PointObject
             @DEFINE_Point_new
 
-            HPyDef_SLOT(p_int, p_int_impl, HPy_nb_int);
+            HPyDef_SLOT(p_int, HPy_nb_int);
             static HPy p_int_impl(HPyContext *ctx, HPy self)
             {
                 return HPyLong_FromLong(ctx, 42);
             }
 
-            HPyDef_SLOT(p_float, p_float_impl, HPy_nb_float);
+            HPyDef_SLOT(p_float, HPy_nb_float);
             static HPy p_float_impl(HPyContext *ctx, HPy self)
             {
                 return HPyFloat_FromDouble(ctx, 123.4);
             }
 
-            HPyDef_SLOT(p_index, p_index_impl, HPy_nb_index);
+            HPyDef_SLOT(p_index, HPy_nb_index);
             static HPy p_index_impl(HPyContext *ctx, HPy self)
             {
                 return HPyLong_FromLong(ctx, -456);
             }
 
-            HPyDef_SLOT(p_bool, p_bool_impl, HPy_nb_bool);
+            HPyDef_SLOT(p_bool, HPy_nb_bool);
             static int p_bool_impl(HPyContext *ctx, HPy self)
             {
                 PointObject *point = PointObject_AsStruct(ctx, self);
                 return (point->x != 0);
             }
 
             @EXPORT_POINT_TYPE(&Point_new, &p_int, &p_float, &p_index, &p_bool)
@@ -319,24 +319,24 @@
         assert bool(mod.Point(0, 0)) is False
         assert bool(mod.Point(1, 0)) is True
 
     def test_nb_ops_power(self):
         mod = self.make_module(r"""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(p_power, p_power_impl, HPy_nb_power);
+            HPyDef_SLOT(p_power, HPy_nb_power);
             static HPy p_power_impl(HPyContext *ctx, HPy self, HPy x, HPy y)
             {
                 HPy s = HPyUnicode_FromString(ctx, "power");
                 HPy res = HPyTuple_Pack(ctx, 4, self, s, x, y);
                 HPy_Close(ctx, s);
                 return res;
             }
 
-            HPyDef_SLOT(p_inplace_power, p_inplace_power_impl, HPy_nb_inplace_power);
+            HPyDef_SLOT(p_inplace_power, HPy_nb_inplace_power);
             static HPy p_inplace_power_impl(HPyContext *ctx, HPy self, HPy x, HPy y)
             {
                 HPy s = HPyUnicode_FromString(ctx, "inplace_power");
                 HPy res = HPyTuple_Pack(ctx, 4, self, s, x, y);
                 HPy_Close(ctx, s);
                 return res;
             }
@@ -359,15 +359,15 @@
                 int exports;
             @TYPE_STRUCT_END
 
             static char static_mem[12] = {0,1,2,3,4,5,6,7,8,9,10,11};
             static HPy_ssize_t _shape[1] = {12};
             static HPy_ssize_t _strides[1] = {1};
 
-            HPyDef_SLOT(FakeArray_getbuffer, _getbuffer_impl, HPy_bf_getbuffer)
+            HPyDef_SLOT_IMPL(FakeArray_getbuffer, _getbuffer_impl, HPy_bf_getbuffer)
             static int _getbuffer_impl(HPyContext *ctx, HPy self, HPy_buffer* buf, int flags) {
                 FakeArrayObject *arr = FakeArrayObject_AsStruct(ctx, self);
                 if (arr->exports > 0) {
                     buf->obj = HPy_NULL;
                     HPyErr_SetString(ctx, ctx->h_BufferError,
                                "only one buffer allowed");
                     return -1;
@@ -383,30 +383,30 @@
                 buf->strides = _strides;
                 buf->suboffsets = NULL;
                 buf->internal = NULL;
                 buf->obj = HPy_Dup(ctx, self);
                 return 0;
             }
 
-            HPyDef_SLOT(FakeArray_releasebuffer, _relbuffer_impl, HPy_bf_releasebuffer)
+            HPyDef_SLOT_IMPL(FakeArray_releasebuffer, _relbuffer_impl, HPy_bf_releasebuffer)
             static void _relbuffer_impl(HPyContext *ctx, HPy h_obj, HPy_buffer* buf) {
                 FakeArrayObject *arr = FakeArrayObject_AsStruct(ctx, h_obj);
                 arr->exports--;
             }
 
             static HPyDef *FakeArray_defines[] = {
                 &FakeArray_getbuffer,
                 &FakeArray_releasebuffer,
                 NULL
             };
 
             static HPyType_Spec FakeArray_Spec = {
                 .name = "mytest.FakeArray",
                 .basicsize = sizeof(FakeArrayObject),
-                .legacy = FakeArrayObject_IS_LEGACY,
+                .builtin_shape = SHAPE(FakeArrayObject),
                 .defines = FakeArray_defines,
             };
 
             @EXPORT_TYPE("FakeArray", FakeArray_Spec)
             @INIT
         """)
         arr = mod.FakeArray()
@@ -419,35 +419,101 @@
                 assert sys.getrefcount(arr) == init_refcount + 1
             for i in range(12):
                 assert mv[i] == i
         if self.supports_refcounts():
             assert sys.getrefcount(arr) == init_refcount
         mv2 = memoryview(arr)  # doesn't raise
 
+    def test_tp_repr_and_tp_str(self):
+        mod = self.make_module("""
+            #include <stdio.h>
+
+            #define BUF_SIZE 128
+
+            @DEFINE_PointObject
+            @DEFINE_Point_new
+
+            static HPy
+            point_str_repr(HPyContext *ctx, HPy h, int str)
+            {
+                char buf[BUF_SIZE];
+                PointObject *p = PointObject_AsStruct(ctx, h);
+                snprintf(buf, BUF_SIZE, "%s(Point(%ld, %ld))",
+                            (str ? "str" : "repr"), p->x, p->y);
+                return HPyUnicode_FromString(ctx, buf);
+            }
+
+            HPyDef_SLOT(Point_repr, HPy_tp_repr)
+            static HPy Point_repr_impl(HPyContext *ctx, HPy self)
+            {
+                return point_str_repr(ctx, self, 0);
+            }
+
+            HPyDef_SLOT(Point_str, HPy_tp_str)
+            static HPy Point_str_impl(HPyContext *ctx, HPy self)
+            {
+                return point_str_repr(ctx, self, 1);
+            }
+
+            @EXPORT_POINT_TYPE(&Point_new, &Point_str, &Point_repr)
+            @INIT
+        """)
+        p = mod.Point(1, 2)
+        assert str(p) == 'str(Point(1, 2))'
+        assert repr(p) == 'repr(Point(1, 2))'
+
+    def test_tp_hash(self):
+        mod = self.make_module("""
+            @DEFINE_PointObject
+            @DEFINE_Point_new
+
+            HPyDef_SLOT(Point_hash, HPy_tp_hash)
+            static HPy_ssize_t Point_hash_impl(HPyContext *ctx, HPy self)
+            {
+                PointObject *p = PointObject_AsStruct(ctx, self);
+                if (p->x < 0) {
+                    HPyErr_SetString(ctx, ctx->h_ValueError, "cannot hash Point object with negative x");
+                    return -1;
+                }
+                return p->x + p->y;
+            }
+
+            @EXPORT_POINT_TYPE(&Point_new, &Point_hash)
+            @INIT
+        """)
+        p = mod.Point(1, 10)
+        assert p.__hash__() == 11
+        assert hash(p) == 11
+        # We expect that the slot wrapper accepts hash code -1 without
+        # complaining. This is not the case for built-in function 'hash'.
+        assert mod.Point(0, -1).__hash__() == -1
+        with pytest.raises(ValueError):
+            hash(mod.Point(-1, 10))
+
 
 class TestSqSlots(HPyTest):
 
     ExtensionTemplate = PointTemplate
 
     def test_mp_subscript_and_mp_length(self):
         mod = self.make_module("""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(Point_getitem, Point_getitem_impl, HPy_mp_subscript);
+            HPyDef_SLOT(Point_getitem, HPy_mp_subscript);
             static HPy Point_getitem_impl(HPyContext *ctx, HPy self, HPy key)
             {
                 HPy prefix = HPyUnicode_FromString(ctx, "key was: ");
                 HPy key_repr = HPy_Repr(ctx, key);
                 HPy res = HPy_Add(ctx, prefix, key_repr);
                 HPy_Close(ctx, key_repr);
                 HPy_Close(ctx, prefix);
                 return res;
             }
 
-            HPyDef_SLOT(Point_length, Point_length_impl, HPy_mp_length);
+            HPyDef_SLOT(Point_length, HPy_mp_length);
             static HPy_ssize_t Point_length_impl(HPyContext *ctx, HPy self)
             {
                 return 1234;
             }
 
             @EXPORT_POINT_TYPE(&Point_getitem, &Point_length)
             @INIT
@@ -464,21 +530,21 @@
     def test_mp_ass_subscript(self):
         import pytest
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
             @DEFINE_Point_xy
 
-            HPyDef_SLOT(Point_len, Point_len_impl, HPy_mp_length);
+            HPyDef_SLOT(Point_len, HPy_mp_length);
             static HPy_ssize_t Point_len_impl(HPyContext *ctx, HPy self)
             {
                 return 2;
             }
 
-            HPyDef_SLOT(Point_setitem, Point_setitem_impl, HPy_mp_ass_subscript);
+            HPyDef_SLOT(Point_setitem, HPy_mp_ass_subscript);
             static int Point_setitem_impl(HPyContext *ctx, HPy self, HPy key,
                                           HPy h_value)
             {
                 long value;
                 if (HPy_IsNull(h_value)) {
                     value = -123; // this is the del p[] case
                 } else {
@@ -521,21 +587,21 @@
         del p['y']
         assert p.y == -123
 
     def test_sq_item_and_sq_length(self):
         mod = self.make_module("""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(Point_getitem, Point_getitem_impl, HPy_sq_item);
+            HPyDef_SLOT(Point_getitem, HPy_sq_item);
             static HPy Point_getitem_impl(HPyContext *ctx, HPy self, HPy_ssize_t idx)
             {
                 return HPyLong_FromLong(ctx, (long)idx*2);
             }
 
-            HPyDef_SLOT(Point_length, Point_length_impl, HPy_sq_length);
+            HPyDef_SLOT(Point_length, HPy_sq_length);
             static HPy_ssize_t Point_length_impl(HPyContext *ctx, HPy self)
             {
                 return 1234;
             }
 
             @EXPORT_POINT_TYPE(&Point_getitem, &Point_length)
             @INIT
@@ -549,21 +615,21 @@
     def test_sq_ass_item(self):
         import pytest
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
             @DEFINE_Point_xy
 
-            HPyDef_SLOT(Point_len, Point_len_impl, HPy_sq_length);
+            HPyDef_SLOT(Point_len, HPy_sq_length);
             static HPy_ssize_t Point_len_impl(HPyContext *ctx, HPy self)
             {
                 return 2;
             }
 
-            HPyDef_SLOT(Point_setitem, Point_setitem_impl, HPy_sq_ass_item);
+            HPyDef_SLOT(Point_setitem, HPy_sq_ass_item);
             static int Point_setitem_impl(HPyContext *ctx, HPy self, HPy_ssize_t idx,
                                           HPy h_value)
             {
                 long value;
                 if (HPy_IsNull(h_value))
                     value = -123; // this is the del p[] case
                 else {
@@ -609,25 +675,24 @@
         del p[-1]
         assert p.y == -123
 
     def test_sq_concat_and_sq_inplace_concat(self):
         mod = self.make_module("""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(Point_concat, Point_concat_impl, HPy_sq_concat);
+            HPyDef_SLOT(Point_concat, HPy_sq_concat);
             static HPy Point_concat_impl(HPyContext *ctx, HPy self, HPy other)
             {
                 HPy s = HPyUnicode_FromString(ctx, "sq_concat");
                 HPy res = HPyTuple_Pack(ctx, 3, self, s, other);
                 HPy_Close(ctx, s);
                 return res;
             }
 
-            HPyDef_SLOT(Point_inplace_concat, Point_inplace_concat_impl,
-                        HPy_sq_inplace_concat);
+            HPyDef_SLOT(Point_inplace_concat, HPy_sq_inplace_concat);
             static HPy Point_inplace_concat_impl(HPyContext *ctx, HPy self, HPy other)
             {
                 HPy s = HPyUnicode_FromString(ctx, "sq_inplace_concat");
                 HPy res = HPyTuple_Pack(ctx, 3, self, s, other);
                 HPy_Close(ctx, s);
                 return res;
             }
@@ -643,27 +708,26 @@
         tmp += 43
         assert tmp == (p, "sq_inplace_concat", 43)
 
     def test_sq_repeat_and_sq_inplace_repeat(self):
         mod = self.make_module("""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(Point_repeat, Point_repeat_impl, HPy_sq_repeat);
+            HPyDef_SLOT(Point_repeat, HPy_sq_repeat);
             static HPy Point_repeat_impl(HPyContext *ctx, HPy self, HPy_ssize_t t)
             {
                 HPy s = HPyUnicode_FromString(ctx, "sq_repeat");
                 HPy other = HPyLong_FromLong(ctx, (long) t);
                 HPy res = HPyTuple_Pack(ctx, 3, self, s, other);
                 HPy_Close(ctx, other);
                 HPy_Close(ctx, s);
                 return res;
             }
 
-            HPyDef_SLOT(Point_inplace_repeat, Point_inplace_repeat_impl,
-                        HPy_sq_inplace_repeat);
+            HPyDef_SLOT(Point_inplace_repeat, HPy_sq_inplace_repeat);
             static HPy Point_inplace_repeat_impl(HPyContext *ctx, HPy self, HPy_ssize_t t)
             {
                 HPy s = HPyUnicode_FromString(ctx, "sq_inplace_repeat");
                 HPy other = HPyLong_FromLong(ctx, (long) t);
                 HPy res = HPyTuple_Pack(ctx, 3, self, s, other);
                 HPy_Close(ctx, other);
                 HPy_Close(ctx, s);
@@ -682,15 +746,15 @@
         assert tmp == (p, "sq_inplace_repeat", 43)
 
     def test_sq_contains(self):
         import pytest
         mod = self.make_module("""
             @DEFINE_PointObject
 
-            HPyDef_SLOT(Point_contains, Point_contains_impl, HPy_sq_contains);
+            HPyDef_SLOT(Point_contains, HPy_sq_contains);
             static int Point_contains_impl(HPyContext *ctx, HPy self, HPy other)
             {
                 long val = HPyLong_AsLong(ctx, other);
                 if (HPyErr_Occurred(ctx))
                     return -1;
                 if (val == 42)
                     return 1;
@@ -708,15 +772,15 @@
 
     def test_tp_richcompare(self):
         import pytest
         mod = self.make_module("""
             @DEFINE_PointObject
             @DEFINE_Point_new
 
-            HPyDef_SLOT(Point_cmp, Point_cmp_impl, HPy_tp_richcompare);
+            HPyDef_SLOT(Point_cmp, HPy_tp_richcompare);
             static HPy Point_cmp_impl(HPyContext *ctx, HPy self, HPy o, HPy_RichCmpOp op)
             {
                 // XXX we should check the type of o
                 PointObject *p1 = PointObject_AsStruct(ctx, self);
                 PointObject *p2 = PointObject_AsStruct(ctx, o);
                 HPy_RETURN_RICHCOMPARE(ctx, p1->x, p2->x, op);
             }
```

### Comparing `hpy-0.0.4/test/test_tracker.py` & `hpy-0.9.0rc1/test/test_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 """
 from .support import HPyTest
 
 
 class TestHPyTracker(HPyTest):
     def hpytracker_module(self, ops, size=0):
         return self.make_module("""
-            HPyDef_METH(f, "f", f_impl, HPyFunc_VARARGS)
+            HPyDef_METH(f, "f", HPyFunc_VARARGS)
             static HPy f_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {{
                 HPyTracker ht;
                 HPy result = HPy_NULL;
                 ht = HPyTracker_New(ctx, {size});
                 if HPy_IsNull(ht) {{
                     return HPy_NULL;
                 }}
@@ -58,17 +58,17 @@
             HPyTracker_ForgetAll(ctx, ht);
         """)
         assert mod.f() is None
 
     def test_squares_example(self):
         import pytest
         mod = self.make_module("""
-            HPyDef_METH(squares, "squares", squares_impl, HPyFunc_VARARGS)
+            HPyDef_METH(squares, "squares", HPyFunc_VARARGS)
             static HPy squares_impl(HPyContext *ctx, HPy self,
-                              HPy *args, HPy_ssize_t nargs)
+                              const HPy *args, size_t nargs)
             {
                 long i, n;
                 long n_err = -1; // simulate an error at the given index
                 int result;
                 HPy key, value;
                 HPyTracker ht;
```

