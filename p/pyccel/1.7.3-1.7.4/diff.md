# Comparing `tmp/pyccel-1.7.3.tar.gz` & `tmp/pyccel-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyccel-1.7.3.tar", last modified: Tue Mar  7 17:50:24 2023, max compression
+gzip compressed data, was "pyccel-1.7.4.tar", last modified: Tue May  2 21:46:47 2023, max compression
```

## Comparing `pyccel-1.7.3.tar` & `pyccel-1.7.4.tar`

### file list

```diff
@@ -1,727 +1,726 @@
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.329573 pyccel-1.7.3/
--rw-r--r--   0 yaman      (501) staff       (20)      432 2023-03-07 17:48:54.000000 pyccel-1.7.3/AUTHORS
--rw-r--r--   0 yaman      (501) staff       (20)        5 2023-03-07 17:48:54.000000 pyccel-1.7.3/CHANGES
--rw-r--r--   0 yaman      (501) staff       (20)     1081 2023-03-07 17:48:54.000000 pyccel-1.7.3/LICENSE
--rw-r--r--   0 yaman      (501) staff       (20)      293 2023-03-07 17:48:54.000000 pyccel-1.7.3/MANIFEST.in
--rw-r--r--   0 yaman      (501) staff       (20)    13225 2023-03-07 17:50:24.329803 pyccel-1.7.3/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)    12901 2023-03-07 17:48:54.000000 pyccel-1.7.3/README.md
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.969295 pyccel-1.7.3/pyccel/
--rw-r--r--   0 yaman      (501) staff       (20)       33 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.983374 pyccel-1.7.3/pyccel/ast/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    15604 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    13168 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/bind_c.py
--rw-r--r--   0 yaman      (501) staff       (20)     7686 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/bitwise_operators.py
--rw-r--r--   0 yaman      (501) staff       (20)     3400 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/builtin_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)    29378 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     6502 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/c_concepts.py
--rw-r--r--   0 yaman      (501) staff       (20)     6460 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/class_defs.py
--rw-r--r--   0 yaman      (501) staff       (20)   121258 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/core.py
--rw-r--r--   0 yaman      (501) staff       (20)    18625 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/cwrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    10493 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/datatypes.py
--rw-r--r--   0 yaman      (501) staff       (20)     3715 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/functionalexpr.py
--rw-r--r--   0 yaman      (501) staff       (20)    27426 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)     9428 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/internals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2062 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/itertoolsext.py
--rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/literals.py
--rw-r--r--   0 yaman      (501) staff       (20)     3564 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)    10805 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/mathext.py
--rw-r--r--   0 yaman      (501) staff       (20)    13295 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/numpy_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    62314 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7113 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)    35482 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/operators.py
--rw-r--r--   0 yaman      (501) staff       (20)      869 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/scipyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7346 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/sympy_helper.py
--rw-r--r--   0 yaman      (501) staff       (20)     1630 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/sysext.py
--rw-r--r--   0 yaman      (501) staff       (20)    30201 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/utilities.py
--rw-r--r--   0 yaman      (501) staff       (20)    28556 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/ast/variable.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.986430 pyccel-1.7.3/pyccel/codegen/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     6587 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.988287 pyccel-1.7.3/pyccel/codegen/compiling/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/compiling/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     7995 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/compiling/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    16711 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/compiling/compilers.py
--rw-r--r--   0 yaman      (501) staff       (20)    16095 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/pipeline.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.996482 pyccel-1.7.3/pyccel/codegen/printing/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    85195 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/ccode.py
--rw-r--r--   0 yaman      (501) staff       (20)     4722 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/codeprinter.py
--rw-r--r--   0 yaman      (501) staff       (20)    63005 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/cwrappercode.py
--rw-r--r--   0 yaman      (501) staff       (20)   120214 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/fcode.py
--rw-r--r--   0 yaman      (501) staff       (20)    20526 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/luacode.py
--rw-r--r--   0 yaman      (501) staff       (20)    38247 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/printing/pycode.py
--rw-r--r--   0 yaman      (501) staff       (20)     6027 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/python_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)     7452 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/codegen/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.999380 pyccel-1.7.3/pyccel/commands/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/commands/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    11032 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/commands/console.py
--rw-r--r--   0 yaman      (501) staff       (20)     3461 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/commands/pyccel_clean.py
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/commands/pyccel_init.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.000251 pyccel-1.7.3/pyccel/compilers/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/compilers/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     9746 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/compilers/default_compilers.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.002597 pyccel-1.7.3/pyccel/complexity/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/complexity/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/complexity/arithmetic.py
--rw-r--r--   0 yaman      (501) staff       (20)     1145 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/complexity/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)     7188 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/complexity/memory.py
--rw-r--r--   0 yaman      (501) staff       (20)     2358 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)    11778 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/epyccel.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.004114 pyccel-1.7.3/pyccel/errors/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/errors/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    11261 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/errors/errors.py
--rw-r--r--   0 yaman      (501) staff       (20)    11854 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/errors/messages.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.006061 pyccel-1.7.3/pyccel/naming/
--rw-r--r--   0 yaman      (501) staff       (20)      791 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/naming/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2980 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/naming/cnameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     3572 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/naming/fortrannameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     1429 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/naming/pythonnameclashchecker.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.009919 pyccel-1.7.3/pyccel/parser/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    16370 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     9547 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/extend_tree.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.012151 pyccel-1.7.3/pyccel/parser/grammar/
--rw-r--r--   0 yaman      (501) staff       (20)     2221 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/grammar/headers.tx
--rw-r--r--   0 yaman      (501) staff       (20)      391 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/grammar/himi.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6361 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/grammar/openacc.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7307 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/grammar/openmp.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6539 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/grammar/pyccel.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7460 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/parser.py
--rw-r--r--   0 yaman      (501) staff       (20)    19696 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/scope.py
--rw-r--r--   0 yaman      (501) staff       (20)   159855 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/semantic.py
--rw-r--r--   0 yaman      (501) staff       (20)    38568 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntactic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.014749 pyccel-1.7.3/pyccel/parser/syntax/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    19189 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)     4144 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/himi.py
--rw-r--r--   0 yaman      (501) staff       (20)    36464 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)    27508 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/syntax/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     4079 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/parser/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.015084 pyccel-1.7.3/pyccel/stdlib/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.016121 pyccel-1.7.3/pyccel/stdlib/cwrapper/
--rw-r--r--   0 yaman      (501) staff       (20)     4529 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/cwrapper/cwrapper.c
--rw-r--r--   0 yaman      (501) staff       (20)     6528 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/cwrapper/cwrapper.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.017472 pyccel-1.7.3/pyccel/stdlib/cwrapper_ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    12578 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     1845 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.020237 pyccel-1.7.3/pyccel/stdlib/external/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/external/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1749 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/external/dfftpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1112 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/external/fitpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/external/lapack.py
--rw-r--r--   0 yaman      (501) staff       (20)     9467 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/external/mpi4py.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.030727 pyccel-1.7.3/pyccel/stdlib/internal/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    35216 2023-03-07 17:50:20.000000 pyccel-1.7.3/pyccel/stdlib/internal/blas.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     7825 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/blas.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     5940 2023-03-07 17:50:20.000000 pyccel-1.7.3/pyccel/stdlib/internal/dfftpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/dfftpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2841 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/fftw.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2867 2023-03-07 17:50:20.000000 pyccel-1.7.3/pyccel/stdlib/internal/fitpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)      343 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/fitpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    18250 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/hdf5.pyh
--rw-r--r--   0 yaman      (501) staff       (20)   354641 2023-03-07 17:50:21.000000 pyccel-1.7.3/pyccel/stdlib/internal/lapack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)    58149 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/lapack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    25250 2023-03-07 17:50:21.000000 pyccel-1.7.3/pyccel/stdlib/internal/mpi.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     5911 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/mpi.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/mpiext.py
--rw-r--r--   0 yaman      (501) staff       (20)    11017 2023-03-07 17:50:21.000000 pyccel-1.7.3/pyccel/stdlib/internal/openacc.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2675 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/openacc.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     8715 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)    10053 2023-03-07 17:50:21.000000 pyccel-1.7.3/pyccel/stdlib/internal/openmp.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2645 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/internal/openmp.pyh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.032161 pyccel-1.7.3/pyccel/stdlib/math/
--rw-r--r--   0 yaman      (501) staff       (20)     1766 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/math/pyc_math_c.c
--rw-r--r--   0 yaman      (501) staff       (20)     1331 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/math/pyc_math_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     3479 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/math/pyc_math_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.033549 pyccel-1.7.3/pyccel/stdlib/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    11346 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/ndarrays/ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     7152 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/ndarrays/ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.035661 pyccel-1.7.3/pyccel/stdlib/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)      755 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/numpy/numpy_c.c
--rw-r--r--   0 yaman      (501) staff       (20)      650 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/numpy/numpy_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     4629 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/numpy/numpy_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.036720 pyccel-1.7.3/pyccel/stdlib/parallel/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/parallel/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     7487 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/stdlib/parallel/mpi.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.037813 pyccel-1.7.3/pyccel/symbolic/
--rw-r--r--   0 yaman      (501) staff       (20)       48 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/symbolic/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     4472 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/symbolic/lambdify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.039835 pyccel-1.7.3/pyccel/utilities/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/utilities/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1203 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/utilities/metaclasses.py
--rw-r--r--   0 yaman      (501) staff       (20)     1227 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/utilities/stage.py
--rw-r--r--   0 yaman      (501) staff       (20)     1796 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/utilities/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyccel/version.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.972375 pyccel-1.7.3/pyccel.egg-info/
--rw-r--r--   0 yaman      (501) staff       (20)    13225 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)    24641 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/SOURCES.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/dependency_links.txt
--rw-r--r--   0 yaman      (501) staff       (20)      185 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/entry_points.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-03-07 17:50:21.000000 pyccel-1.7.3/pyccel.egg-info/not-zip-safe
--rw-r--r--   0 yaman      (501) staff       (20)      178 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/requires.txt
--rw-r--r--   0 yaman      (501) staff       (20)        7 2023-03-07 17:50:23.000000 pyccel-1.7.3/pyccel.egg-info/top_level.txt
--rw-r--r--   0 yaman      (501) staff       (20)      225 2023-03-07 17:48:54.000000 pyccel-1.7.3/pyproject.toml
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.041444 pyccel-1.7.3/samples/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/samples/README.rst
--rw-r--r--   0 yaman      (501) staff       (20)      385 2023-03-07 17:48:54.000000 pyccel-1.7.3/samples/mxm.py
--rw-r--r--   0 yaman      (501) staff       (20)      564 2023-03-07 17:48:54.000000 pyccel-1.7.3/samples/mxm_openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)      950 2023-03-07 17:50:24.330653 pyccel-1.7.3/setup.cfg
--rw-r--r--   0 yaman      (501) staff       (20)      628 2023-03-07 17:48:54.000000 pyccel-1.7.3/setup.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.043467 pyccel-1.7.3/tests/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.044240 pyccel-1.7.3/tests/ast/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.045628 pyccel-1.7.3/tests/ast/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      274 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ast/scripts/cyclic_dependence.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ast/scripts/math.py
--rw-r--r--   0 yaman      (501) staff       (20)     5177 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ast/test_basic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.946026 pyccel-1.7.3/tests/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.046318 pyccel-1.7.3/tests/codegen/ccode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.052481 pyccel-1.7.3/tests/codegen/ccode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_create.py
--rw-r--r--   0 yaman      (501) staff       (20)      755 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_indexing.py
--rw-r--r--   0 yaman      (501) staff       (20)      617 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1321 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_slicing.py
--rw-r--r--   0 yaman      (501) staff       (20)      894 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      926 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)     1301 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      379 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1735 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/ccode/test_ccode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.053094 pyccel-1.7.3/tests/codegen/fcode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.073760 pyccel-1.7.3/tests/codegen/fcode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1281 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/CommentBlock.py
--rw-r--r--   0 yaman      (501) staff       (20)      852 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      402 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/ListComprehension.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      230 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      102 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      622 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      710 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/classes_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      711 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/classes_3.py
--rw-r--r--   0 yaman      (501) staff       (20)     1364 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/classes_4.py
--rw-r--r--   0 yaman      (501) staff       (20)      296 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/complex_numbers.py
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/concatenation.py
--rw-r--r--   0 yaman      (501) staff       (20)     1136 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/context.py
--rw-r--r--   0 yaman      (501) staff       (20)     1248 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)      295 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      164 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/decorators_pure.py
--rw-r--r--   0 yaman      (501) staff       (20)     1104 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/decorators_types.py
--rw-r--r--   0 yaman      (501) staff       (20)      233 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1258 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      575 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/functions_inout.py
--rw-r--r--   0 yaman      (501) staff       (20)      456 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      426 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      981 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      258 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      461 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/issue_177.py
--rw-r--r--   0 yaman      (501) staff       (20)      191 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      839 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     2003 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)      803 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/matrix_assembly.py
--rw-r--r--   0 yaman      (501) staff       (20)      682 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/matrix_mul.py
--rw-r--r--   0 yaman      (501) staff       (20)      258 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/multiple_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)     1232 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)      783 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/precision.py
--rw-r--r--   0 yaman      (501) staff       (20)      762 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/recursive_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      237 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/returns.py
--rw-r--r--   0 yaman      (501) staff       (20)      360 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      382 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1712 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/fcode/test_fcode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.074304 pyccel-1.7.3/tests/codegen/pycode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.074828 pyccel-1.7.3/tests/codegen/pycode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1428 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/pycode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1352 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/codegen/pycode/test_pycode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.075441 pyccel-1.7.3/tests/complexity/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.075904 pyccel-1.7.3/tests/complexity/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/complexity/scripts/ex.py
--rw-r--r--   0 yaman      (501) staff       (20)     1054 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/complexity/test_complexity.py
--rw-r--r--   0 yaman      (501) staff       (20)     2254 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/conftest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.109795 pyccel-1.7.3/tests/epyccel/
--rw-r--r--   0 yaman      (501) staff       (20)      241 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      238 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/README.rst
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.130332 pyccel-1.7.3/tests/epyccel/modules/
--rw-r--r--   0 yaman      (501) staff       (20)      241 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      316 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      248 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      339 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_4.py
--rw-r--r--   0 yaman      (501) staff       (20)     1364 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      699 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_6.py
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_7.py
--rw-r--r--   0 yaman      (501) staff       (20)      235 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/Module_8.py
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      728 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/array_consts.py
--rw-r--r--   0 yaman      (501) staff       (20)    47943 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     2417 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)      235 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/awkward_names.py
--rw-r--r--   0 yaman      (501) staff       (20)     3566 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     1498 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)      846 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/call_user_defined_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)     2002 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      222 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/consts.py
--rw-r--r--   0 yaman      (501) staff       (20)     2285 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2093 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2228 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4059 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/generic_functions_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     4158 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/highorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4142 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1071 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)      531 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     2912 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)     5156 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)    14901 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1199 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1102 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)      682 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     9816 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      633 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/modules/types.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.134948 pyccel-1.7.3/tests/epyccel/recognised_functions/
--rw-r--r--   0 yaman      (501) staff       (20)     2757 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
--rw-r--r--   0 yaman      (501) staff       (20)    37670 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/recognised_functions/test_math_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)   247535 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/recognised_functions/test_numpy_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)    45813 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/recognised_functions/test_numpy_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     4693 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_array_as_func_args.py
--rw-r--r--   0 yaman      (501) staff       (20)    95680 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     9426 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_arrays_multiple_assignments.py
--rw-r--r--   0 yaman      (501) staff       (20)     6171 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_base.py
--rw-r--r--   0 yaman      (501) staff       (20)     5121 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)     9649 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     2538 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_class_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1477 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_compare_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      834 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_default_precision_template.py
--rw-r--r--   0 yaman      (501) staff       (20)     1192 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_docstrings.py
--rw-r--r--   0 yaman      (501) staff       (20)     7705 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_IfTernaryOperator.py
--rw-r--r--   0 yaman      (501) staff       (20)     7922 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)     3818 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     3137 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2378 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     8415 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_division.py
--rw-r--r--   0 yaman      (501) staff       (20)     9370 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4663 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_generators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2823 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)     4653 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_modules.py
--rw-r--r--   0 yaman      (501) staff       (20)     5520 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)    19623 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     5682 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_optional_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     6664 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_pow.py
--rw-r--r--   0 yaman      (501) staff       (20)     3266 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)    30657 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_return_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)    13389 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)     5824 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_transpose.py
--rw-r--r--   0 yaman      (501) staff       (20)     3472 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_epyccel_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     3307 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2150 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)    14121 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1923 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_higherorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1842 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)     2209 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_kind.py
--rw-r--r--   0 yaman      (501) staff       (20)     5448 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     4165 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)     2115 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     1041 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)     1736 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_parallel_epyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)     1259 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     7585 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_return.py
--rw-r--r--   0 yaman      (501) staff       (20)     1334 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     3201 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/test_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      705 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/epyccel/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.136098 pyccel-1.7.3/tests/errors/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.948106 pyccel-1.7.3/tests/errors/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.137608 pyccel-1.7.3/tests/errors/codegen/fortran/
--rw-r--r--   0 yaman      (501) staff       (20)      109 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      132 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/codegen/fortran/randint.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.142480 pyccel-1.7.3/tests/errors/known_bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      237 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/cross.py
--rw-r--r--   0 yaman      (501) staff       (20)      144 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/dicts.py
--rw-r--r--   0 yaman      (501) staff       (20)      471 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      630 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      580 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/header_interface.py
--rw-r--r--   0 yaman      (501) staff       (20)      904 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/inheritance.py
--rw-r--r--   0 yaman      (501) staff       (20)      181 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/known_bugs/lambdas.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.948989 pyccel-1.7.3/tests/errors/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.161205 pyccel-1.7.3/tests/errors/semantic/blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      129 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
--rw-r--r--   0 yaman      (501) staff       (20)      209 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      175 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/COMPLEX_TYPE.py
--rw-r--r--   0 yaman      (501) staff       (20)      160 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      194 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      133 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      272 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      115 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
--rw-r--r--   0 yaman      (501) staff       (20)      146 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
--rw-r--r--   0 yaman      (501) staff       (20)      316 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
--rw-r--r--   0 yaman      (501) staff       (20)       95 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      125 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      437 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      183 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/OPENMP_loop_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      103 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      132 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/OPENMP_simd_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      264 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      242 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
--rw-r--r--   0 yaman      (501) staff       (20)      494 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      111 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       93 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
--rw-r--r--   0 yaman      (501) staff       (20)       90 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
--rw-r--r--   0 yaman      (501) staff       (20)      109 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      187 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)       96 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)       98 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)       89 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)       93 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/ex5.py
--rw-r--r--   0 yaman      (501) staff       (20)      101 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/str_join.py
--rw-r--r--   0 yaman      (501) staff       (20)      107 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/blocking/str_join2.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.173140 pyccel-1.7.3/tests/errors/semantic/non_blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      137 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      151 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      153 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      119 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
--rw-r--r--   0 yaman      (501) staff       (20)       88 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      148 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      164 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      149 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      141 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      221 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)      119 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)       98 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      202 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      144 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/is.py
--rw-r--r--   0 yaman      (501) staff       (20)      196 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/semantic/non_blocking/var_is_none.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.174672 pyccel-1.7.3/tests/errors/syntax_blockers/
--rw-r--r--   0 yaman      (501) staff       (20)      287 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_blockers/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      388 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_blockers/imports.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.181965 pyccel-1.7.3/tests/errors/syntax_errors/
--rw-r--r--   0 yaman      (501) staff       (20)      372 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
--rw-r--r--   0 yaman      (501) staff       (20)      383 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/dict_str_keys.py
--rw-r--r--   0 yaman      (501) staff       (20)      207 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/functions_in_template.py
--rw-r--r--   0 yaman      (501) staff       (20)      158 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/functions_in_uniontype.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/import_star.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/list_comprehension_no_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)       96 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/nargs.py
--rw-r--r--   0 yaman      (501) staff       (20)      126 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/not_implemented.py
--rw-r--r--   0 yaman      (501) staff       (20)      115 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/raise.py
--rw-r--r--   0 yaman      (501) staff       (20)      126 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/try.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/types_arg.py
--rw-r--r--   0 yaman      (501) staff       (20)      138 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/types_arg_type.py
--rw-r--r--   0 yaman      (501) staff       (20)      100 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/syntax_errors/yield.py
--rw-r--r--   0 yaman      (501) staff       (20)     4384 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/errors/test_errors.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.182369 pyccel-1.7.3/tests/external/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.950501 pyccel-1.7.3/tests/external/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.183167 pyccel-1.7.3/tests/external/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2401 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.193331 pyccel-1.7.3/tests/external/scripts/mpi4py/
--rw-r--r--   0 yaman      (501) staff       (20)      335 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      685 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.194441 pyccel-1.7.3/tests/external/scripts/mpi4py/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      944 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/bugs/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      663 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/bugs/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      551 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      469 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      766 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      721 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      436 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      525 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      637 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      403 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1560 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      275 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      368 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1560 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      340 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      365 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      241 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/scripts/mpi4py/who_am_i.py
--rw-r--r--   0 yaman      (501) staff       (20)     1363 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/external/test_external.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.195011 pyccel-1.7.3/tests/internal/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.952568 pyccel-1.7.3/tests/internal/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.197587 pyccel-1.7.3/tests/internal/scripts/blas/
--rw-r--r--   0 yaman      (501) staff       (20)      560 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/blas/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      891 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/blas/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)      585 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/blas/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      921 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/blas/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      762 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/blas/ex5.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.198170 pyccel-1.7.3/tests/internal/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.206936 pyccel-1.7.3/tests/internal/scripts/mpi/
--rw-r--r--   0 yaman      (501) staff       (20)     1402 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/allgather.py
--rw-r--r--   0 yaman      (501) staff       (20)     1206 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1392 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/alltoall.py
--rw-r--r--   0 yaman      (501) staff       (20)     1130 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)     2058 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/column.py
--rw-r--r--   0 yaman      (501) staff       (20)     1478 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     2090 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/line.py
--rw-r--r--   0 yaman      (501) staff       (20)     1772 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/nonblocking.py
--rw-r--r--   0 yaman      (501) staff       (20)     1267 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/point_to_point_1.py
--rw-r--r--   0 yaman      (501) staff       (20)     3049 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1238 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1432 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/scatter.py
--rw-r--r--   0 yaman      (501) staff       (20)     1373 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)     1322 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/sendrecv_replace.py
--rw-r--r--   0 yaman      (501) staff       (20)     1741 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/split.py
--rw-r--r--   0 yaman      (501) staff       (20)      773 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/mpi/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.208506 pyccel-1.7.3/tests/internal/scripts/openacc/
--rw-r--r--   0 yaman      (501) staff       (20)      449 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/openacc/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      620 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/openacc/sum.py
--rw-r--r--   0 yaman      (501) staff       (20)      582 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/openacc/sum_kernels.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.209411 pyccel-1.7.3/tests/internal/scripts/openmp/
--rw-r--r--   0 yaman      (501) staff       (20)      607 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/openmp/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      413 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/scripts/openmp/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)     3508 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/internal/test_internal.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.209852 pyccel-1.7.3/tests/macro/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:23.954434 pyccel-1.7.3/tests/macro/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.219688 pyccel-1.7.3/tests/macro/scripts/MPI/
--rw-r--r--   0 yaman      (501) staff       (20)      448 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      865 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.221186 pyccel-1.7.3/tests/macro/scripts/MPI/bug/
--rw-r--r--   0 yaman      (501) staff       (20)     1587 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/bug/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      663 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/bug/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      789 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     7905 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/mpi4py.py
--rw-r--r--   0 yaman      (501) staff       (20)      549 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      899 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      832 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      552 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      568 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      750 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      603 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1943 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      380 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      568 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1953 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      472 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      479 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      404 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/MPI/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.224765 pyccel-1.7.3/tests/macro/scripts/blas/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.225232 pyccel-1.7.3/tests/macro/scripts/blas/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      364 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/bugs/dnrm2.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_daxpy.py
--rw-r--r--   0 yaman      (501) staff       (20)      467 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dcopy.py
--rw-r--r--   0 yaman      (501) staff       (20)     1148 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dgemm.py
--rw-r--r--   0 yaman      (501) staff       (20)     1186 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dgemv.py
--rw-r--r--   0 yaman      (501) staff       (20)      756 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dger.py
--rw-r--r--   0 yaman      (501) staff       (20)      482 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dscal.py
--rw-r--r--   0 yaman      (501) staff       (20)      636 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/blas/runtest_dswap.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.225792 pyccel-1.7.3/tests/macro/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)      670 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/scripts/lapack/runtest_dgbtrf.py
--rw-r--r--   0 yaman      (501) staff       (20)     3215 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/macro/test_macro.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.227299 pyccel-1.7.3/tests/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)     4725 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ndarrays/conftest.py
--rw-r--r--   0 yaman      (501) staff       (20)     1715 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ndarrays/leaks_check.py
--rw-r--r--   0 yaman      (501) staff       (20)    26585 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/ndarrays/test_ndarrays.c
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.229961 pyccel-1.7.3/tests/parser/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.230315 pyccel-1.7.3/tests/parser/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1075 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/scripts/comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     3491 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/test_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     1469 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/test_headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      305 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/test_himi.py
--rw-r--r--   0 yaman      (501) staff       (20)      359 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/test_openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)      280 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/parser/test_openmp.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.230833 pyccel-1.7.3/tests/preprocess/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.231239 pyccel-1.7.3/tests/preprocess/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      944 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/preprocess/scripts/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1018 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/preprocess/test_preprocess.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.232013 pyccel-1.7.3/tests/pyccel/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.233028 pyccel-1.7.3/tests/pyccel/project_abs_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.233662 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.234449 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      306 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.235950 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      228 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      307 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      215 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_abs_imports/runtest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.238682 pyccel-1.7.3/tests/pyccel/project_multi_imports/
--rw-r--r--   0 yaman      (501) staff       (20)      117 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_multi_imports/file1.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_multi_imports/file2.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_multi_imports/file3.py
--rw-r--r--   0 yaman      (501) staff       (20)      180 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_multi_imports/file4.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.240014 pyccel-1.7.3/tests/pyccel/project_rel_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.240717 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.241388 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      306 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.242783 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      222 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      286 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      215 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/project_rel_imports/runtest.py
--rw-r--r--   0 yaman      (501) staff       (20)      200 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/run_import_function.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.263385 pyccel-1.7.3/tests/pyccel/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2970 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/array_binary_operation.py
--rw-r--r--   0 yaman      (501) staff       (20)     4132 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/arrays_view.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.265485 pyccel-1.7.3/tests/pyccel/scripts/asserts/
--rw-r--r--   0 yaman      (501) staff       (20)      118 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/asserts/unvalid_assert1.py
--rw-r--r--   0 yaman      (501) staff       (20)      139 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/asserts/unvalid_assert2.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/asserts/unvalid_assert3.py
--rw-r--r--   0 yaman      (501) staff       (20)      218 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/asserts/valid_assert.py
--rw-r--r--   0 yaman      (501) staff       (20)       68 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/basic_header.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1411 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/bool_comp.py
--rw-r--r--   0 yaman      (501) staff       (20)     2133 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/c_arrays.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.267347 pyccel-1.7.3/tests/pyccel/scripts/classes/
--rw-r--r--   0 yaman      (501) staff       (20)      735 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/classes/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      600 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/classes/classes_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      500 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/classes/classes_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      373 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      822 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      916 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/default_args_mod.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.271967 pyccel-1.7.3/tests/pyccel/scripts/exits/
--rw-r--r--   0 yaman      (501) staff       (20)      127 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/empty_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)      151 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/negative_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/negative_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/positive_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/positive_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      185 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/positive_exit3.py
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/exits/zero_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)     2237 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/expressions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.273279 pyccel-1.7.3/tests/pyccel/scripts/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      301 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder1/folder1_funcs.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.276306 pyccel-1.7.3/tests/pyccel/scripts/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      301 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder2/folder2_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      199 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder2/runtest_imports2.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/folder2/runtest_rel_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      301 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)     3618 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/generic_functions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.280227 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/
--rw-r--r--   0 yaman      (501) staff       (20)      286 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      592 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      815 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      304 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
--rw-r--r--   0 yaman      (501) staff       (20)     1189 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      808 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      281 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.283354 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/
--rw-r--r--   0 yaman      (501) staff       (20)      310 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      584 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      827 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)     1227 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      825 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      307 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.296998 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/
--rw-r--r--   0 yaman      (501) staff       (20)      183 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/collisions2.py
--rw-r--r--   0 yaman      (501) staff       (20)      202 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/collisions3.py
--rw-r--r--   0 yaman      (501) staff       (20)      219 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/collisions4.py
--rw-r--r--   0 yaman      (501) staff       (20)      188 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/collisions5.py
--rw-r--r--   0 yaman      (501) staff       (20)      923 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import.py
--rw-r--r--   0 yaman      (501) staff       (20)      994 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1003 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      292 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      944 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      291 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      296 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      935 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      926 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1020 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      285 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      289 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      191 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/user_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      175 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/import_syntax/user_mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      883 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/lapack_subroutine.py
--rw-r--r--   0 yaman      (501) staff       (20)      176 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      117 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/module_init2.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.298170 pyccel-1.7.3/tests/pyccel/scripts/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)     1591 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/numpy/numpy_kernels.py
--rw-r--r--   0 yaman      (501) staff       (20)     2813 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/numpy/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)      813 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/print_integers.py
--rw-r--r--   0 yaman      (501) staff       (20)      886 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/print_sp_and_end.py
--rw-r--r--   0 yaman      (501) staff       (20)     2057 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/print_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)      382 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/print_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      643 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/return_numpy_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      419 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      737 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)      674 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_degree_in.py
--rw-r--r--   0 yaman      (501) staff       (20)      167 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_folder_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      351 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      325 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_function_alias.py
--rw-r--r--   0 yaman      (501) staff       (20)      660 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      151 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      428 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_inoutfunc.py
--rw-r--r--   0 yaman      (501) staff       (20)      168 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      306 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_module_init2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1511 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)      413 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/scripts/runtest_type_print.py
--rw-r--r--   0 yaman      (501) staff       (20)    41856 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/pyccel/test_pyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)      844 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/run_tests.bat
--rwxr-xr-x   0 yaman      (501) staff       (20)      899 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/run_tests_py3.sh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.298832 pyccel-1.7.3/tests/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.306464 pyccel-1.7.3/tests/semantic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      136 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      482 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      826 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1172 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      129 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      198 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      112 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      308 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      164 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      312 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1031 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/semantic/test_semantic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.307086 pyccel-1.7.3/tests/symbolic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.308946 pyccel-1.7.3/tests/symbolic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      959 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/symbolic/scripts/decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      284 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/symbolic/scripts/lambdas.py
--rw-r--r--   0 yaman      (501) staff       (20)      712 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/symbolic/scripts/neural_net.py
--rw-r--r--   0 yaman      (501) staff       (20)     1264 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/symbolic/test_symbolic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.309503 pyccel-1.7.3/tests/syntax/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.319482 pyccel-1.7.3/tests/syntax/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      852 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      158 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/annotated_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)       87 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/asserts.py
--rw-r--r--   0 yaman      (501) staff       (20)       78 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/breaks.py
--rw-r--r--   0 yaman      (501) staff       (20)      111 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/class_member_index.py
--rw-r--r--   0 yaman      (501) staff       (20)      345 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)       87 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/dels.py
--rw-r--r--   0 yaman      (501) staff       (20)      191 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/dots.py
--rw-r--r--   0 yaman      (501) staff       (20)      965 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      194 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      289 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      111 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)       81 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/prints.py
--rw-r--r--   0 yaman      (501) staff       (20)      197 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/slice.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)       93 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      312 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1060 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/syntax/test_syntax.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.319920 pyccel-1.7.3/tests/warnings/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.322615 pyccel-1.7.3/tests/warnings/semantic/
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      146 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      294 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      134 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/UNDEFINED_DECORATOR.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/semantic/UNDEFINED_DECORATORS.py
--rw-r--r--   0 yaman      (501) staff       (20)     3008 2023-03-07 17:48:54.000000 pyccel-1.7.3/tests/warnings/test_warnings.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-03-07 17:50:24.329016 pyccel-1.7.3/tutorial/
--rw-r--r--   0 yaman      (501) staff       (20)     1667 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/builtin-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)     2642 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/compiler.md
--rw-r--r--   0 yaman      (501) staff       (20)     1779 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/const_keyword.md
--rw-r--r--   0 yaman      (501) staff       (20)    15373 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/decorators.md
--rw-r--r--   0 yaman      (501) staff       (20)    10633 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/function-pointers-as-arguments.md
--rw-r--r--   0 yaman      (501) staff       (20)     3173 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/header-files.md
--rw-r--r--   0 yaman      (501) staff       (20)     8825 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/ndarrays.md
--rw-r--r--   0 yaman      (501) staff       (20)    16159 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/numpy-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)    18475 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/openmp.md
--rw-r--r--   0 yaman      (501) staff       (20)    17344 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/quickstart.md
--rw-r--r--   0 yaman      (501) staff       (20)     2505 2023-03-07 17:48:54.000000 pyccel-1.7.3/tutorial/templates.md
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.194131 pyccel-1.7.4/
+-rw-r--r--   0 yaman      (501) staff       (20)      451 2023-05-02 21:45:18.000000 pyccel-1.7.4/AUTHORS
+-rw-r--r--   0 yaman      (501) staff       (20)     1081 2023-05-02 21:45:18.000000 pyccel-1.7.4/LICENSE
+-rw-r--r--   0 yaman      (501) staff       (20)      293 2023-05-02 21:45:18.000000 pyccel-1.7.4/MANIFEST.in
+-rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-05-02 21:46:47.194320 pyccel-1.7.4/PKG-INFO
+-rw-r--r--   0 yaman      (501) staff       (20)    13180 2023-05-02 21:45:18.000000 pyccel-1.7.4/README.md
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.813501 pyccel-1.7.4/pyccel/
+-rw-r--r--   0 yaman      (501) staff       (20)       33 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.831474 pyccel-1.7.4/pyccel/ast/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    15604 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    13461 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/bind_c.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7686 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/bitwise_operators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3400 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/builtin_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)    29378 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/builtins.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6502 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/c_concepts.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6460 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/class_defs.py
+-rw-r--r--   0 yaman      (501) staff       (20)   126977 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/core.py
+-rw-r--r--   0 yaman      (501) staff       (20)    20054 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/cwrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10493 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/datatypes.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3715 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/functionalexpr.py
+-rw-r--r--   0 yaman      (501) staff       (20)    29329 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9428 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/internals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2062 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/itertoolsext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/literals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3564 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/macros.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10805 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/mathext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    14034 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/numpy_wrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)    62314 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/numpyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7113 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/omp.py
+-rw-r--r--   0 yaman      (501) staff       (20)    35482 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/operators.py
+-rw-r--r--   0 yaman      (501) staff       (20)      869 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/scipyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7346 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/sympy_helper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1630 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/sysext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    30831 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/utilities.py
+-rw-r--r--   0 yaman      (501) staff       (20)    28982 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/variable.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.834125 pyccel-1.7.4/pyccel/codegen/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6587 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.835598 pyccel-1.7.4/pyccel/codegen/compiling/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9200 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16711 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/compilers.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16095 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/pipeline.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.843133 pyccel-1.7.4/pyccel/codegen/printing/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    85613 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/ccode.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4722 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/codeprinter.py
+-rw-r--r--   0 yaman      (501) staff       (20)    63675 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/cwrappercode.py
+-rw-r--r--   0 yaman      (501) staff       (20)   121391 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/fcode.py
+-rw-r--r--   0 yaman      (501) staff       (20)    20480 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/luacode.py
+-rw-r--r--   0 yaman      (501) staff       (20)    38538 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/pycode.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5941 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/python_wrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7452 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.846050 pyccel-1.7.4/pyccel/commands/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11032 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/console.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3461 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/pyccel_clean.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/pyccel_init.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.847418 pyccel-1.7.4/pyccel/compilers/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/compilers/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10742 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/compilers/default_compilers.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.849477 pyccel-1.7.4/pyccel/complexity/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/arithmetic.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1145 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7188 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/memory.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2358 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11778 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/epyccel.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.850786 pyccel-1.7.4/pyccel/errors/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11261 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/errors.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11854 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/messages.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.852404 pyccel-1.7.4/pyccel/naming/
+-rw-r--r--   0 yaman      (501) staff       (20)      791 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2980 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/cnameclashchecker.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3572 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/fortrannameclashchecker.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1429 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/pythonnameclashchecker.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.855745 pyccel-1.7.4/pyccel/parser/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16370 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9547 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/extend_tree.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.860050 pyccel-1.7.4/pyccel/parser/grammar/
+-rw-r--r--   0 yaman      (501) staff       (20)     2221 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/headers.tx
+-rw-r--r--   0 yaman      (501) staff       (20)      391 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/himi.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     6361 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/openacc.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     7307 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/openmp.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     6539 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/pyccel.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     7460 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/parser.py
+-rw-r--r--   0 yaman      (501) staff       (20)    19696 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/scope.py
+-rw-r--r--   0 yaman      (501) staff       (20)   161830 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/semantic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    39088 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntactic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.864222 pyccel-1.7.4/pyccel/parser/syntax/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    19189 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/himi.py
+-rw-r--r--   0 yaman      (501) staff       (20)    36464 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/openacc.py
+-rw-r--r--   0 yaman      (501) staff       (20)    27508 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4079 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.864714 pyccel-1.7.4/pyccel/stdlib/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.865543 pyccel-1.7.4/pyccel/stdlib/cwrapper/
+-rw-r--r--   0 yaman      (501) staff       (20)     4529 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.c
+-rw-r--r--   0 yaman      (501) staff       (20)     6528 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.866905 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)    12578 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
+-rw-r--r--   0 yaman      (501) staff       (20)     1845 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.869194 pyccel-1.7.4/pyccel/stdlib/external/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1749 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/dfftpack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1112 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/fitpack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/lapack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9467 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/mpi4py.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.880124 pyccel-1.7.4/pyccel/stdlib/internal/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    35216 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/blas.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     7825 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/blas.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     5940 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     2841 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/fftw.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     2867 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)      343 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)    18250 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/hdf5.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)   354641 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)    58149 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)    25250 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     5911 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpiext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11017 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     2675 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     8715 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10053 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     2645 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyh
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.882061 pyccel-1.7.4/pyccel/stdlib/math/
+-rw-r--r--   0 yaman      (501) staff       (20)     1766 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.c
+-rw-r--r--   0 yaman      (501) staff       (20)     1331 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.h
+-rw-r--r--   0 yaman      (501) staff       (20)     3479 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_f90.f90
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.883523 pyccel-1.7.4/pyccel/stdlib/ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)    11346 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.c
+-rw-r--r--   0 yaman      (501) staff       (20)     7152 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.885589 pyccel-1.7.4/pyccel/stdlib/numpy/
+-rw-r--r--   0 yaman      (501) staff       (20)      755 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.c
+-rw-r--r--   0 yaman      (501) staff       (20)      650 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.h
+-rw-r--r--   0 yaman      (501) staff       (20)     4629 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_f90.f90
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.886537 pyccel-1.7.4/pyccel/stdlib/parallel/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/parallel/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7487 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/parallel/mpi.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.887520 pyccel-1.7.4/pyccel/symbolic/
+-rw-r--r--   0 yaman      (501) staff       (20)       48 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/symbolic/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4472 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/symbolic/lambdify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.889491 pyccel-1.7.4/pyccel/utilities/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1203 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/metaclasses.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1227 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/stage.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1796 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/version.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.816588 pyccel-1.7.4/pyccel.egg-info/
+-rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/PKG-INFO
+-rw-r--r--   0 yaman      (501) staff       (20)    24626 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/SOURCES.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        1 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/dependency_links.txt
+-rw-r--r--   0 yaman      (501) staff       (20)      185 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/entry_points.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        1 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel.egg-info/not-zip-safe
+-rw-r--r--   0 yaman      (501) staff       (20)      178 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/requires.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        7 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/top_level.txt
+-rw-r--r--   0 yaman      (501) staff       (20)      225 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyproject.toml
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.891082 pyccel-1.7.4/samples/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/README.rst
+-rw-r--r--   0 yaman      (501) staff       (20)      385 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/mxm.py
+-rw-r--r--   0 yaman      (501) staff       (20)      564 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/mxm_openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)      950 2023-05-02 21:46:47.195119 pyccel-1.7.4/setup.cfg
+-rw-r--r--   0 yaman      (501) staff       (20)      628 2023-05-02 21:45:18.000000 pyccel-1.7.4/setup.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.893571 pyccel-1.7.4/tests/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.894232 pyccel-1.7.4/tests/ast/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.895557 pyccel-1.7.4/tests/ast/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      257 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/scripts/cyclic_dependence.py
+-rw-r--r--   0 yaman      (501) staff       (20)      173 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/scripts/math.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5098 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/test_basic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.792333 pyccel-1.7.4/tests/codegen/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.896295 pyccel-1.7.4/tests/codegen/ccode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.901543 pyccel-1.7.4/tests/codegen/ccode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1558 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_create.py
+-rw-r--r--   0 yaman      (501) staff       (20)      754 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_indexing.py
+-rw-r--r--   0 yaman      (501) staff       (20)      616 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1320 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_slicing.py
+-rw-r--r--   0 yaman      (501) staff       (20)      876 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      925 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)      378 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1734 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/test_ccode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.902104 pyccel-1.7.4/tests/codegen/fcode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.923259 pyccel-1.7.4/tests/codegen/fcode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1280 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/CommentBlock.py
+-rw-r--r--   0 yaman      (501) staff       (20)      851 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/Functional_Stmts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/ListComprehension.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
+-rw-r--r--   0 yaman      (501) staff       (20)      229 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)      101 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      646 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      734 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      735 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1388 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      295 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/complex_numbers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      154 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/concatenation.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1160 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/context.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1272 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)      294 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_elemental.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_pure.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1103 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)      232 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      574 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/functions_inout.py
+-rw-r--r--   0 yaman      (501) staff       (20)      480 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/generic_methods.py
+-rw-r--r--   0 yaman      (501) staff       (20)      425 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      980 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      264 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      485 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/issue_177.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      838 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2002 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/macros.py
+-rw-r--r--   0 yaman      (501) staff       (20)      802 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_assembly.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_mul.py
+-rw-r--r--   0 yaman      (501) staff       (20)      257 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/multiple_assign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1231 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/numpyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)      782 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/precision.py
+-rw-r--r--   0 yaman      (501) staff       (20)      761 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/recursive_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/returns.py
+-rw-r--r--   0 yaman      (501) staff       (20)      359 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      381 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1711 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/test_fcode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.923902 pyccel-1.7.4/tests/codegen/pycode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.924482 pyccel-1.7.4/tests/codegen/pycode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1427 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/pycode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1351 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/pycode/test_pycode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.925108 pyccel-1.7.4/tests/complexity/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.925845 pyccel-1.7.4/tests/complexity/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/complexity/scripts/ex.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1053 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/complexity/test_complexity.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2253 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/conftest.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.957871 pyccel-1.7.4/tests/epyccel/
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/Module_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      238 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/README.rst
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.980337 pyccel-1.7.4/tests/epyccel/modules/
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      315 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      247 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      338 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_4.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1363 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      698 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_7.py
+-rw-r--r--   0 yaman      (501) staff       (20)      234 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_8.py
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      728 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/array_consts.py
+-rw-r--r--   0 yaman      (501) staff       (20)    47942 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2416 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/augassign.py
+-rw-r--r--   0 yaman      (501) staff       (20)      234 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/awkward_names.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3565 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1497 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/bitwise.py
+-rw-r--r--   0 yaman      (501) staff       (20)      845 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/call_user_defined_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2001 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/complex_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      222 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/consts.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2284 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/external_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2092 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/functionals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2227 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4058 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/generic_functions_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/highorder_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4462 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1070 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/mpi_collective.py
+-rw-r--r--   0 yaman      (501) staff       (20)      530 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/mpi_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2911 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/multi_rank.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/numpy_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)    14866 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1198 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1101 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/python_annotations.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9815 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      632 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/types.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.986185 pyccel-1.7.4/tests/epyccel/recognised_functions/
+-rw-r--r--   0 yaman      (501) staff       (20)     2756 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
+-rw-r--r--   0 yaman      (501) staff       (20)    37669 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_math_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)   247535 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)    45813 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4693 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_array_as_func_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)    95679 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9425 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_arrays_multiple_assignments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6170 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5120 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_bitwise.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9648 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_builtins.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2537 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_class_expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1476 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_compare_expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      834 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_default_precision_template.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1191 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_docstrings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7704 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_IfTernaryOperator.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7921 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_augassign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3817 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_complex_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3136 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2377 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_default_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)     8351 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_division.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9369 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_generators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2822 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4652 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_modules.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5519 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_multi_rank.py
+-rw-r--r--   0 yaman      (501) staff       (20)    19588 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_optional_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6663 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_pow.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3265 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_python_annotations.py
+-rw-r--r--   0 yaman      (501) staff       (20)    30656 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_return_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)    13388 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5823 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_transpose.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3471 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_external_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2149 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_functionals.py
+-rw-r--r--   0 yaman      (501) staff       (20)    14120 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1922 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_higherorder_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1841 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2208 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_kind.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5783 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4164 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_mpi_collective.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_mpi_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1040 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_multiple_results.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1735 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_parallel_epyccel.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1258 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7595 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_return.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1333 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3200 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      704 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.987366 pyccel-1.7.4/tests/errors/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.795123 pyccel-1.7.4/tests/errors/codegen/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.989006 pyccel-1.7.4/tests/errors/codegen/fortran/
+-rw-r--r--   0 yaman      (501) staff       (20)      108 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
+-rw-r--r--   0 yaman      (501) staff       (20)      131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/codegen/fortran/randint.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.995793 pyccel-1.7.4/tests/errors/known_bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/cross.py
+-rw-r--r--   0 yaman      (501) staff       (20)      143 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/dicts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      495 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      796 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      654 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/generic_methods.py
+-rw-r--r--   0 yaman      (501) staff       (20)      579 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/header_interface.py
+-rw-r--r--   0 yaman      (501) staff       (20)      928 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/inheritance.py
+-rw-r--r--   0 yaman      (501) staff       (20)      180 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/lambdas.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.795987 pyccel-1.7.4/tests/errors/semantic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.017946 pyccel-1.7.4/tests/errors/semantic/blocking/
+-rw-r--r--   0 yaman      (501) staff       (20)      128 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
+-rw-r--r--   0 yaman      (501) staff       (20)      208 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      174 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/COMPLEX_TYPE.py
+-rw-r--r--   0 yaman      (501) staff       (20)      159 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      193 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      132 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      296 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      315 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
+-rw-r--r--   0 yaman      (501) staff       (20)       94 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INHOMOG_LIST.py
+-rw-r--r--   0 yaman      (501) staff       (20)      124 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
+-rw-r--r--   0 yaman      (501) staff       (20)      436 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      182 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      129 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_loop_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      102 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_simd_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      263 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
+-rw-r--r--   0 yaman      (501) staff       (20)      241 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
+-rw-r--r--   0 yaman      (501) staff       (20)      493 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
+-rw-r--r--   0 yaman      (501) staff       (20)       89 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
+-rw-r--r--   0 yaman      (501) staff       (20)      108 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
+-rw-r--r--   0 yaman      (501) staff       (20)      186 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)       95 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)       97 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)       88 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      100 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/str_join.py
+-rw-r--r--   0 yaman      (501) staff       (20)      106 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/str_join2.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.033268 pyccel-1.7.4/tests/errors/semantic/non_blocking/
+-rw-r--r--   0 yaman      (501) staff       (20)      136 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      152 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      118 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)       87 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
+-rw-r--r--   0 yaman      (501) staff       (20)      149 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
+-rw-r--r--   0 yaman      (501) staff       (20)      147 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
+-rw-r--r--   0 yaman      (501) staff       (20)      148 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
+-rw-r--r--   0 yaman      (501) staff       (20)      140 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
+-rw-r--r--   0 yaman      (501) staff       (20)      156 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
+-rw-r--r--   0 yaman      (501) staff       (20)      220 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      118 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
+-rw-r--r--   0 yaman      (501) staff       (20)       97 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      201 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      143 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/is.py
+-rw-r--r--   0 yaman      (501) staff       (20)      195 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/var_is_none.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.034559 pyccel-1.7.4/tests/errors/syntax_blockers/
+-rw-r--r--   0 yaman      (501) staff       (20)      286 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_blockers/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_blockers/imports.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.043753 pyccel-1.7.4/tests/errors/syntax_errors/
+-rw-r--r--   0 yaman      (501) staff       (20)      371 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
+-rw-r--r--   0 yaman      (501) staff       (20)      382 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)       91 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/dict_str_keys.py
+-rw-r--r--   0 yaman      (501) staff       (20)      206 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/functions_in_template.py
+-rw-r--r--   0 yaman      (501) staff       (20)      157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/functions_in_uniontype.py
+-rw-r--r--   0 yaman      (501) staff       (20)      109 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/import_star.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/list_comprehension_no_assign.py
+-rw-r--r--   0 yaman      (501) staff       (20)       95 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/nargs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      125 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/not_implemented.py
+-rw-r--r--   0 yaman      (501) staff       (20)      114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/raise.py
+-rw-r--r--   0 yaman      (501) staff       (20)      125 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/try.py
+-rw-r--r--   0 yaman      (501) staff       (20)      156 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/types_arg.py
+-rw-r--r--   0 yaman      (501) staff       (20)      137 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/types_arg_type.py
+-rw-r--r--   0 yaman      (501) staff       (20)       99 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/yield.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4383 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/test_errors.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.044398 pyccel-1.7.4/tests/external/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.797285 pyccel-1.7.4/tests/external/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.045065 pyccel-1.7.4/tests/external/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)     2401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/lapack/ex1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.056787 pyccel-1.7.4/tests/external/scripts/mpi4py/
+-rw-r--r--   0 yaman      (501) staff       (20)      334 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      684 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bcast.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.058230 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex8.py
+-rw-r--r--   0 yaman      (501) staff       (20)      550 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      468 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      765 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)      720 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      435 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      524 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      636 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      402 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      274 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      367 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      339 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      364 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/who_am_i.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1362 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/test_external.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.058935 pyccel-1.7.4/tests/internal/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.799163 pyccel-1.7.4/tests/internal/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.062314 pyccel-1.7.4/tests/internal/scripts/blas/
+-rw-r--r--   0 yaman      (501) staff       (20)      559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      890 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      584 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      920 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      761 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex5.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.062955 pyccel-1.7.4/tests/internal/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)     2779 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/lapack/ex1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.072661 pyccel-1.7.4/tests/internal/scripts/mpi/
+-rw-r--r--   0 yaman      (501) staff       (20)     1401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/allgather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1205 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1391 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/alltoall.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1129 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2057 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/column.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1477 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2089 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/line.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/nonblocking.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3048 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1237 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1431 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/scatter.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1372 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1321 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv_replace.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1740 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/split.py
+-rw-r--r--   0 yaman      (501) staff       (20)      772 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/who_am_i.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.075069 pyccel-1.7.4/tests/internal/scripts/openacc/
+-rw-r--r--   0 yaman      (501) staff       (20)      448 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      619 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/sum.py
+-rw-r--r--   0 yaman      (501) staff       (20)      581 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/sum_kernels.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.076953 pyccel-1.7.4/tests/internal/scripts/openmp/
+-rw-r--r--   0 yaman      (501) staff       (20)      606 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openmp/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openmp/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3507 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/test_internal.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.077625 pyccel-1.7.4/tests/macro/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.800614 pyccel-1.7.4/tests/macro/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.089085 pyccel-1.7.4/tests/macro/scripts/MPI/
+-rw-r--r--   0 yaman      (501) staff       (20)      447 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      864 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bcast.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.090471 pyccel-1.7.4/tests/macro/scripts/MPI/bug/
+-rw-r--r--   0 yaman      (501) staff       (20)     1586 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex8.py
+-rw-r--r--   0 yaman      (501) staff       (20)      788 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7929 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/mpi4py.py
+-rw-r--r--   0 yaman      (501) staff       (20)      548 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      898 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)      831 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      551 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      567 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      749 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      602 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1942 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      379 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      567 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1952 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      471 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      478 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      403 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/who_am_i.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.094922 pyccel-1.7.4/tests/macro/scripts/blas/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.095544 pyccel-1.7.4/tests/macro/scripts/blas/bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      363 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/bugs/dnrm2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_daxpy.py
+-rw-r--r--   0 yaman      (501) staff       (20)      467 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dcopy.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1148 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemm.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1186 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      756 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dger.py
+-rw-r--r--   0 yaman      (501) staff       (20)      482 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dscal.py
+-rw-r--r--   0 yaman      (501) staff       (20)      636 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dswap.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.096229 pyccel-1.7.4/tests/macro/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)      670 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/lapack/runtest_dgbtrf.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/test_macro.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.098132 pyccel-1.7.4/tests/ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)     4723 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/conftest.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1714 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/leaks_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)    26585 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/test_ndarrays.c
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.101658 pyccel-1.7.4/tests/parser/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.102270 pyccel-1.7.4/tests/parser/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1074 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/scripts/comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3490 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1468 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      304 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_himi.py
+-rw-r--r--   0 yaman      (501) staff       (20)      358 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_openacc.py
+-rw-r--r--   0 yaman      (501) staff       (20)      279 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_openmp.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.102974 pyccel-1.7.4/tests/preprocess/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.103505 pyccel-1.7.4/tests/preprocess/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/preprocess/scripts/omp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1017 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/preprocess/test_preprocess.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.104860 pyccel-1.7.4/tests/pyccel/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.106066 pyccel-1.7.4/tests/pyccel/project_abs_imports/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.106666 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.108019 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/mod1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.109561 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      227 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/mod3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/runtest.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.112300 pyccel-1.7.4/tests/pyccel/project_multi_imports/
+-rw-r--r--   0 yaman      (501) staff       (20)      116 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      179 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file4.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.112985 pyccel-1.7.4/tests/pyccel/project_rel_imports/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.113684 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.114492 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/mod1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.116257 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      221 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      285 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/mod3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/runtest.py
+-rw-r--r--   0 yaman      (501) staff       (20)      199 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/run_import_function.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.137798 pyccel-1.7.4/tests/pyccel/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2969 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/array_binary_operation.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/arrays_view.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.140046 pyccel-1.7.4/tests/pyccel/scripts/asserts/
+-rw-r--r--   0 yaman      (501) staff       (20)      117 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      138 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      162 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      217 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/valid_assert.py
+-rw-r--r--   0 yaman      (501) staff       (20)       68 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/basic_header.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     1410 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/bool_comp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2132 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/c_arrays.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.141781 pyccel-1.7.4/tests/pyccel/scripts/classes/
+-rw-r--r--   0 yaman      (501) staff       (20)      726 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      590 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      490 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes_5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      372 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/decorators_elemental.py
+-rw-r--r--   0 yaman      (501) staff       (20)      821 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/decorators_inline.py
+-rw-r--r--   0 yaman      (501) staff       (20)      915 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/default_args_mod.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.145918 pyccel-1.7.4/tests/pyccel/scripts/exits/
+-rw-r--r--   0 yaman      (501) staff       (20)      126 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/empty_exit.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/negative_exit1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/negative_exit2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      127 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      184 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      127 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/zero_exit.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/expressions.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.146742 pyccel-1.7.4/tests/pyccel/scripts/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder1/folder1_funcs.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.148571 pyccel-1.7.4/tests/pyccel/scripts/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/folder2_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      198 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/runtest_imports2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      189 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/runtest_rel_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1154 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3617 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/generic_functions.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.152243 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/
+-rw-r--r--   0 yaman      (501) staff       (20)      285 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
+-rw-r--r--   0 yaman      (501) staff       (20)      591 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      814 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      265 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1188 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      807 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/quicksort.py
+-rw-r--r--   0 yaman      (501) staff       (20)      280 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/simplify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.155001 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/
+-rw-r--r--   0 yaman      (501) staff       (20)      309 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
+-rw-r--r--   0 yaman      (501) staff       (20)      583 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      826 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      824 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
+-rw-r--r--   0 yaman      (501) staff       (20)      306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.165774 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/
+-rw-r--r--   0 yaman      (501) staff       (20)      182 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      201 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      218 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      187 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      922 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import.py
+-rw-r--r--   0 yaman      (501) staff       (20)      993 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      287 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      291 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      290 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      295 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      934 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)      925 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1019 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      282 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      287 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1001 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      284 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      288 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/user_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)      174 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/user_mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      882 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/lapack_subroutine.py
+-rw-r--r--   0 yaman      (501) staff       (20)      175 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/module_init.py
+-rw-r--r--   0 yaman      (501) staff       (20)      116 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/module_init2.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.166780 pyccel-1.7.4/tests/pyccel/scripts/numpy/
+-rw-r--r--   0 yaman      (501) staff       (20)     1590 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_kernels.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2812 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)      812 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_integers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      885 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_sp_and_end.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2056 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)      381 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      617 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/return_numpy_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)      418 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_decorators_inline.py
+-rw-r--r--   0 yaman      (501) staff       (20)      736 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_default_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)      673 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_degree_in.py
+-rw-r--r--   0 yaman      (501) staff       (20)      166 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_folder_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      350 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      324 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_function_alias.py
+-rw-r--r--   0 yaman      (501) staff       (20)      659 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      427 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_inoutfunc.py
+-rw-r--r--   0 yaman      (501) staff       (20)      167 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_module_init.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_module_init2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1510 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_multiple_results.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_type_print.py
+-rw-r--r--   0 yaman      (501) staff       (20)    42226 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/test_pyccel.py
+-rw-r--r--   0 yaman      (501) staff       (20)      844 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/run_tests.bat
+-rwxr-xr-x   0 yaman      (501) staff       (20)      899 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/run_tests_py3.sh
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.167188 pyccel-1.7.4/tests/semantic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.172742 pyccel-1.7.4/tests/semantic/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      135 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      506 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      825 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1171 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      128 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      197 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      141 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      111 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)      307 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)      311 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/zeros.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1030 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/test_semantic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.173178 pyccel-1.7.4/tests/symbolic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.174865 pyccel-1.7.4/tests/symbolic/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      958 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/decorator.py
+-rw-r--r--   0 yaman      (501) staff       (20)      283 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/lambdas.py
+-rw-r--r--   0 yaman      (501) staff       (20)      711 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/neural_net.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1263 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/test_symbolic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.175404 pyccel-1.7.4/tests/syntax/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.184461 pyccel-1.7.4/tests/syntax/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      851 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/Functional_Stmts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/annotated_comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/asserts.py
+-rw-r--r--   0 yaman      (501) staff       (20)       77 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/breaks.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      796 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/class_member_index.py
+-rw-r--r--   0 yaman      (501) staff       (20)      369 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/dels.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/dots.py
+-rw-r--r--   0 yaman      (501) staff       (20)      964 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      193 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      288 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)       80 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/prints.py
+-rw-r--r--   0 yaman      (501) staff       (20)      196 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/slice.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)      311 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/zeros.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1059 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/test_syntax.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.184966 pyccel-1.7.4/tests/warnings/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.187968 pyccel-1.7.4/tests/warnings/semantic/
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      318 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      133 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/UNDEFINED_DECORATOR.py
+-rw-r--r--   0 yaman      (501) staff       (20)      141 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/UNDEFINED_DECORATORS.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3007 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/test_warnings.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.193718 pyccel-1.7.4/tutorial/
+-rw-r--r--   0 yaman      (501) staff       (20)     1667 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/builtin-functions.md
+-rw-r--r--   0 yaman      (501) staff       (20)     2642 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/compiler.md
+-rw-r--r--   0 yaman      (501) staff       (20)     1779 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/const_keyword.md
+-rw-r--r--   0 yaman      (501) staff       (20)    15373 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/decorators.md
+-rw-r--r--   0 yaman      (501) staff       (20)    10633 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/function-pointers-as-arguments.md
+-rw-r--r--   0 yaman      (501) staff       (20)     3173 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/header-files.md
+-rw-r--r--   0 yaman      (501) staff       (20)     8825 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/ndarrays.md
+-rw-r--r--   0 yaman      (501) staff       (20)    16159 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/numpy-functions.md
+-rw-r--r--   0 yaman      (501) staff       (20)    18475 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/openmp.md
+-rw-r--r--   0 yaman      (501) staff       (20)    17344 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/quickstart.md
+-rw-r--r--   0 yaman      (501) staff       (20)     2505 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/templates.md
```

### Comparing `pyccel-1.7.3/LICENSE` & `pyccel-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/PKG-INFO` & `pyccel-1.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.7.3
+Version: 1.7.4
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 # Welcome to Pyccel
 
- [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade)
+ [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -296,15 +296,15 @@
     ```
 
 -   **Development mode**:
 
     ```sh
     git clone git@github.com:pyccel/pyccel.git
     cd pyccel
-    pip3 install --user -e .[test]
+    pip3 install --user -e ".[test]"
     ```
 
 this will install a _python_ library **Pyccel** and a _binary_ called **`pyccel`**.
 Any required Python packages will be installed automatically from PyPI.
 
 ### On a read-only system
 
@@ -318,15 +318,15 @@
 A warning, reminding the user to execute this command, will be printed to the screen when pyccelising files which rely on these packages if the pickling step has not been executed.
 
 ## Additional packages
 
 In order to run the unit tests and to get a coverage report, a few additional Python packages should be installed:
 
 ```sh
-pip install --user -e .[test]
+pip install --user -e ".[test]"
 ```
 
 Most of the unit tests can also be run in parallel.
 
 ## Testing
 
 To test your Pyccel installation please run the script `tests/run\_tests\_py3.sh` (Unix), or `tests/run\_tests.bat` (Windows).
@@ -358,10 +358,13 @@
 Alternatively you may have docker or podman set the context using `-v $PWD:/data:rwz` instead of `-v $PWD:/data:rw` .
 
 ## Developer Documentation
 
 -   [Overview](./developer_docs/overview.md)
 -   [How to solve an issue](./developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](./developer_docs/review_process.md)
+-   [Development Conventions](./developer_docs/development_conventions.md)
 -   [Tips and Tricks](./developer_docs/tips_and_tricks.md)
+-   [Scope](./developer_docs/scope.md)
+-   [Array Ordering](./developer_docs/order_docs.md)
```

### Comparing `pyccel-1.7.3/README.md` & `pyccel-1.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Welcome to Pyccel
 
- [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade)
+ [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -281,15 +281,15 @@
     ```
 
 -   **Development mode**:
 
     ```sh
     git clone git@github.com:pyccel/pyccel.git
     cd pyccel
-    pip3 install --user -e .[test]
+    pip3 install --user -e ".[test]"
     ```
 
 this will install a _python_ library **Pyccel** and a _binary_ called **`pyccel`**.
 Any required Python packages will be installed automatically from PyPI.
 
 ### On a read-only system
 
@@ -303,15 +303,15 @@
 A warning, reminding the user to execute this command, will be printed to the screen when pyccelising files which rely on these packages if the pickling step has not been executed.
 
 ## Additional packages
 
 In order to run the unit tests and to get a coverage report, a few additional Python packages should be installed:
 
 ```sh
-pip install --user -e .[test]
+pip install --user -e ".[test]"
 ```
 
 Most of the unit tests can also be run in parallel.
 
 ## Testing
 
 To test your Pyccel installation please run the script `tests/run\_tests\_py3.sh` (Unix), or `tests/run\_tests.bat` (Windows).
@@ -343,8 +343,11 @@
 Alternatively you may have docker or podman set the context using `-v $PWD:/data:rwz` instead of `-v $PWD:/data:rw` .
 
 ## Developer Documentation
 
 -   [Overview](./developer_docs/overview.md)
 -   [How to solve an issue](./developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](./developer_docs/review_process.md)
+-   [Development Conventions](./developer_docs/development_conventions.md)
 -   [Tips and Tricks](./developer_docs/tips_and_tricks.md)
+-   [Scope](./developer_docs/scope.md)
+-   [Array Ordering](./developer_docs/order_docs.md)
```

### Comparing `pyccel-1.7.3/pyccel/ast/basic.py` & `pyccel-1.7.4/pyccel/ast/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/bind_c.py` & `pyccel-1.7.4/pyccel/ast/bind_c.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 from pyccel.ast.basic import Basic
 from pyccel.ast.core import CodeBlock, FunctionCall, Module
 from pyccel.ast.core import FunctionAddress
 from pyccel.ast.core import FunctionDef
+from pyccel.ast.core import FunctionDefArgument, FunctionDefResult
 from pyccel.ast.core import Assign
 from pyccel.ast.core import Import
 from pyccel.ast.core import AsName
 from pyccel.ast.core import Allocate
 from pyccel.ast.datatypes import DataType, NativeInteger
 from pyccel.ast.variable import Variable
 from pyccel.parser.scope import Scope
@@ -69,34 +70,41 @@
         else:
             raise NotImplementedError('TODO for {}'.format(type(a)))
 
     return _args
 
 #=======================================================================================
 def as_static_function(func, *, mod_scope, name=None):
-    """ Translate a FunctionDef to a BindCFunctionDef by altering the
-    arguments to allow the function to be called from c.
-    E.g. the size of each dimension of an array is provided
+    """
+    Translate a FunctionDef to a BindCFunctionDef.
+
+    Translate a FunctionDef to a BindCFunctionDef by altering the
+    arguments to allow the function to be called from C.
+    E.g. the size of each dimension of an array is provided.
 
     Parameters
-    ==========
-    func     : FunctionDef
-               The function to be translated
-    mod_scope: Scope
-               The scope of the module which contains func
-    name     : str
-               The new name of the function
+    ----------
+    func : FunctionDef
+        The function to be translated.
+    mod_scope : Scope
+        The scope of the module which contains the function.
+    name : str
+        The new name of the function.
+
+    Returns
+    -------
+    BindCFunctionDef
+        The function which can be called from C.
     """
 
     assert(isinstance(func, FunctionDef))
 
     args    = list(func.arguments)
-    results = list(func.results)
+    results = [r.var for r in func.results]
     body    = func.body.body
-    arguments_inout = func.arguments_inout
     functions = func.functions
     _results = []
     interfaces = func.interfaces
 
     scope = mod_scope.new_child_scope(func.name)
 
     # Convert array results to inout arguments
@@ -116,15 +124,14 @@
 
     if name is None:
         name = 'bind_c_{}'.format(func.name).lower()
 
     # ...
     results_names = [i.name for i in _results]
     _args = []
-    _arguments_inout = []
 
     for i_a, a in enumerate(args):
         a = a.var
         if not isinstance(a, (Variable, FunctionAddress)):
             raise TypeError('Expecting a Variable or FunctionAddress type for {}'.format(a))
         if not isinstance(a, FunctionAddress) and a.rank > 0:
             # ...
@@ -134,43 +141,35 @@
                 n_arg  = Variable('int', n_name)
 
                 additional_args += [n_arg]
 
             shape_new = tuple(additional_args)
             # ...
 
-            _args += additional_args
-            _arguments_inout += [False] * len(additional_args)
+            _args += [FunctionDefArgument(a) for a in additional_args]
 
             a_new = Variable( a.dtype, a.name,
                               memory_handling = a.memory_handling,
+                              is_argument = True,
                               is_optional = a.is_optional,
                               shape       = shape_new,
                               rank        = a.rank,
                               order       = a.order,
                               precision   = a.precision)
 
-            if not( a.name in results_names ):
-                _args += [a_new]
-
-            else:
-                _results += [a_new]
+            _args.append(FunctionDefArgument(a_new))
 
         else:
-            _args += [a]
+            _args.append(FunctionDefArgument(a))
 
-        intent = arguments_inout[i_a]
-        _arguments_inout += [intent]
     args = _args
-    results = _results
-    arguments_inout = _arguments_inout
+    results = [FunctionDefResult(r) for r in _results]
     # ...
-    return BindCFunctionDef( name, list(args), results, body,
+    return BindCFunctionDef( name, args, results, body,
                         is_static = True,
-                        arguments_inout = arguments_inout,
                         functions = functions,
                         interfaces = interfaces,
                         imports = func.imports,
                         original_function = func,
                         doc_string = func.doc_string,
                         scope = scope
                         )
@@ -198,30 +197,44 @@
         name = scope.get_new_name('bind_c_{}'.format(original_module.name.target))
     else:
         name = scope.get_new_name('bind_c_{}'.format(original_module.name))
     return Module(name, (), bind_c_funcs+bind_c_arrays, imports = imports, scope=scope)
 
 #=======================================================================================
 def as_static_function_call(func, mod, mod_scope, name=None, imports = None):
-    """ Translate a FunctionDef to a BindCFunctionDef which calls the
+    """
+    Create a BindCFunctionDef which calls the provided FunctionDef.
+
+    Translate a FunctionDef to a BindCFunctionDef which calls the
     original function. A BindCFunctionDef is a FunctionDef where the
     arguments are altered to allow the function to be called from c.
-    E.g. the size of each dimension of an array is provided
+    E.g. the size of each dimension of an array is provided.
 
     Parameters
-    ==========
-    func     : FunctionDef
-               The function to be translated
-    mod      : Module
-               The module which contains func
-    name     : str
-               The new name of the function
-    imports  : list
-               An optional parameter into which any required imports
-               can be collected
+    ----------
+    func : FunctionDef
+        The function to be translated.
+
+    mod : Module
+        The module which contains the function.
+
+    mod_scope : Scope
+        The scope describing the module.
+
+    name : str
+        The new name of the function.
+
+    imports : list
+        An optional parameter into which any required imports
+        can be collected.
+
+    Returns
+    -------
+    BindCFunctionDef
+        The function which can be called from C.
     """
 
     assert isinstance(func, FunctionDef)
     assert isinstance(mod, Module)
     mod_name = mod.scope.get_python_name(mod.name)
 
     # from module import func
@@ -231,22 +244,21 @@
         imports.append(Import(target=AsName(func, func.name), source=mod_name, mod=mod))
         local_imports = ()
 
     # function arguments
     args = sanitize_arguments(func.arguments)
     # function body
     call    = FunctionCall(func, args)
-    results = func.results
+    results = [r.var for r in func.results]
     results = results[0] if len(results) == 1 else results
     stmt    = call if len(func.results) == 0 else Assign(results, call)
     body    = [stmt]
 
     # new function declaration
     new_func = FunctionDef(func.name, func.arguments, func.results, body,
-                       arguments_inout = func.arguments_inout,
                        functions = func.functions,
                        interfaces = func.interfaces,
                        imports = local_imports,
                        doc_string = func.doc_string
                        )
 
     # make it compatible with c
@@ -330,37 +342,42 @@
         c_loc = CLocFunc(var, bind_var)
         body = [*assigns, c_loc]
     return body, variables
 
 #=======================================================================================
 
 def wrap_module_array_var(var, scope, mod):
-    """ Function returning the function necessary to expose an array
+    """
+    Get a function which allows a module variable to be accessed.
+
+    Create a function which exposes a module array variable to C.
+    This allows the module variable to be accessed from the Python
+    code.
 
     Parameters
     ----------
     var : Variable
-            The array to be exposed
+            The array to be exposed.
     scope : Scope
-            The current scope (used to find valid names for variables)
+            The current scope (used to find valid names for variables).
     mod : Module
-            The module where the variable is defined
+            The module where the variable is defined.
 
-    Results
+    Returns
     -------
-    func : FunctionDef
-            A function which wraps an array and can be called from C
+    FunctionDef
+        A function which wraps an array and can be called from C.
     """
     func_name = 'bind_c_'+var.name.lower()
     func_scope = scope.new_child_scope(func_name)
     body, necessary_vars = wrap_array(var, func_scope, True)
     func_scope.insert_variable(necessary_vars[0])
-    arg_vars = necessary_vars
+    result_vars = [FunctionDefResult(v) for v in necessary_vars]
     import_mod = Import(mod.name, AsName(var,var.name), mod=mod)
     func = BindCFunctionDef(name = func_name,
                   body      = body,
                   arguments = [],
-                  results   = arg_vars,
+                  results   = result_vars,
                   imports   = [import_mod],
                   scope = func_scope,
                   original_function = None)
     return func
```

### Comparing `pyccel-1.7.3/pyccel/ast/bitwise_operators.py` & `pyccel-1.7.4/pyccel/ast/bitwise_operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/builtin_imports.py` & `pyccel-1.7.4/pyccel/ast/builtin_imports.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/builtins.py` & `pyccel-1.7.4/pyccel/ast/builtins.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/c_concepts.py` & `pyccel-1.7.4/pyccel/ast/c_concepts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/class_defs.py` & `pyccel-1.7.4/pyccel/ast/class_defs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/core.py` & `pyccel-1.7.4/pyccel/ast/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     'ForIterator',
     'FuncAddressDeclare',
     'FunctionAddress',
     'FunctionCall',
     'FunctionCallArgument',
     'FunctionDef',
     'FunctionDefArgument',
+    'FunctionDefResult',
     'If',
     'IfSection',
     'Import',
     'InlineFunctionDef',
     'InProgram',
     'Interface',
     'Iterable',
@@ -1075,67 +1076,76 @@
     @property
     def declarations(self):
         return [Declare(i.dtype, i) for i in self.variables]
 
 
 
 class Module(ScopedNode):
+    """
+    Represents a module in the code.
 
-    """Represents a module in the code. A block consists of the following inputs
+    The Pyccel node representing a Python module. A module consists of everything
+    inside a given Python file.
 
     Parameters
     ----------
-    name: str
-        name of the module
+    name : str
+        Name of the module.
 
-    variables: list
-        list of the variables that appear in the block.
+    variables : list
+        List of the variables that appear in the block.
 
-    funcs: list
-        a list of FunctionDef instances
+    funcs : list
+        A list of FunctionDef instances.
 
-    init_func: FunctionDef
+    init_func : FunctionDef, default: None
         The function which initialises the module (expressions in the
-        python module which are executed on import)
-        Default : None
+        python module which are executed on import).
 
-    free_func: FunctionDef
-        The function which frees any variables allocated in the module
-        Default : None
+    free_func : FunctionDef, default: None
+        The function which frees any variables allocated in the module.
 
-    program: Program/CodeBlock
+    program : Program/CodeBlock
         CodeBlock containing any expressions which are only executed
-        when the module is executed directly
+        when the module is executed directly.
 
-    interfaces: list
-        a list of Interface instances
+    interfaces : list
+        A list of Interface instances.
 
-    classes: list
-        a list of ClassDef instances
+    classes : list
+        A list of ClassDef instances.
 
-    imports: list, tuple
-        list of needed imports
+    imports : list, tuple
+        List of needed imports.
+
+    scope : Scope
+        The scope of the module.
 
     Examples
     --------
-    >>> from pyccel.ast.core import Variable, Assign
+    >>> from pyccel.ast.variable import Variable
+    >>> from pyccel.ast.core import FunctionDefArgument, Assign, FunctionDefResult
     >>> from pyccel.ast.core import ClassDef, FunctionDef, Module
+    >>> from pyccel.ast.operators import PyccelAdd, PyccelMinus
+    >>> from pyccel.ast.literals import LiteralInteger
     >>> x = Variable('float', 'x')
     >>> y = Variable('float', 'y')
     >>> z = Variable('float', 'z')
     >>> t = Variable('float', 't')
     >>> a = Variable('float', 'a')
     >>> b = Variable('float', 'b')
-    >>> body = [Assign(y,x+a)]
-    >>> translate = FunctionDef('translate', [x,y,a,b], [z,t], body)
+    >>> body = [Assign(z,PyccelAdd(x,a))]
+    >>> args = [FunctionDefArgument(arg) for arg in [x,y,a,b]]
+    >>> results = [FunctionDefResult(res) for res in [z,t]]
+    >>> translate = FunctionDef('translate', args, results, body)
     >>> attributes   = [x,y]
     >>> methods     = [translate]
     >>> Point = ClassDef('Point', attributes, methods)
-    >>> incr = FunctionDef('incr', [x], [y], [Assign(y,x+1)])
-    >>> decr = FunctionDef('decr', [x], [y], [Assign(y,x-1)])
+    >>> incr = FunctionDef('incr', [FunctionDefArgument(x)], [FunctionDefResult(y)], [Assign(y,PyccelAdd(x,LiteralInteger(1)))])
+    >>> decr = FunctionDef('decr', [FunctionDefArgument(x)], [FunctionDefResult(y)], [Assign(y,PyccelMinus(x,LiteralInteger(1)))])
     >>> Module('my_module', [], [incr, decr], classes = [Point])
     Module(my_module, [], [FunctionDef(), FunctionDef()], [], [ClassDef(Point, (x, y), (FunctionDef(),), [public], (), [], [])], ())
     """
     __slots__ = ('_name','_variables','_funcs','_interfaces',
                  '_classes','_imports','_init_func','_free_func',
                  '_program','_variable_inits','_internal_dictionary')
     _attribute_nodes = ('_variables','_funcs','_interfaces',
@@ -1334,40 +1344,52 @@
 
     def keys(self):
         """ Returns the names of all objects accessible directly in this module
         """
         return self._internal_dictionary.keys()
 
 class ModuleHeader(Basic):
+    """
+    Represents the header file for a module.
 
-    """Represents the header file for a module
+    This class is simply a wrapper around a module. It is helpful to differentiate
+    between headers and sources when printing.
 
     Parameters
     ----------
-    module: Module
-        the module
+    module : Module
+        The module described by the header.
+
+    See Also
+    --------
+    Module : The module itself.
 
     Examples
     --------
-    >>> from pyccel.ast.core import Variable, Assign
+    >>> from pyccel.ast.variable import Variable
+    >>> from pyccel.ast.core import FunctionDefArgument, Assign, FunctionDefResult
     >>> from pyccel.ast.core import ClassDef, FunctionDef, Module
+    >>> from pyccel.ast.operators import PyccelAdd, PyccelMinus
+    >>> from pyccel.ast.literals import LiteralInteger
     >>> x = Variable('float', 'x')
     >>> y = Variable('float', 'y')
     >>> z = Variable('float', 'z')
     >>> t = Variable('float', 't')
     >>> a = Variable('float', 'a')
     >>> b = Variable('float', 'b')
-    >>> body = [Assign(y,x+a)]
-    >>> translate = FunctionDef('translate', [x,y,a,b], [z,t], body)
+    >>> body = [Assign(z,PyccelAdd(x,a))]
+    >>> args = [FunctionDefArgument(arg) for arg in [x,y,a,b]]
+    >>> results = [FunctionDefResult(res) for res in [z,t]]
+    >>> translate = FunctionDef('translate', args, results, body)
     >>> attributes   = [x,y]
     >>> methods     = [translate]
     >>> Point = ClassDef('Point', attributes, methods)
-    >>> incr = FunctionDef('incr', [x], [y], [Assign(y,x+1)])
-    >>> decr = FunctionDef('decr', [x], [y], [Assign(y,x-1)])
-    >>> mod = Module('my_module', [], [incr, decr], classes = [Point])
+    >>> incr = FunctionDef('incr', [FunctionDefArgument(x)], [FunctionDefResult(y)], [Assign(y,PyccelAdd(x,LiteralInteger(1)))])
+    >>> decr = FunctionDef('decr', [FunctionDefArgument(x)], [FunctionDefResult(y)], [Assign(y,PyccelMinus(x,LiteralInteger(1)))])
+    >>> Module('my_module', [], [incr, decr], classes = [Point])
     >>> ModuleHeader(mod)
     Module(my_module, [], [FunctionDef(), FunctionDef()], [], [ClassDef(Point, (x, y), (FunctionDef(),), [public], (), [], [])], ())
     """
     __slots__ = ('_module',)
     _attribute_nodes = ('_module',)
 
     def __init__(self, module):
@@ -1848,39 +1870,68 @@
     def __str__(self):
         if self.has_keyword:
             return '{} = {}'.format(self.keyword, str(self.value))
         else:
             return '{}'.format(str(self.value))
 
 class FunctionDefArgument(PyccelAstNode):
+    """
+    Node describing the argument of a function.
 
-    """A FunctionDef FunctionDefArgument
+    An object describing the argument of a function described
+    by a FunctionDef. This object stores all the information
+    which describes an argument but is superfluous for a Variable.
+
+    Parameters
+    ----------
+    name : PyccelSymbol, Variable, FunctionAddress
+        The name of the argument.
+
+    value : PyccelAstNode, default: None
+        The default value of the argument.
+
+    kwonly : bool
+        Indicates if the argument must be passed by keyword.
+
+    annotation : str
+        The type annotation describing the argument.
+
+    See Also
+    --------
+    FunctionDef : The class where these objects will be stored.
 
     Examples
     --------
     >>> from pyccel.ast.core import FunctionDefArgument
     >>> n = FunctionDefArgument('n')
     >>> n
     n
     """
-    __slots__ = ('_name','_var','_kwonly','_annotation','_value')
+    __slots__ = ('_name','_var','_kwonly','_annotation','_value','_inout')
     _attribute_nodes = ('_value','_var')
 
     def __init__(self, name, *, value = None, kwonly=False, annotation=None):
         if isinstance(name, (Variable, FunctionAddress)):
             self._var  = name
             self._name = name.name
         elif isinstance(name, PyccelSymbol):
             self._var  = name
             self._name = name
         else:
             raise TypeError("Name must be a PyccelSymbol, Variable or FunctionAddress")
         self._value      = value
         self._kwonly     = kwonly
         self._annotation = annotation
+
+        if isinstance(name, Variable):
+            name.declare_as_argument()
+
+        if pyccel_stage != "syntactic":
+            self._inout = self.var.rank>0 and not self.var.is_const if isinstance(self.var, Variable) else False
+
         super().__init__()
 
     @property
     def name(self):
         """ The name of the argument
         """
         return self._name
@@ -1922,14 +1973,33 @@
     @property
     def has_default(self):
         """ Indicates whether the argument has a default value
         (if not then it must be provided)
         """
         return self._value is not None
 
+    @property
+    def inout(self):
+        """
+        Indicates whether the argument may be modified by the function.
+
+        True if the argument may be modified in the function. False if
+        the argument remains constant in the function.
+        """
+        return self._inout
+
+    def make_const(self):
+        """
+        Indicate that the argument does not change in the function.
+
+        Indicate that the argument does not change in the function by
+        modifying the inout flag.
+        """
+        self._inout = False
+
     def __str__(self):
         if self.has_default:
             argument = str(self.name)
             value = str(self.value)
             return '{0}={1}'.format(argument, value)
         else:
             return str(self.name)
@@ -1938,17 +2008,112 @@
         if self.has_default:
             argument = str(self.name)
             value = str(self.value)
             return 'FunctionDefArgument({0}={1})'.format(argument, value)
         else:
             return 'FunctionDefArgument({})'.format(repr(self.name))
 
+class FunctionDefResult(PyccelAstNode):
+    """
+    Node describing the result of a function.
+
+    An object describing the result of a function described
+    by a FunctionDef. This object stores all the information
+    which describes an result but is superfluous for a Variable.
+
+    Parameters
+    ----------
+    var : Variable
+        The variable which represents the returned value.
+
+    annotation : str, default: None
+        The type annotation describing the argument.
+
+    See Also
+    --------
+    FunctionDef : The class where these objects will be stored.
+
+    Examples
+    --------
+    >>> from pyccel.ast.core import FunctionDefResult
+    >>> n = FunctionDefResult('n')
+    >>> n
+    n
+    """
+    __slots__ = ('_var','_is_argument','_annotation')
+    _attribute_nodes = ('_var',)
+
+    def __init__(self, var, *, annotation=None):
+        self._var        = var
+        self._annotation = annotation
+
+        if pyccel_stage == 'syntactic':
+            if not isinstance(var, PyccelSymbol):
+                raise TypeError("Var must be a PyccelSymbol")
+        elif not isinstance(var, Variable):
+            raise TypeError("Var must be a Variable")
+        else:
+            self._is_argument = var.is_argument
+
+        super().__init__()
+
+    @property
+    def var(self):
+        """
+        The variable representing the result.
+
+        The variable which represents the result. This variable is only
+        available after the semantic stage.
+        """
+        return self._var
+
+    @property
+    def annotation(self):
+        """
+        The result annotation providing dtype information.
+
+        The annotation which provides all information about the data
+        types, precision, etc, necessary to fully define the result.
+        """
+        return self._annotation
+
+    @property
+    def is_argument(self):
+        """
+        Indicates if the result was declared as an argument.
+
+        Indicates if the result of the function was initially declared
+        as an argument of the same function. If this is the case then
+        the result may be printed simply as an inout argument.
+        """
+        return self._is_argument
+
+    def __repr__(self):
+        return 'FunctionDefResult({})'.format(repr(self.var))
+
+    def __str__(self):
+        return str(self.var)
+
 class FunctionCall(PyccelAstNode):
+    """
+    Represents a function call in the code.
+
+    A node which holds all information necessary to represent a function
+    call in the code.
 
-    """Represents a function call in the code.
+    Parameters
+    ----------
+    func : FunctionDef
+        The function being called.
+
+    args : list of FunctionCallArgument
+        The arguments passed to the function.
+
+    current_function : FunctionDef, default: None
+        The function where the call takes place.
     """
     __slots__ = ('_arguments','_funcdef','_interface','_func_name','_interface_name',
                  '_dtype','_precision','_shape','_rank','_order')
     _attribute_nodes = ('_arguments','_funcdef','_interface')
 
     def __init__(self, func, args, current_function=None):
 
@@ -2014,19 +2179,19 @@
 
         if current_function == func.name:
             if len(func.results)>0 and not isinstance(func.results[0], PyccelAstNode):
                 errors.report(RECURSIVE_RESULTS_REQUIRED, symbol=func, severity="fatal")
 
         self._funcdef       = func
         self._arguments     = args
-        self._dtype         = func.results[0].dtype     if len(func.results) == 1 else NativeTuple()
-        self._rank          = func.results[0].rank      if len(func.results) == 1 else None
-        self._shape         = func.results[0].shape     if len(func.results) == 1 else None
-        self._precision     = func.results[0].precision if len(func.results) == 1 else None
-        self._order         = func.results[0].order     if len(func.results) == 1 else None
+        self._dtype         = func.results[0].var.dtype     if len(func.results) == 1 else NativeTuple()
+        self._rank          = func.results[0].var.rank      if len(func.results) == 1 else None
+        self._shape         = func.results[0].var.shape     if len(func.results) == 1 else None
+        self._precision     = func.results[0].var.precision if len(func.results) == 1 else None
+        self._order         = func.results[0].var.order     if len(func.results) == 1 else None
         self._func_name     = func.name
         super().__init__()
 
     @property
     def args(self):
         """ List of FunctionCallArguments provided to the function call
         (contains default values after semantic stage)
@@ -2148,88 +2313,101 @@
             code = repr(self.stmt)+';'
         else:
             code = ''
         return code+"Return({})".format(','.join([repr(e) for e in self.expr]))
 
 class FunctionDef(ScopedNode):
 
-    """Represents a function definition.
+    """
+    Represents a function definition.
+
+    Node containing all the information necessary to describe a function.
+    This information should provide enough information to print a functionally
+    equivalent function in any target language.
 
     Parameters
     ----------
     name : str
         The name of the function.
 
-    arguments : iterable
+    arguments : iterable of FunctionDefArgument
         The arguments to the function.
 
     results : iterable
         The direct outputs of the function.
 
     body : iterable
         The body of the function.
 
     global_vars : list of Symbols
         Variables which will not be passed into the function.
 
-    cls_name: str
-        Class name if the function is a method of cls_name
+    cls_name : str
+        Class name if the function is a method of cls_name.
 
-    is_static: bool
-        True for static functions. Needed for iso_c_binding interface
+    is_static : bool
+        True for static functions. Needed for iso_c_binding interface.
 
-    imports: list, tuple
-        a list of needed imports
+    imports : list, tuple
+        A list of needed imports.
 
-    decorators: list, tuple
-        a list of properties
+    decorators : list, tuple
+        A list of properties.
 
-    headers: list,tuple
-        a list of headers describing the function
+    headers : list,tuple
+        A list of headers describing the function.
 
-    is_recursive: bool
-        True for a function which calls itself
+    is_recursive : bool
+        True for a function which calls itself.
 
-    is_pure: bool
-        True for a function without side effect
+    is_pure : bool
+        True for a function without side effect.
 
-    is_elemental: bool
-        True for a function that is elemental
+    is_elemental : bool
+        True for a function that is elemental.
 
-    is_private: bool
-        True for a function that is private
+    is_private : bool
+        True for a function that is private.
 
-    is_header: bool
-        True for a function which has no body available
+    is_header : bool
+        True for a function which has no body available.
 
-    is_external: bool
-        True for a function which cannot be explicitly imported or renamed
+    is_external : bool
+        True for a function which cannot be explicitly imported or renamed.
 
-    arguments_inout: list, tuple
-        a list of booleans indicating if each argument is modified by the function
+    functions : list, tuple
+        A list of functions defined within this function.
 
-    functions: list, tuple
-        a list of functions defined within this function
+    interfaces : list, tuple
+        A list of interfaces defined within this function.
 
-    interfaces: list, tuple
-        a list of interfaces defined within this function
+    doc_string : str
+        The doc string of the function.
 
-    doc_string: str
-        The doc string of the function
+    scope : parser.scope.Scope
+        The scope containing all objects scoped to the inside of this function.
+
+    See Also
+    --------
+    FunctionDefArgument : The type used to store the arguments.
 
     Examples
     --------
-    >>> from pyccel.ast.core import Assign, Variable, FunctionDef
+    >>> from pyccel.ast.variable import Variable
+    >>> from pyccel.ast.core import FunctionDefArgument, FunctionDefResult
+    >>> from pyccel.ast.core import Assign, FunctionDef
+    >>> from pyccel.ast.operators import PyccelAdd
+    >>> from pyccel.ast.literals import LiteralInteger
     >>> x = Variable('float', 'x')
     >>> y = Variable('float', 'y')
-    >>> args        = [x]
-    >>> results     = [y]
-    >>> body        = [Assign(y,x+1)]
+    >>> args        = [FunctionDefArgument(x)]
+    >>> results     = [FunctionDefResult(y)]
+    >>> body        = [Assign(y,PyccelAdd(x,LiteralInteger(1)))]
     >>> FunctionDef('incr', args, results, body)
-    FunctionDef(incr, (x,), (y,), [y := 1 + x], [], [], None, False, function)
+    FunctionDef(incr, (x,), (y,), [y := x + 1], [], [], None, False, function)
 
     One can also use parametrized argument, using FunctionDefArgument
 
     >>> from pyccel.ast.core import Variable
     >>> from pyccel.ast.core import Assign
     >>> from pyccel.ast.core import FunctionDef
     >>> from pyccel.ast.core import FunctionDefArgument
@@ -2241,15 +2419,15 @@
     >>> body        = [Assign(y,x+n)]
     >>> FunctionDef('incr', args, results, body)
     FunctionDef(incr, (x, n=4), (y,), [y := 1 + x], [], [], None, False, function, [])
     """
     __slots__ = ('_name','_arguments','_results','_body',
                  '_global_vars','_cls_name','_is_static','_imports',
                  '_decorators','_headers','_is_recursive','_is_pure',
-                 '_is_elemental','_is_private','_is_header','_arguments_inout',
+                 '_is_elemental','_is_private','_is_header',
                  '_functions','_interfaces','_doc_string', '_is_external')
     _attribute_nodes = ('_arguments','_results','_body',
                  '_global_vars','_imports','_functions','_interfaces')
 
     def __init__(
         self,
         name,
@@ -2264,15 +2442,14 @@
         headers=(),
         is_recursive=False,
         is_pure=False,
         is_elemental=False,
         is_private=False,
         is_header=False,
         is_external=False,
-        arguments_inout=(),
         functions=(),
         interfaces=(),
         doc_string=None,
         scope=None):
 
         if isinstance(name, str):
             name = PyccelSymbol(name)
@@ -2288,30 +2465,33 @@
         else:
             raise TypeError('Function name must be PyccelSymbol or string')
 
         # arguments
 
         if not iterable(arguments):
             raise TypeError('arguments must be an iterable')
+        if not all(isinstance(a, FunctionDefArgument) for a in arguments):
+            raise TypeError('arguments must be all be FunctionDefArguments')
 
-        arguments = tuple(a if isinstance(a, FunctionDefArgument) else FunctionDefArgument(a) for a in arguments)
+        arg_vars = [a.var for a in arguments]
 
         # body
 
         if iterable(body):
             body = CodeBlock(body)
         elif not isinstance(body,CodeBlock):
             raise TypeError('body must be an iterable or a CodeBlock')
 
 #        body = tuple(i for i in body)
         # results
 
         if not iterable(results):
             raise TypeError('results must be an iterable')
-        results = tuple(results)
+        if not all(isinstance(r, FunctionDefResult) for r in results):
+            raise TypeError('results must be all be FunctionDefResults')
 
         # if method
 
         if cls_name:
 
             if not isinstance(cls_name, str):
                 raise TypeError('cls_name must be a string')
@@ -2341,25 +2521,14 @@
             raise TypeError('Expecting a boolean for header')
 
         if not isinstance(is_external, bool):
             raise TypeError('Expecting a boolean for external')
         else:
             is_external = is_external and is_header and ( len(results) == 1 )
 
-        if arguments_inout:
-            if not isinstance(arguments_inout, (list, tuple)):
-                raise TypeError('Expecting a list or tuple ')
-
-            if not all([isinstance(i, bool) for i in arguments_inout]):
-                raise ValueError('Expecting booleans')
-
-        else:
-            arg_vars = [a.var for a in arguments]
-            arguments_inout = [a.rank>0 and not a.is_const if isinstance(a, Variable) else False for a in arg_vars]
-
         if functions:
             for i in functions:
                 if not isinstance(i, FunctionDef):
                     raise TypeError('Expecting a FunctionDef')
 
         self._name            = name
         self._arguments       = arguments
@@ -2373,15 +2542,14 @@
         self._headers         = headers
         self._is_recursive    = is_recursive
         self._is_pure         = is_pure
         self._is_elemental    = is_elemental
         self._is_private      = is_private
         self._is_header       = is_header
         self._is_external     = is_external
-        self._arguments_inout = arguments_inout
         self._functions       = functions
         self._interfaces      = interfaces
         self._doc_string      = doc_string
         super().__init__(scope)
 
     @property
     def name(self):
@@ -2401,18 +2569,25 @@
     @property
     def body(self):
         """ CodeBlock containing all the statements in the function """
         return self._body
 
     @property
     def local_vars(self):
-        """ List of variables defined in the function """
+        """
+        List of variables defined in the function.
+
+        A list of all variables which are local to the function. This
+        includes arguments, results, and variables defined inside the
+        function.
+        """
         local_vars = self.scope.variables.values()
         argument_vars = [a.var for a in self.arguments]
-        return tuple(l for l in local_vars if l not in self.results and l not in argument_vars)
+        result_vars = [r.var for r in self.results]
+        return tuple(l for l in local_vars if l not in result_vars and l not in argument_vars)
 
     @property
     def global_vars(self):
         """ List of global variables used in the function """
         return self._global_vars
 
     @property
@@ -2500,19 +2675,14 @@
 
     @property
     def is_inline(self):
         """ True if the function should be printed inline """
         return False
 
     @property
-    def arguments_inout(self):
-        """ List of variables which are the modifiable function arguments """
-        return self._arguments_inout
-
-    @property
     def functions(self):
         """ List of functions within this function """
         return self._functions
 
     @property
     def interfaces(self):
         """ List of interfaces within this function """
@@ -2576,15 +2746,14 @@
         'decorators':self._decorators,
         'headers':self._headers,
         'is_recursive':self._is_recursive,
         'is_pure':self._is_pure,
         'is_elemental':self._is_elemental,
         'is_private':self._is_private,
         'is_header':self._is_header,
-        'arguments_inout':self._arguments_inout,
         'functions':self._functions,
         'is_external':self._is_external,
         'interfaces':self._interfaces,
         'doc_string':self._doc_string,
         'scope':self._scope}
         return args, kwargs
```

### Comparing `pyccel-1.7.3/pyccel/ast/cwrapper.py` & `pyccel-1.7.4/pyccel/ast/cwrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 """
 Module representing objects (functions/variables etc) required for the interface
-between python code and C code (using Python/C Api and cwrapper.c).
+between Python code and C code (using Python/C Api and cwrapper.c).
 """
 
 from ..errors.errors import Errors
 from ..errors.messages import PYCCEL_RESTRICTION_TODO
 
 from .basic     import Basic, PyccelAstNode
 
 from .datatypes import DataType, default_precision
 from .datatypes import NativeInteger, NativeFloat, NativeComplex
 from .datatypes import NativeBool, NativeString
 
-from .core      import FunctionDefArgument
+from .core      import FunctionDefArgument, FunctionDefResult
 from .core      import FunctionCall, FunctionDef, FunctionAddress
 
 from .internals import get_final_precision
 
 from .variable  import Variable
 
 from .c_concepts import ObjectAddress
@@ -41,15 +41,15 @@
 #--------- CONSTANTS ----------
     'Py_True',
     'Py_False',
     'Py_None',
     'flags_registry',
 #----- C / PYTHON FUNCTIONS ---
     'Py_DECREF',
-    'PyErr_SetString',
+    'set_python_error_message',
 #----- CHECK FUNCTIONS ---
     'generate_datatype_error',
     'scalar_object_check',
 )
 
 #-------------------------------------------------------------------
 #                        Python DataTypes
@@ -322,42 +322,49 @@
 
 # Python.h object representing None
 Py_None = Variable(PyccelPyObject(), 'Py_None', memory_handling='alias')
 
 # https://docs.python.org/3/c-api/refcounting.html#c.Py_DECREF
 Py_DECREF = FunctionDef(name = 'Py_DECREF',
                         body = [],
-                        arguments = [Variable(dtype=PyccelPyObject(), name='o', memory_handling='alias')],
+                        arguments = [FunctionDefArgument(Variable(dtype=PyccelPyObject(), name='o', memory_handling='alias'))],
                         results = [])
 
 #-------------------------------------------------------------------
 #                      cwrapper.h functions
 #-------------------------------------------------------------------
 
 def Python_to_C(c_object):
     """
-    Create FunctionDef responsible for casting python argument to C
-    Parameters:
+    Create a FunctionDef responsible for casting scalar Python argument to C.
+
+    Creates a FunctionDef node which contains all the code necessary
+    for casting a PythonObject to a C object whose characteristics
+    match that of the object passed as an argument.
+
+    Parameters
     ----------
-    c_object  : Variable
-        The variable needed for the generation of the cast_function
+    c_object : Variable
+        The variable needed for the generation of the cast_function.
+
     Returns
     -------
-    FunctionDef : cast type FunctionDef
+    FunctionDef
+        The function which casts the Python object to C.
     """
     dtype = c_object.dtype
     prec  = get_final_precision(c_object)
     try :
         cast_function = py_to_c_registry[(dtype, prec)]
     except KeyError:
         errors.report(PYCCEL_RESTRICTION_TODO, symbol=dtype,severity='fatal')
     cast_func = FunctionDef(name = cast_function,
                        body      = [],
-                       arguments = [Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias')],
-                       results   = [Variable(dtype=dtype, name = 'v', precision = prec)])
+                       arguments = [FunctionDefArgument(Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias'))],
+                       results   = [FunctionDefResult(Variable(dtype=dtype, name = 'v', precision = prec))])
 
     return cast_func
 
 # Functions definitions are defined in pyccel/stdlib/cwrapper/cwrapper.c
 py_to_c_registry = {
     (NativeBool(), 4)      : 'PyBool_to_Bool',
     (NativeInteger(), 1)   : 'PyInt8_to_Int8',
@@ -367,22 +374,29 @@
     (NativeFloat(), 4)     : 'PyFloat_to_Float',
     (NativeFloat(), 8)     : 'PyDouble_to_Double',
     (NativeComplex(), 4)   : 'PyComplex_to_Complex64',
     (NativeComplex(), 8)   : 'PyComplex_to_Complex128'}
 
 def C_to_Python(c_object):
     """
-    Create FunctionDef responsible for casting c argument to python
-    Parameters:
+    Create a FunctionDef responsible for casting scalar C results to Python.
+
+    Creates a FunctionDef node which contains all the code necessary
+    for casting a C object, whose characteristics match that of the object
+    passed as an argument, to a PythonObject which can be used in Python code.
+
+    Parameters
     ----------
-    c_object  : Variable
-        The variable needed for the generation of the cast_function
+    c_object : Variable
+        The variable needed for the generation of the cast_function.
+
     Returns
     -------
-    FunctionDef : cast type FunctionDef
+    FunctionDef
+        The function which casts the C object to Python.
     """
     if c_object.rank != 0:
         if c_object.order == 'C':
             cast_function = 'c_ndarray_to_pyarray'
         elif c_object.order == 'F':
             cast_function = 'fortran_ndarray_to_pyarray'
         else:
@@ -391,16 +405,16 @@
         try :
             cast_function = c_to_py_registry[(c_object.dtype, c_object.precision)]
         except KeyError:
             errors.report(PYCCEL_RESTRICTION_TODO, symbol=c_object.dtype,severity='fatal')
 
     cast_func = FunctionDef(name = cast_function,
                        body      = [],
-                       arguments = [Variable(dtype=c_object.dtype, name = 'v', precision = c_object.precision)],
-                       results   = [Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias')])
+                       arguments = [FunctionDefArgument(Variable(dtype=c_object.dtype, name = 'v', precision = c_object.precision))],
+                       results   = [FunctionDefResult(Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias'))])
 
     return cast_func
 
 # Functions definitions are defined in pyccel/stdlib/cwrapper/cwrapper.c
 c_to_py_registry = {
     (NativeBool(), -1)     : 'Bool_to_PyBool',
     (NativeBool(), 4)      : 'Bool_to_PyBool',
@@ -420,54 +434,70 @@
 #-------------------------------------------------------------------
 #              errors and check functions
 #-------------------------------------------------------------------
 
 # https://docs.python.org/3/c-api/exceptions.html#c.PyErr_Occurred
 PyErr_Occurred = FunctionDef(name      = 'PyErr_Occurred',
                              arguments = [],
-                             results   = [Variable(dtype = PyccelPyObject(), name = 'r', memory_handling = 'alias')],
+                             results   = [FunctionDefResult(Variable(dtype = PyccelPyObject(), name = 'r', memory_handling = 'alias'))],
                              body      = [])
 
-def PyErr_SetString(exception, message):
+PyErr_SetString = FunctionDef(name = 'PyErr_SetString',
+              body      = [],
+              arguments = [FunctionDefArgument(Variable(dtype = PyccelPyObject(), name = 'o')),
+                           FunctionDefArgument(Variable(dtype = NativeString(), name = 's'))],
+              results   = [])
+
+def set_python_error_message(exception, message):
     """
-    Generate function Call of c/python api PyErr_SetString
+    Generate a function call which sets the Python error.
+
+    Generate a function call of C/Python API PyErr_SetString
     https://docs.python.org/3/c-api/exceptions.html#c.PyErr_SetString
     with a defined error message used to set the error indicator.
 
-    Parameters:
+    Parameters
     ----------
-    exception  : str
-        The exception type
-    message    : str
-        Error message
+    exception : str
+        The error exception type.
+    message : str
+        The message which will be shown.
+
     Returns
-    FunctionCall : raise error FunctionCall
+    -------
+    FunctionCall
+        The FunctionCall which raises the error.
     """
     func = FunctionDef(name = 'PyErr_SetString',
                   body      = [],
-                  arguments = [Variable(dtype = PyccelPyObject(), name = 'o'),
-                               Variable(dtype = NativeString(), name = 's')],
+                  arguments = [FunctionDefArgument(Variable(dtype = PyccelPyObject(), name = 'o')),
+                               FunctionDefArgument(Variable(dtype = NativeString(), name = 's'))],
                   results   = [])
 
     exception = Variable(PyccelPyObject(), name = exception)
 
     return FunctionCall(func, [exception, message])
 
 
 def generate_datatype_error(variable):
     """
-    Generate TypeError exception from the variable information (datatype, precision)
-    Parameters:
+    Generate TypeError exception from the variable information.
+
+    Generate a TypeError exception indicated that the variable passed
+    as an argument does not have the right datatype/precision.
+
+    Parameters
     ----------
     variable : Variable
+        The variable which indicates the correct datatype/precision.
 
-    Returns:
+    Returns
     -------
-    func     : FunctionCall
-        call to PyErr_SetString with TypeError as exception and custom message
+    FunctionCall
+        Call to PyErr_SetString with TypeError as exception and custom message.
     """
     dtype     = variable.dtype
 
     if variable.precision == -1:
         precision = 'native '
     elif isinstance(dtype, NativeBool):
         precision = ''
@@ -475,15 +505,15 @@
         precision = '{} bit '.format(variable.precision * 2 * 8)
     else:
         precision = '{} bit '.format(variable.precision * 8)
 
     message = '"Argument must be {precision}{dtype}"'.format(
             precision = precision,
             dtype     = variable.dtype)
-    return PyErr_SetString('PyExc_TypeError', message)
+    return set_python_error_message('PyExc_TypeError', message)
 
 
 # Functions definitions are defined in pyccel/stdlib/cwrapper/cwrapper.c
 check_type_registry = {
     (NativeBool(), -1)     : 'PyIs_Bool',
     (NativeBool(), 4)      : 'PyIs_Bool',
     (NativeInteger(), -1)  : 'PyIs_NativeInt',
@@ -496,32 +526,37 @@
     (NativeFloat(), 8)     : 'PyIs_Double',
     (NativeComplex(), -1)  : 'PyIs_NativeComplex',
     (NativeComplex(), 4)   : 'PyIs_Complex64',
     (NativeComplex(), 8)   : 'PyIs_Complex128'}
 
 def scalar_object_check(py_object, c_object):
     """
-    Create FunctionCall responsible for checking python argument data type
-    Parameters:
+    Create FunctionCall responsible for checking Python argument data type.
+
+    Create a FunctionCall which checks whether the Python argument
+    passed as an argument is a scalar with a type which matches the
+    type of the C object.
+
+    Parameters
     ----------
-    py_object  : Variable
-        The python argument of the check function
-    c_object   : Variable
-        The variable needed for the generation of the type check
-    precision_check : Boolean
-        True if checking the exact precision is needed
+    py_object : Variable
+        The Python argument of the check function.
+    c_object : Variable
+        The variable needed for the generation of the type check.
+
     Returns
     -------
-    FunctionCall : Check type FunctionCall
+    FunctionCall
+        Check type FunctionCall.
     """
 
     try :
         check_type = check_type_registry[c_object.dtype, c_object.precision]
     except KeyError:
         errors.report(PYCCEL_RESTRICTION_TODO, symbol=c_object.dtype,severity='fatal')
 
     check_func = FunctionDef(name = check_type,
                     body      = [],
-                    arguments = [Variable(dtype=PyccelPyObject(), name = 'o', memory_handling = 'alias')],
-                    results   = [Variable(dtype=NativeBool(), name = 'r')])
+                    arguments = [FunctionDefArgument(Variable(dtype=PyccelPyObject(), name = 'o', memory_handling = 'alias'))],
+                    results   = [FunctionDefResult(Variable(dtype=NativeBool(), name = 'r'))])
 
     return FunctionCall(check_func, [py_object])
```

### Comparing `pyccel-1.7.3/pyccel/ast/datatypes.py` & `pyccel-1.7.4/pyccel/ast/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/functionalexpr.py` & `pyccel-1.7.4/pyccel/ast/functionalexpr.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/headers.py` & `pyccel-1.7.4/pyccel/ast/headers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pyccel.utilities.strings import create_incremented_string
 from ..errors.errors    import Errors
 from ..errors.messages  import TEMPLATE_IN_UNIONTYPE
 from .basic             import Basic, iterable
 from .core              import Assign, FunctionCallArgument
 from .core              import FunctionDef, FunctionCall, FunctionAddress
+from .core              import FunctionDefArgument, FunctionDefResult
 from .datatypes         import datatype, DataTypeFactory, UnionType, default_precision
 from .internals         import PyccelSymbol, Slice
 from .macros            import Macro, MacroShape, construct_macro
 from .variable          import DottedName, DottedVariable
 from .variable          import Variable
 
 __all__ = (
@@ -190,33 +191,38 @@
            to create the initial version of the object
            and its arguments
         """
         return (self.__class__, (self.name, self.dtypes))
 
 #==============================================================================
 class FunctionHeader(Header):
-    """Represents function/subroutine header in the code.
+    """
+    Represents function/subroutine header in the code.
+
+    A node which represents the header for a function/subroutine.
+    It describes all the type information provided in the header
+    so that a typed function can be created.
 
     Parameters
     ----------
-    name: str
-        function/subroutine name
+    name : str
+        Function/subroutine name.
 
-    dtypes: tuple/list
-        a list of datatypes. an element of this list can be str/DataType of a
-        tuple (str/DataType, attr, allocatable)
-
-    results: tuple/list
-        a list of datatypes. an element of this list can be str/DataType of a
-        tuple (str/DataType, attr, allocatable)
-
-    is_static: bool
-        True if we want to pass arrays in bind(c) mode. every argument of type
-        array will be preceeded by its shape, the later will appear in the
-        argument declaration. default value: False
+    dtypes : tuple/list
+        A list of datatypes. An element of this list can be str/DataType of a
+        tuple (str/DataType, attr, allocatable).
+
+    results : tuple/list
+        A list of datatypes. An element of this list can be str/DataType of a
+        tuple (str/DataType, attr, allocatable).
+
+    is_static : bool, default: False
+        True if we want to pass arrays in bind(c) mode. Every argument of type
+        array will be preceeded by its shape, which will also appear in the
+        argument declaration.
 
     Examples
     --------
 
     >>> from pyccel.ast.headers import FunctionHeader
     >>> FunctionHeader('f', ['double'])
     FunctionHeader(f, [(NativeDouble(), [])])
@@ -257,56 +263,101 @@
         return self._results
 
     @property
     def is_static(self):
         return self._is_static
 
     def create_definition(self, templates = (), is_external=False):
-        """Returns a FunctionDef with empy body."""
+        """
+        Create a FunctionDef with the described types.
+
+        Create a FunctionDef with arguments and results whose types
+        are indicated by the information stored in the header. The
+        body of the function is left empty.
+
+        Parameters
+        ----------
+        templates : list/tuple, default: ()
+            A list of all templates defined in the context which can be used
+            to define argument or result types.
+
+        is_external : bool, default: False
+            Indicates whether the function is an external function which
+            is defined elsewhere in the linked files.
+
+        Returns
+        -------
+        list of FunctionDef
+            A list of all functions described by the header.
+        """
         # TODO factorize what can be factorized
         from itertools import product
 
         name = self.name
 
         body      = []
         cls_name  = None
         is_static = self.is_static
         used_names = set(name)
         imports   = []
         funcs = []
         dtypes = []
 
         def build_argument(var_name, dc):
-            #Constructs an argument variable from a dictionary.
+            """
+            Construct an argument variable from a dictionary describing its properties.
+
+            Use a dictionary describing the properties of a variable which is either
+            an argument (in/inout) or a result (out) to create a variable and an
+            annotation string for the variable.
+
+            Parameters
+            ----------
+            var_name : srt
+                The name of the variable.
+
+            dc : dict
+                The properties of the variable.
+
+            Returns
+            -------
+            Variable
+                The newly created variable.
+
+            str
+                The annotation string.
+            """
             dtype    = dc['datatype']
             memory_handling = dc['memory_handling']
             precision = dc['precision']
             rank = dc['rank']
             is_const = dc['is_const']
 
             order = None
             shape = None
+            annotation = None
 
             if rank and precision == -1:
                 precision = default_precision[dtype]
 
             if rank >1:
                 order = dc['order']
 
             if isinstance(dtype, str):
+                annotation = dtype
                 try:
                     dtype = datatype(dtype)
                 except ValueError:
                     dtype = DataTypeFactory(str(dtype), ("_name"))()
             var = Variable(dtype, var_name,
                            memory_handling=memory_handling, is_const=is_const,
                            rank=rank, shape=shape ,order=order, precision=precision,
-                           is_argument=True, is_temp=True)
+                           is_temp=True)
 
-            return var
+            return var, annotation
 
         def process_template(signature, Tname, d_type):
             #Replaces templates named Tname inside signature, with the given type.
             new_sig = tuple(d_type if 'datatype' in t and t['datatype'] == Tname\
                             else t for t in signature)
             return new_sig
 
@@ -345,36 +396,37 @@
                 # TODO  handle function as argument, which itself has a function argument
                 if (d['is_func']):
                     decs = []
                     results = []
                     _count = 0
                     for dc in d['decs']:
                         _name, _count = create_incremented_string(used_names, 'in', _count)
-                        var = build_argument(_name, dc)
-                        decs.append(var)
+                        var, annotation = build_argument(_name, dc)
+                        decs.append(FunctionDefArgument(var, annotation=annotation))
                     _count = 0
                     for dc in d['results']:
                         _name, _count = create_incremented_string(used_names, 'out', _count)
-                        var = build_argument(_name, dc)
-                        results.append(var)
+                        var, annotation = build_argument(_name, dc)
+                        results.append(FunctionDefResult(var, annotation=annotation))
                     arg_name = 'arg_{0}'.format(str(i))
-                    arg = FunctionAddress(arg_name, decs, results, [])
+                    arg = FunctionDefArgument(FunctionAddress(arg_name, decs, results, []))
 
                 else:
                     arg_name = 'arg_{0}'.format(str(i))
-                    arg = build_argument(arg_name, d)
+                    var, annotation = build_argument(arg_name, d)
+                    arg = FunctionDefArgument(var, annotation=annotation)
                 args.append(arg)
 
             # ... factorize the following 2 blocks
             results = []
             for i,d_var in enumerate(self.results):
                 is_func = d_var.pop('is_func')
                 dtype = d_var.pop('datatype')
                 var = Variable(dtype, 'res_{}'.format(i), **d_var, is_temp = True)
-                results.append(var)
+                results.append(FunctionDefResult(var, annotation = str(dtype)))
                 # we put back dtype otherwise macro will crash when it tries to
                 # call create_definition
                 d_var['datatype'] = dtype
                 d_var['is_func'] = is_func
 
             func= FunctionDef(name, args, results, body,
                               global_vars=[],
```

### Comparing `pyccel-1.7.3/pyccel/ast/internals.py` & `pyccel-1.7.4/pyccel/ast/internals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/itertoolsext.py` & `pyccel-1.7.4/pyccel/ast/itertoolsext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/literals.py` & `pyccel-1.7.4/pyccel/ast/literals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/macros.py` & `pyccel-1.7.4/pyccel/ast/macros.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/mathext.py` & `pyccel-1.7.4/pyccel/ast/mathext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/numpy_wrapper.py` & `pyccel-1.7.4/pyccel/ast/numpy_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 """
-Handling the transitions between python code and C code using (Numpy/C Api).
+Handling the transitions between Python code and C code using (Numpy/C Api).
 """
 
 import numpy as np
 
 from .datatypes         import (NativeInteger, NativeFloat, NativeComplex,
                                 NativeBool, NativeGeneric, NativeVoid)
 
 from .cwrapper          import PyccelPyObject
 
 from .core              import FunctionDef, FunctionCall
+from .core              import FunctionDefArgument, FunctionDefResult
 
 from .internals         import get_final_precision
 
 from .literals          import LiteralInteger
 
 from .variable          import Variable
 
@@ -60,59 +61,59 @@
 
     return '#ifndef NPY_NO_DEPRECATED_API\n'+ \
             numpy_api_macro+\
            '#endif'
 
 PyArray_Check = FunctionDef(name      = 'PyArray_Check',
                             body      = [],
-                            arguments = [Variable(dtype=PyccelPyObject(), name = 'o')],
-                            results   = [Variable(dtype=NativeBool(), name='b')])
+                            arguments = [FunctionDefArgument(Variable(dtype=PyccelPyObject(), name = 'o'))],
+                            results   = [FunctionDefResult(Variable(dtype=NativeBool(), name='b'))])
 
 # numpy array to c ndarray : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 pyarray_to_ndarray = FunctionDef(
                 name      = 'pyarray_to_ndarray',
-                arguments = [Variable(name = 'a', dtype = PyccelPyObject(), memory_handling = 'alias')],
+                arguments = [FunctionDefArgument(Variable(name = 'a', dtype = PyccelPyObject(), memory_handling = 'alias'))],
                 body      = [],
-                results   = [Variable(name = 'array', dtype = NativeGeneric())])
+                results   = [FunctionDefResult(Variable(name = 'array', dtype = NativeGeneric()))])
 
 # numpy array check elements : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 pyarray_check = FunctionDef(
                 name      = 'pyarray_check',
                 arguments = [
-                        Variable(name = 'a', dtype = PyccelPyObject(), memory_handling='alias'),
-                        Variable(name = 'dtype', dtype = NativeInteger()),
-                        Variable(name = 'rank', dtype = NativeInteger()),
-                        Variable(name = 'flag', dtype = NativeInteger())
+                        FunctionDefArgument(Variable(name = 'a', dtype = PyccelPyObject(), memory_handling='alias')),
+                        FunctionDefArgument(Variable(name = 'dtype', dtype = NativeInteger())),
+                        FunctionDefArgument(Variable(name = 'rank', dtype = NativeInteger())),
+                        FunctionDefArgument(Variable(name = 'flag', dtype = NativeInteger()))
                     ],
                 body      = [],
-                results   = [Variable(name = 'b', dtype = NativeBool())])
+                results   = [FunctionDefResult(Variable(name = 'b', dtype = NativeBool()))])
 
 is_numpy_array = FunctionDef(
                 name      = 'is_numpy_array',
                 arguments = [
-                        Variable(name = 'a', dtype = PyccelPyObject(), memory_handling='alias'),
-                        Variable(name = 'dtype', dtype = NativeInteger()),
-                        Variable(name = 'rank', dtype = NativeInteger()),
-                        Variable(name = 'flag', dtype = NativeInteger())
+                        FunctionDefArgument(Variable(name = 'a', dtype = PyccelPyObject(), memory_handling='alias')),
+                        FunctionDefArgument(Variable(name = 'dtype', dtype = NativeInteger())),
+                        FunctionDefArgument(Variable(name = 'rank', dtype = NativeInteger())),
+                        FunctionDefArgument(Variable(name = 'flag', dtype = NativeInteger()))
                     ],
                 body      = [],
-                results   = [Variable(name = 'b', dtype = NativeBool())])
+                results   = [FunctionDefResult(Variable(name = 'b', dtype = NativeBool()))])
 
 # Return the shape of the n-th dimension : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 array_get_dim  = FunctionDef(name    = 'nd_ndim',
                            body      = [],
-                           arguments = [Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias'),
-                                        Variable(dtype=NativeInteger(), name = 'idx')],
-                           results   = [Variable(dtype=NativeInteger(), name = 'd')])
+                           arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias')),
+                                        FunctionDefArgument(Variable(dtype=NativeInteger(), name = 'idx'))],
+                           results   = [FunctionDefResult(Variable(dtype=NativeInteger(), name = 'd'))])
 
 # Return the data of ndarray : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 array_get_data  = FunctionDef(name   = 'nd_data',
                            body      = [],
-                           arguments = [Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias')],
-                           results   = [Variable(dtype=NativeVoid(), name = 'v', memory_handling='alias', rank = 1)])
+                           arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias'))],
+                           results   = [FunctionDefResult(Variable(dtype=NativeVoid(), name = 'v', memory_handling='alias', rank = 1))])
 
 # Basic Array Flags
 # https://numpy.org/doc/stable/reference/c-api/array.html#c.NPY_ARRAY_OWNDATA
 numpy_flag_own_data     = Variable(dtype=NativeInteger(),  name = 'NPY_ARRAY_OWNDATA')
 # https://numpy.org/doc/stable/reference/c-api/array.html#c.NPY_ARRAY_C_CONTIGUOUS
 numpy_flag_c_contig     = Variable(dtype=NativeInteger(),  name = 'NPY_ARRAY_C_CONTIGUOUS')
 # https://numpy.org/doc/stable/reference/c-api/array.html#c.NPY_ARRAY_F_CONTIGUOUS
@@ -252,30 +253,38 @@
         return FunctionCall(pyarray_check, [py_variable, type_ref, LiteralInteger(rank), flag])
     else:
         return FunctionCall(is_numpy_array, [py_variable, type_ref, LiteralInteger(rank), flag])
 
 
 def scalar_type_check(py_variable, c_variable):
     """
-    Create FunctionCall responsible of checking numpy argument data type
-    Parameters:
+    Create a FunctionCall to check the type of a Python object.
+
+    Create a FunctionCall object representing a call to a function which
+    is responsible for checking if the Python object passed as an argument
+    has a type matching that of the provided C object.
+
+    Parameters
     ----------
     py_variable : Variable
-        The python argument of the check function
+        The Python argument of the check function.
+
     c_variable : Variable
-        The variable needed for the generation of the type check
+        The variable needed for the generation of the type check.
+
     Returns
     -------
-    FunctionCall : Check type FunctionCall
+    FunctionCall
+        The FunctionCall which checks the type.
     """
     try :
         check_numpy_ref = numpy_type_check_registry[(c_variable.dtype, c_variable.precision)]
     except KeyError:
         errors.report(PYCCEL_RESTRICTION_TODO, symbol=c_variable.dtype,severity='fatal')
 
     check_numpy_func = FunctionDef(name = 'PyArray_IsScalar',
                               body      = [],
-                              arguments = [Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias'),
-                                           check_numpy_ref],
-                              results   = [Variable(dtype=NativeBool(), name = 'r')])
+                              arguments = [FunctionDefArgument(Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias')),
+                                           FunctionDefArgument(check_numpy_ref)],
+                              results   = [FunctionDefResult(Variable(dtype=NativeBool(), name = 'r'))])
 
     return FunctionCall(check_numpy_func, [py_variable, check_numpy_ref])
```

### Comparing `pyccel-1.7.3/pyccel/ast/numpyext.py` & `pyccel-1.7.4/pyccel/ast/numpyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/omp.py` & `pyccel-1.7.4/pyccel/ast/omp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/operators.py` & `pyccel-1.7.4/pyccel/ast/operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/scipyext.py` & `pyccel-1.7.4/pyccel/ast/scipyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/sympy_helper.py` & `pyccel-1.7.4/pyccel/ast/sympy_helper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/sysext.py` & `pyccel-1.7.4/pyccel/ast/sysext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/ast/utilities.py` & `pyccel-1.7.4/pyccel/ast/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 errors = Errors()
 
 __all__ = (
     'LoopCollection',
     'builtin_function',
     'builtin_import',
-    'builtin_import_registery',
+    'builtin_import_registry',
     'split_positional_keyword_arguments',
 )
 
 #==============================================================================
 def builtin_function(expr, args=None):
     """Returns a builtin-function call applied to given arguments."""
 
@@ -77,40 +77,53 @@
 #==============================================================================
 decorators_mod = Module('decorators',(),
         funcs = [PyccelFunctionDef(d, PyccelInternalFunction) for d in pyccel_decorators.__all__])
 pyccel_mod = Module('pyccel',(),(),
         imports = [Import('decorators', decorators_mod)])
 
 # TODO add documentation
-builtin_import_registery = Module('__main__',
+builtin_import_registry = Module('__main__',
         (),(),
         imports = [
-            Import('numpy', AsName(numpy_mod,'numpy')),
-            Import('scipy', AsName(scipy_mod,'scipy')),
-            Import('itertools', AsName(itertools_mod,'itertools')),
-            Import('math', AsName(math_mod,'math')),
-            Import('pyccel', AsName(pyccel_mod,'pyccel')),
-            Import('sys', AsName(sys_mod,'sys')),
+            Import('numpy', numpy_mod),
+            Import('scipy', scipy_mod),
+            Import('itertools', itertools_mod),
+            Import('math', math_mod),
+            Import('pyccel', pyccel_mod),
+            Import('sys', sys_mod),
             ])
 if sys.version_info < (3, 10):
     from .builtin_imports import python_builtin_libs
 else:
     python_builtin_libs = set(sys.stdlib_module_names) # pylint: disable=no-member
 
-recognised_libs = python_builtin_libs | builtin_import_registery.keys()
+recognised_libs = python_builtin_libs | builtin_import_registry.keys()
 
 def recognised_source(source_name):
-    """ Determine whether the imported source is recognised by pyccel.
-    If it is not recognised then it should be imported and translated
+    """
+    Determine whether the imported source is recognised by pyccel.
+
+    Determine whether the imported source is recognised by pyccel.
+    If it is not recognised then it will need to be imported and translated.
+
+    Parameters
+    ----------
+    source_name : str
+        The name of the imported module.
+
+    Returns
+    -------
+    bool
+        True if the source is recognised, False otherwise.
     """
     source = str(source_name).split('.')
-    if source[0] in python_builtin_libs and source[0] not in builtin_import_registery.keys():
+    if source[0] in python_builtin_libs and source[0] not in builtin_import_registry.keys():
         return True
     else:
-        return source_name in builtin_import_registery
+        return source_name in builtin_import_registry
 
 #==============================================================================
 def collect_relevant_imports(module, targets):
     """
     Extract all objects necessary to create imports from a module given a list of targets
 
     Parameters
@@ -136,31 +149,48 @@
             code_name = import_name
 
         if import_name in module.keys():
             imports.append((code_name, module[import_name]))
     return imports
 
 def builtin_import(expr):
-    """Returns a builtin pyccel-extension function/object from an import."""
+    """
+    Return a Pyccel-extension function/object from an import of a recognised module.
+
+    Examine an Import object which imports something which is recognised by
+    Pyccel internally. The object(s) imported are then returned for use in the
+    code.
+
+    Parameters
+    ----------
+    expr : Import
+        The expression which imports the module.
+
+    Returns
+    -------
+    list
+        A list of 2-tuples. The first element is the name of the imported object,
+        the second element is the object itself.
+    """
 
     if not isinstance(expr, Import):
         raise TypeError('Expecting an Import expression')
 
     if isinstance(expr.source, AsName):
         source = expr.source.name
     else:
         source = str(expr.source)
 
-    if source in builtin_import_registery:
+    if source in builtin_import_registry:
         if expr.target:
-            return collect_relevant_imports(builtin_import_registery[source], expr.target)
+            return collect_relevant_imports(builtin_import_registry[source], expr.target)
         elif isinstance(expr.source, AsName):
-            return [(expr.source.target, builtin_import_registery[source])]
+            return [(expr.source.target, builtin_import_registry[source])]
         else:
-            return [(expr.source, builtin_import_registery[source])]
+            return [(expr.source, builtin_import_registry[source])]
 
     return []
 
 #==============================================================================
 def get_function_from_ast(ast, func_name):
     node = None
     for stmt in ast:
@@ -321,45 +351,53 @@
 #==============================================================================
 
 LoopCollection = namedtuple('LoopCollection', ['body', 'length', 'modified_vars'])
 
 #==============================================================================
 def collect_loops(block, indices, new_index, language_has_vectors = False, result = None):
     """
+    Collect blocks of code into loops.
+
     Run through a code block and split it into lists of tuples of lists where
     each inner list represents a code block and the tuples contain the lists
     and the size of the code block.
     So the following:
-    a = a+b
+    `a = a+b`
     for a: int[:,:] and b: int[:]
     Would be returned as:
+    ```
     [
       ([
         ([a[i,j]=a[i,j]+b[j]],a.shape[1])
        ]
        , a.shape[0]
       )
     ]
+    ```
 
     Parameters
-    ==========
-    block                 : list of Ast Nodes
-                            The expressions to be modified
-    indices               : list
-                            An empty list to be filled with the temporary variables created
-    new_index             : function (class method of a Scope)
-                            A function which provides a new variable from a base name,
-                            avoiding name collisions.
-    language_has_vectors  : bool
-                            Indicates if the language has support for vector
-                            operations of the same shape
-    Results
-    =======
-    block : list of tuples of lists
-            The modified expression
+    ----------
+    block : list of Ast Nodes
+        The expressions to be modified.
+    indices : list
+        An empty list to be filled with the temporary variables created.
+    new_index : function (class method of a Scope)
+        A function which provides a new variable from a base name,
+        avoiding name collisions.
+    language_has_vectors : bool
+        Indicates if the language has support for vector
+        operations of the same shape.
+    result : list, default: None
+        The list which will be returned. If none is provided, a new list
+        is created.
+
+    Returns
+    -------
+    list of tuples of lists
+        The modified expression.
     """
     if result is None:
         result = []
     current_level = 0
     array_creator_types = (Allocate, PythonList, PythonTuple, Concatenate, Duplicate)
     is_function_call = lambda f: ((isinstance(f, FunctionCall) and not f.funcdef.is_elemental)
                                 or (isinstance(f, PyccelInternalFunction) and not f.is_elemental and not hasattr(f, '__getitem__')
@@ -441,15 +479,15 @@
 
 
             if any(len(f.funcdef.results)!=1 for f in funcs):
                 errors.report("Loop unravelling cannot handle function calls "\
                         "which return tuples or None",
                         symbol=line, severity='fatal')
 
-            func_results = [f.funcdef.results[0] for f in funcs]
+            func_results = [f.funcdef.results[0].var for f in funcs]
             func_vars2 = [new_index(r.dtype, r.name) for r in func_results]
             assigns   += [Assign(v, f) for v,f in zip(func_vars2, funcs)]
 
             if assigns:
                 # For now we do not handle memory allocation in loop unravelling
                 if any(v.rank > 0 for v in func_vars1) or any(v.rank > 0 for v in func_results):
                     errors.report("Loop unravelling cannot handle extraction of function calls "\
```

### Comparing `pyccel-1.7.3/pyccel/ast/variable.py` & `pyccel-1.7.4/pyccel/ast/variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,84 +32,89 @@
     'IndexedElement',
     'InhomogeneousTupleVariable',
     'TupleVariable',
     'Variable'
 )
 
 class Variable(PyccelAstNode):
+    """
+    Represents a typed variable.
 
-    """Represents a typed variable.
+    Represents a variable in the code and stores all useful properties which allow
+    for easy usage of this variable.
 
     Parameters
     ----------
     dtype : str, DataType
         The type of the variable. Can be either a DataType,
         or a str (bool, int, float).
 
     name : str, list, DottedName
         The name of the variable represented. This can be either a string
         or a dotted name, when using a Class attribute.
 
-    rank : int
-        used for arrays. [Default value: 0]
-
-    memory_handling: str
-        'heap' is used for arrays, if we need to allocate memory on the heap
-        'stack' if memory should be allocated on the stack, represents stack arrays and scalars
-        'alias' if object allows access to memory stored in another variable
-        [Default value: 'stack']
+    rank : int, default: 0
+        The number of dimensions for an array.
 
-    is_target: bool
-        if object is pointed to by another variable [Default value: False]
+    memory_handling : str, default: 'stack'
+        'heap' is used for arrays, if we need to allocate memory on the heap.
+        'stack' if memory should be allocated on the stack, represents stack arrays and scalars.
+        'alias' if object allows access to memory stored in another variable.
 
-    is_optional: bool
-        if object is an optional argument of a function [Default value: False]
+    is_const : bool, default: False
+        Indicates if object is a const argument of a function.
 
-    shape: int or list
-        shape of the array. [Default value: None]
+    is_target : bool, default: False
+        Indicates if object is pointed to by another variable.
 
-    cls_base: class
-        class base if variable is an object or an object member [Default value: None]
+    is_optional : bool, default: False
+        Indicates if object is an optional argument of a function.
 
-    order : str
-        used for arrays. Indicates whether the data is stored in C or Fortran format in memory [Default value: 'C']
+    is_private : bool, default: False
+        Indicates if object is private within a Module.
 
-    precision : str
-        Precision of the data type [Default value: depends on the datatype]
+    shape : tuple, default: None
+        The shape of the array. A tuple whose elements indicate the number of elements along
+        each of the dimensions of an array. The elements of the tuple should be None or PyccelAstNodes.
 
-    is_argument: bool
-        if object is the argument of a function [Default value: False]
+    cls_base : class, default: None
+        Class base if variable is an object or an object member.
 
-    is_kwonly: bool
-        if object is an argument which can only be specified using its keyword
+    order : str, default: 'C'
+        Used for arrays. Indicates whether the data is stored in C or Fortran format in memory.
+        See order_docs.md in the developer docs for more details.
 
-    is_const: bool
-        if object is a const argument of a function [Default value: False]
+    precision : str, default: 0
+        Precision of the data type.
 
-    is_private: bool
-        if object is private within a Module [Default value: False]
+    is_argument : bool, default: False
+        Indicates if object is the argument of a function.
 
-    is_temp: bool
+    is_temp : bool, default: False
         Indicates if this symbol represents a temporary variable created by Pyccel,
-        and was not present in the original Python code [default value : False].
+        and was not present in the original Python code.
+
+    allows_negative_indexes : bool, default: False
+        Indicates if non-literal negative indexes should be correctly handled when indexing this
+        variable. The default is False for performance reasons.
 
     Examples
     --------
     >>> from pyccel.ast.core import Variable
     >>> Variable('int', 'n')
     n
     >>> n = 4
     >>> Variable('float', 'x', rank=2, shape=(n,2), memory_handling='heap')
     x
     >>> Variable('int', DottedName('matrix', 'n_rows'))
     matrix.n_rows
     """
     __slots__ = ('_name', '_alloc_shape', '_memory_handling', '_is_const',
             '_is_target', '_is_optional', '_allows_negative_indexes',
-            '_cls_base', '_is_argument', '_is_kwonly', '_is_temp','_dtype','_precision',
+            '_cls_base', '_is_argument', '_is_temp','_dtype','_precision',
             '_rank','_shape','_order','_is_private')
     _attribute_nodes = ()
 
     def __init__(
         self,
         dtype,
         name,
@@ -121,15 +126,14 @@
         is_optional=False,
         is_private=False,
         shape=None,
         cls_base=None,
         order=None,
         precision=0,
         is_argument=False,
-        is_kwonly=False,
         is_temp =False,
         allows_negative_indexes=False
         ):
         super().__init__()
 
         # ------------ Variable Properties ---------------
         # if class attribute
@@ -170,15 +174,14 @@
         if not isinstance(allows_negative_indexes, bool):
             raise TypeError('allows_negative_indexes must be a boolean.')
         self._allows_negative_indexes = allows_negative_indexes
 
         self._cls_base       = cls_base
         self._order          = order
         self._is_argument    = is_argument
-        self._is_kwonly      = is_kwonly
         self._is_temp        = is_temp
 
         # ------------ PyccelAstNode Properties ---------------
         if isinstance(dtype, str) or str(dtype) == '*':
 
             dtype = datatype(str(dtype))
         elif not isinstance(dtype, DataType):
@@ -380,21 +383,22 @@
     @property
     def is_argument(self):
         """ Indicates whether the Variable is
         a function argument in this context
         """
         return self._is_argument
 
-    @property
-    def is_kwonly(self):
-        """ If the Variable is an argument then this
-        indicates whether the argument is a keyword
-        only argument
+    def declare_as_argument(self):
+        """
+        Indicate that the variable is used as an argument.
+
+        This function is called by FunctionDefArgument to ensure that
+        arguments are correctly flagged as such.
         """
-        return self._is_kwonly
+        self._is_argument = True
 
     @property
     def is_ndarray(self):
         """user friendly method to check if the variable is an ndarray:
             1. have a rank > 0
             2. dtype is one among {int, bool, float, complex}
         """
```

### Comparing `pyccel-1.7.3/pyccel/codegen/codegen.py` & `pyccel-1.7.4/pyccel/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/codegen/compiling/basic.py` & `pyccel-1.7.4/pyccel/codegen/compiling/basic.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,45 +9,54 @@
 """
 import os
 import sys
 from filelock import FileLock
 
 class CompileObj:
     """
-    Class containing all information necessary for compiling
+    Class containing all information necessary for compiling.
+
+    A class which stores all information which may be needed in order to
+    compile an object. This includes its name, location, and all dependencies
+    and flags which may need to be passed to the compiler.
 
     Parameters
     ----------
-    file_name     : str
-                    Name of file to be compiled
+    file_name : str
+        Name of file to be compiled.
+
+    folder : str
+        Name of the folder where the file is found.
 
-    folder        : str
-                    Name of the folder where the file is found
+    flags : str
+        Any non-default flags passed to the compiler.
 
-    flags         : str
-                    Any non-default flags passed to the compiler
+    includes : iterable of strs
+        Include directories paths.
 
-    includes      : iterable of strs
-                    include directories paths
+    libs : iterable of strs
+        Required libraries.
 
-    libs          : iterable of strs
-                    required libraries
+    libdirs : iterable of strs
+        Paths to directories containing the required libraries.
 
-    libdirs       : iterable of strs
-                    paths to directories containing the required libraries
+    dependencies : iterable of CompileObjs
+        Objects which must also be compiled in order to compile this module/program.
 
-    dependencies  : iterable of CompileObjs
-                    objects which must also be compiled in order to compile this module/program
+    accelerators : iterable of str
+        Tool used to accelerate the code (e.g. openmp openacc).
 
-    accelerators  : str
-                    Tool used to accelerate the code (e.g. openmp openacc)
+    has_target_file : bool, default : True
+        If set to false then this flag indicates that the file has no target.
+        Eg an interface for a library.
 
-    has_target_file : bool
-                    If set to false then this flag indicates that the file has no target.
-                    Eg an interface for a library
+    prog_target : str, default: None
+        The name of the executable that should be generated if this file is a
+        program. If no name is provided then the module name deduced from the file
+        name is used.
     """
     __slots__ = ('_file','_folder','_module_name','_module_target','_prog_target',
                  '_lock','_flags','_includes','_libs','_libdirs','_accelerators',
                  '_dependencies','_has_target_file')
     def __init__(self,
                  file_name,
                  folder,
@@ -83,17 +92,15 @@
         if has_target_file:
             self._includes     = set([folder, *includes])
         else:
             self._includes = set(includes)
         self._libs         = list(libs)
         self._libdirs      = set(libdirs)
         self._accelerators = set(accelerators)
-        self._dependencies = dict()
-        if dependencies:
-            self.add_dependencies(*dependencies)
+        self._dependencies = {a.module_target:a for a in dependencies}
         self._has_target_file = has_target_file
 
     def reset_folder(self, folder):
         """
         Change the folder in which the source file is saved (useful for stdlib)
         """
         if self.has_target_file:
@@ -147,29 +154,42 @@
     def flags(self):
         """ Returns the additional flags required to compile the file
         """
         return self._flags
 
     @property
     def includes(self):
-        """ Returns the additional include directories required to compile the file
         """
-        return self._includes
+        Get the additional include directories required to compile the file.
+
+        Return a set containing all the directories which must be passed to the
+        compiler via the include flag `-I`.
+        """
+        return self._includes.union([di for d in self._dependencies.values() for di in d.includes])
 
     @property
     def libs(self):
-        """ Returns the additional libraries required to compile the file
         """
-        return self._libs
+        Get the additional libraries required to compile the file.
+
+        Return a list containing all the libraries which must be passed to the
+        compiler via the library flag `-l`.
+        """
+        return self._libs+[dl for d in self._dependencies.values() for dl in d.libs]
 
     @property
     def libdirs(self):
-        """ Returns the additional library directories required to compile the file
         """
-        return self._libdirs
+        Get the additional library directories required to compile the file.
+
+        Return a set containing all the directories which must be passed to the
+        compiler via the library directory flag `-L` so that the necessary
+        libraries can be correctly located.
+        """
+        return self._libdirs.union([dld for d in self._dependencies.values() for dld in d.libdirs])
 
     @property
     def extra_modules(self):
         """ Returns the additional objects required to compile the file
         """
         deps = set()
         for d in self._dependencies.values():
@@ -196,19 +216,14 @@
         Parameters
         ----------
         *args : CompileObj
         """
         if not all(isinstance(d, CompileObj) for d in args):
             raise TypeError("Dependencies require necessary compile information")
         self._dependencies.update({a.module_target:a for a in args})
-        for a in args:
-            self._includes.update(a.includes)
-            self._libs.extend(a.libs)
-            self._libdirs.update(a.libdirs)
-            self._accelerators.update(a.accelerators)
 
     def acquire_lock(self):
         """
         Lock the file and its dependencies to prevent race conditions
         """
         self.acquire_simple_lock()
         for d in self.dependencies:
@@ -234,17 +249,25 @@
         Unlock the file
         """
         if self.has_target_file:
             self._lock.release()
 
     @property
     def accelerators(self):
-        """ Returns the names of the accelerators required to compile the file
         """
-        return self._accelerators
+        Get the names of the accelerators required to compile the file.
+
+        Return a set containing the name of all accelerators required
+        to compile the file. An accelerator is a tool used to add a new
+        capacity to the code. Such an addition requires multiple flags
+        (includes/libs/libdirs/etc) and is therefore specified separately
+        in the compiler configuration file. Examples of 'accelerators' are:
+        openmp, openacc, python.
+        """
+        return self._accelerators.union([da for d in self._dependencies.values() for da in d.accelerators])
 
     def __eq__(self, other):
         return self.module_target == other.module_target
 
     def __hash__(self):
         return hash(self.module_target)
```

### Comparing `pyccel-1.7.3/pyccel/codegen/compiling/compilers.py` & `pyccel-1.7.4/pyccel/codegen/compiling/compilers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/codegen/pipeline.py` & `pyccel-1.7.4/pyccel/codegen/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/ccode.py` & `pyccel-1.7.4/pyccel/codegen/printing/ccode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
-# pylint: disable=missing-function-docstring
 import functools
 from itertools import chain
 import re
 
 from pyccel.ast.basic     import ScopedNode
 
 from pyccel.ast.builtins  import PythonRange, PythonComplex
@@ -340,15 +339,15 @@
         -------
         bool
             True if a C pointer, False otherwise.
         """
         if isinstance(a, (Nil, ObjectAddress)):
             return True
         if isinstance(a, FunctionCall):
-            a = a.funcdef.results[0]
+            a = a.funcdef.results[0].var
 
         if not isinstance(a, Variable):
             return False
         return (a.is_alias and not a.is_ndarray) or a.is_optional or \
                 any(a is bi for b in self._additional_args for bi in b)
 
     #========================== Numpy Elements ===============================#
@@ -455,15 +454,30 @@
         array_init = array_init.format(np_dtype, dummy_array_name,
                     shape_init, strides_init, len(var.shape), 'false')
         array_init += 'stack_array_init(&{})'.format(self._print(var))
         self.add_import(c_imports['ndarrays'])
         return buffer_array, array_init
 
     def _handle_inline_func_call(self, expr):
-        """ Print a function call to an inline function
+        """
+        Print a function call to an inline function.
+
+        Use the arguments passed to an inline function to print
+        its body with the passed arguments in place of the function
+        arguments.
+
+        Parameters
+        ----------
+        expr : FunctionCall
+            The function call which should be printed inline.
+
+        Returns
+        -------
+        str
+            The code for the inline function.
         """
         func = expr.funcdef
         body = func.body
 
         for b in body.body:
             if isinstance(b, ScopedNode):
                 b.scope.update_parent_scope(self.scope, is_loop=True)
@@ -480,15 +494,15 @@
                 args.append(a.value)
 
         new_local_vars = [self.scope.get_temporary_variable(v) \
                             for v in func.local_vars]
 
         parent_assign = expr.get_direct_user_nodes(lambda x: isinstance(x, Assign))
         if parent_assign:
-            results = dict(zip(func.results, parent_assign[0].lhs))
+            results = {r.var : l for r,l in zip(func.results, parent_assign[0].lhs)}
             orig_res_vars = list(results.keys())
             new_res_vars  = self._temporary_args
             new_res_vars = [a.obj if isinstance(a, ObjectAddress) else a for a in new_res_vars]
             self._temporary_args = []
             body.substitute(orig_res_vars, new_res_vars)
 
         # Replace the arguments in the code
@@ -878,18 +892,14 @@
 
     def _print_CStringExpression(self, expr):
         return "".join(self._print(e) for e in expr.get_flat_expression_list())
 
     def _print_CMacro(self, expr):
         return str(expr.macro)
 
-    def extract_function_call_results(self, expr):
-        tmp_list = [self.scope.get_temporary_variable(a.dtype) for a in expr.funcdef.results]
-        return tmp_list
-
     def _print_PythonPrint(self, expr):
         self.add_import(c_imports['stdio'])
         self.add_import(c_imports['inttypes'])
         end = '\n'
         sep = ' '
         code = ''
         empty_end = FunctionCallArgument(LiteralString(''), 'end')
@@ -937,15 +947,15 @@
                 code += self._print(PythonPrint([tuple_start, *args, tuple_end, empty_sep, end_of_tuple]))
                 args = []
                 continue
             if isinstance(f, PythonType):
                 f = f.print_string
 
             if isinstance(f, FunctionCall) and isinstance(f.dtype, NativeTuple):
-                tmp_list = self.extract_function_call_results(f)
+                tmp_list = [self.scope.get_temporary_variable(a.var.dtype) for a in f.funcdef.results]
                 tmp_arg_format_list = []
                 for a in tmp_list:
                     arg_format, arg = self.get_print_format_and_arg(a)
                     tmp_arg_format_list.append(arg_format)
                     args.append(arg)
                 tmp_arg_format_list = CStringExpression(', ').join(tmp_arg_format_list)
                 args_format.append(CStringExpression('(', tmp_arg_format_list, ')'))
@@ -1138,37 +1148,42 @@
             Indicates whether argument names should be printed.
 
         Returns
         -------
         str
             Signature of the function.
         """
-        if len(expr.results) > 1:
-            self._additional_args.append(expr.results)
-        args = list(expr.arguments)
-        if len(expr.results) == 1:
-            ret_type = self.get_declare_type(expr.results[0])
-        elif len(expr.results) > 1:
+        arg_vars = [a.var for a in expr.arguments]
+        result_vars = [r.var for r in expr.results if not r.is_argument]
+
+        n_results = len(result_vars)
+
+        if n_results == 1:
+            ret_type = self.get_declare_type(result_vars[0])
+        elif n_results > 1:
             ret_type = self._print(datatype('int'))
-            args += [FunctionDefArgument(a) for a in expr.results]
+            arg_vars.extend(result_vars)
+            self._additional_args.append(result_vars) # Ensure correct result for is_c_pointer
         else:
             ret_type = self._print(datatype('void'))
+
         name = expr.name
-        if not args:
+        if not arg_vars:
             arg_code = 'void'
         else:
-            def get_var_arg(arg, var):
+            def get_arg_declaration(var):
+                """ Get the code which declares the argument variable.
+                """
                 code = "const " * var.is_const
                 code += self.get_declare_type(var) + ' '
-                code += arg.name * print_arg_names
+                code += var.name * print_arg_names
                 return code
 
-            var_list = [a.var for a in args]
             arg_code_list = [self.function_signature(var, False) if isinstance(var, FunctionAddress)
-                                else get_var_arg(arg, var) for arg, var in zip(args, var_list)]
+                                else get_arg_declaration(var) for var in arg_vars]
             arg_code = ', '.join(arg_code_list)
 
         if self._additional_args :
             self._additional_args.pop()
 
         if isinstance(expr, FunctionAddress):
             return f'{ret_type} (*{name})({arg_code})'
@@ -1593,27 +1608,30 @@
         return ""
 
     def _print_FunctionDef(self, expr):
         if expr.is_inline:
             return ''
         self.set_scope(expr.scope)
 
+        arguments = [a.var for a in expr.arguments]
+        results = [r.var for r in expr.results]
         if len(expr.results) > 1:
-            self._additional_args.append(expr.results)
+            self._additional_args.append(results)
+
         body  = self._print(expr.body)
         decs  = [Declare(i.dtype, i) if isinstance(i, Variable) else FuncAddressDeclare(i) for i in expr.local_vars]
-        if len(expr.results) <= 1 :
-            for i in expr.results:
-                if isinstance(i, Variable) and not i.is_temp:
-                    decs += [Declare(i.dtype, i)]
-                elif not isinstance(i, Variable):
-                    decs += [FuncAddressDeclare(i)]
-        arguments = [a.var for a in expr.arguments]
+
+        if len(results) == 1 :
+            res = results[0]
+            if isinstance(res, Variable) and not res.is_temp:
+                decs += [Declare(res.dtype, res)]
+            elif not isinstance(res, Variable):
+                raise NotImplementedError(f"Can't return {type(res)} from a function")
         decs += [Declare(v.dtype,v) for v in self.scope.variables.values() \
-                if v not in chain(expr.local_vars, expr.results, arguments)]
+                if v not in chain(expr.local_vars, results, arguments)]
         decs  = ''.join(self._print(i) for i in decs)
 
         sep = self._print(SeparatorComment(40))
         if self._additional_args :
             self._additional_args.pop()
         for i in expr.imports:
             self.add_import(i)
```

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/codeprinter.py` & `pyccel-1.7.4/pyccel/codegen/printing/codeprinter.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/cwrappercode.py` & `pyccel-1.7.4/pyccel/codegen/printing/cwrappercode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
-# pylint: disable=no-self-use
 
 from collections import OrderedDict
 
 from pyccel.codegen.printing.ccode import CCodePrinter
 
 from pyccel.ast.bind_c   import as_static_function, wrap_module_array_var, BindCPointer
 
 from pyccel.ast.builtins import PythonTuple, PythonType
 
 from pyccel.ast.core import Assign, AliasAssign, FunctionDef, FunctionAddress
 from pyccel.ast.core import If, IfSection, Return, FunctionCall, Deallocate
 from pyccel.ast.core import SeparatorComment, Allocate
 from pyccel.ast.core import Import, Module, Declare
 from pyccel.ast.core import AugAssign, CodeBlock
+from pyccel.ast.core import FunctionDefArgument, FunctionDefResult
 
 from pyccel.ast.cwrapper    import PyArg_ParseTupleNode, PyBuildValueNode
 from pyccel.ast.cwrapper    import PyArgKeywords
 from pyccel.ast.cwrapper    import Py_None, Py_DECREF
-from pyccel.ast.cwrapper    import generate_datatype_error, PyErr_SetString
+from pyccel.ast.cwrapper    import generate_datatype_error, set_python_error_message
 from pyccel.ast.cwrapper    import scalar_object_check
 from pyccel.ast.cwrapper    import PyccelPyObject
 from pyccel.ast.cwrapper    import C_to_Python, Python_to_C
 from pyccel.ast.cwrapper    import PyModule_AddObject
 
 from pyccel.ast.datatypes import NativeInteger, NativeBool, NativeFloat
 from pyccel.ast.datatypes import datatype, NativeVoid
@@ -292,19 +292,20 @@
             Signature of the function.
         """
         #if target_language is C no need for the binding
         if self._target_language == 'c':
             return self.function_signature(expr)
 
         args = [a.var for a in expr.arguments]
-        if len(expr.results) == 1:
-            ret_type = self.get_declare_type(expr.results[0])
-        elif len(expr.results) > 1:
+        results = [r.var for r in expr.results]
+        if len(results) == 1:
+            ret_type = self.get_declare_type(results[0])
+        elif len(results) > 1:
             ret_type = self._print(datatype('int'))
-            args += [a.clone(name = a.name, memory_handling='alias') for a in expr.results]
+            args += [a.clone(name = a.name, memory_handling='alias') for a in results]
         else:
             ret_type = self._print(datatype('void'))
         name = expr.name
         if not args:
             arg_code = 'void'
         else:
             arg_code = ', '.join(self.function_signature(i, False)
@@ -708,47 +709,49 @@
 
             body = [self._body_scalar(variable, collect_var, default_value, check_type, tmp_variable)]
 
         return body, tmp_variable
 
     def untranslatable_function(self, wrapper_name, wrapper_args, wrapper_results, error_msg):
         """
+        Create code for a function complaining about an object which cannot be wrapped.
+
         Certain functions are not handled in the wrapper (e.g. private),
         This creates a wrapper function which raises NotImplementedError
-        exception and returns NULL
+        exception and returns NULL.
 
         Parameters
         ----------
-        wrapper_name    : string
-            The name of the C wrapper function
+        wrapper_name : str
+            The name of the C wrapper function.
 
-        wrapper_args    : list of Variables
+        wrapper_args : list of Variables
             List of variables with dtype PyObject which hold the arguments
-            passed to the function
+            passed to the function.
 
         wrapper_results : Variable
             List containing one variable with dtype PyObject which represents
-            the variable which will be returned by the function
+            the variable which will be returned by the function.
 
-        error_msg       : string
-            The message to be raised in the NotImplementedError
+        error_msg : str
+            The message to be raised in the NotImplementedError.
 
         Returns
         -------
-        code : string
-            returns the string containing the printed FunctionDef
+        str
+            Returns the string containing the printed FunctionDef.
         """
         current_scope = self.scope
         wrapper_func = FunctionDef(
                 name      = wrapper_name,
-                arguments = wrapper_args,
-                results   = wrapper_results,
+                arguments = [FunctionDefArgument(a) for a in wrapper_args],
+                results   = [FunctionDefResult(r) for r in wrapper_results],
                 body      = [
-                                PyErr_SetString('PyExc_NotImplementedError',
-                                            '"{}"'.format(error_msg)),
+                                set_python_error_message('PyExc_NotImplementedError',
+                                            f'"{error_msg}"'),
                                 AliasAssign(wrapper_results[0], Nil()),
                                 Return(wrapper_results)
                             ],
                 scope     = Scope())
 
         code = CCodePrinter._print_FunctionDef(self, wrapper_func)
         self.set_scope(current_scope)
@@ -847,27 +850,31 @@
         if_expr = If(IfSection(PyccelLt(add_expr,LiteralInteger(0)),
                         [FunctionCall(Py_DECREF, [collect_var]),
                          Return([PyccelUnarySub(LiteralInteger(1))])]))
         return [collect_value, if_expr]
 
     def get_module_exec_function(self, expr, exec_func_name):
         """
+        Create code which initialises a module.
+
         Create the function which executes any statements which happen
-        when the module is loaded
+        when the module is loaded.
 
         Parameters
         ----------
-        expr           : Module
-                         The module being wrapped
+        expr : Module
+            The module being wrapped.
+
         exec_func_name : str
-                         The name of the function
+            The name of the function.
 
-        Result
-        ------
+        Returns
+        -------
         str
+            The code for a function which initialises a module.
         """
         # Create scope for the module initialisation function
         scope = self.scope.new_child_scope(exec_func_name)
         self.set_scope(scope)
 
         #Create module variable
         mod_var_name = self.scope.get_new_name('m')
@@ -940,17 +947,17 @@
             static_function = self.get_static_function(expr.init_func)
             body.insert(0,FunctionCall(static_function,[],[]))
 
         body.append(Return([LiteralInteger(0)]))
         self.exit_scope()
 
         func = FunctionDef(name = exec_func_name,
-            arguments = (mod_var,),
-            results = (scope.get_temporary_variable(NativeInteger(),
-                precision = 4),),
+            arguments = (FunctionDefArgument(mod_var),),
+            results = (FunctionDefResult(scope.get_temporary_variable(NativeInteger(),
+                precision = 4)),),
             body = CodeBlock(body),
             scope = scope)
         func_code = super()._print_FunctionDef(func).split('\n')
         func_code[1] = "static "+func_code[1]
 
 
         return '\n'.join(func_code)
@@ -1016,20 +1023,21 @@
 
             mini_wrapper_func_name = self.scope.get_new_name(func.name + '_mini_wrapper')
             mini_scope = mod_scope.new_child_scope(mini_wrapper_func_name)
             self.set_scope(mini_scope)
 
             # update ndarray local variables properties
             arg_vars = {a.var: a for a in func.arguments}
+            result_vars = [r.var for r in func.results]
             local_arg_vars = {(v.clone(v.name, memory_handling='alias')
                               if isinstance(v, Variable) and v.rank > 0 or v.is_optional \
                               else v) : a for v,a in arg_vars.items()}
             for a in local_arg_vars:
                 mini_scope.insert_variable(a)
-            for r in func.results:
+            for r in result_vars:
                 mini_scope.insert_variable(r)
 
             # Loop for all args in every functions and create the corresponding condition and body
             for idx, (p_arg, (f_var, f_arg)) in enumerate(zip(parse_args, local_arg_vars.items())):
                 collect_var  = self.get_PyArgParseType(f_var)
                 body, tmp_variable = self._body_management(f_var, p_arg, f_arg.value)
 
@@ -1050,19 +1058,19 @@
                 flag_value = argument_type_flags[func][idx]
                 if flag_value >= len(types_dict[f_var]):
                     types_dict[f_var].add((f_var, check, flag_value)) # collect variable type for each arguments
 
                 mini_wrapper_func_body += body
 
             # create the corresponding function call
-            mini_wrapper_func_body.extend(self._get_static_func_call_code(func, static_func_args, func.results))
+            mini_wrapper_func_body.extend(self._get_static_func_call_code(func, static_func_args, result_vars))
 
 
             # Loop for all res in every functions and create the corresponding body and cast
-            for r in func.results :
+            for r in result_vars :
                 collect_var, cast_func = self.get_PyBuildValue(r)
                 if cast_func is not None:
                     mini_wrapper_func_body.append(AliasAssign(collect_var, cast_func))
 
                 res_args.append(ObjectAddress(collect_var) if collect_var.is_alias else collect_var)
 
             # Building PybuildValue and freeing the allocated variable after.
@@ -1075,16 +1083,16 @@
             mini_wrapper_func_body.append(Return(wrapper_results))
             self._to_free_PyObject_list.clear()
 
             self.set_scope(scope)
 
             # Building Mini wrapper function
             mini_wrapper_func_def = FunctionDef(name = mini_wrapper_func_name,
-                arguments = parse_args,
-                results = wrapper_results,
+                arguments = [FunctionDefArgument(a) for a in parse_args],
+                results = [FunctionDefResult(r) for r in wrapper_results],
                 body = mini_wrapper_func_body,
                 scope = mini_scope)
             funcs_def.append(mini_wrapper_func_def)
 
             # append check condition to the functioncall
             body_tmp.append(IfSection(PyccelEq(check_var, LiteralInteger(sum(argument_type_flags[func]))), [AliasAssign(wrapper_results[0],
                     FunctionCall(mini_wrapper_func_def, parse_args))]))
@@ -1093,15 +1101,15 @@
         # Creating check_type function
         check_func_def = self._create_wrapper_check(check_var, parse_args, types_dict, funcs[0].name)
         funcs_def.append(check_func_def)
 
         # Create the wrapper body with collected informations
         body_tmp = [IfSection(PyccelEq(check_var, PyccelUnarySub(LiteralInteger(1))), [Return([Nil()])])] + body_tmp
         body_tmp.append(IfSection(LiteralTrue(),
-            [PyErr_SetString('PyExc_TypeError', '"This combination of arguments is not valid"'),
+            [set_python_error_message('PyExc_TypeError', '"This combination of arguments is not valid"'),
             Return([Nil()])]))
         wrapper_body_translations = [If(*body_tmp)]
 
         # Parsing Arguments
         parse_node = PyArg_ParseTupleNode(*wrapper_args[1:],
                                           funcs[0].arguments,
                                           parse_args, keyword_list)
@@ -1112,16 +1120,16 @@
         #finishing the wrapper body
         wrapper_body.append(Assign(check_var, FunctionCall(check_func_def, parse_args)))
         wrapper_body.extend(wrapper_body_translations)
         wrapper_body.append(Return(wrapper_results)) # Return
 
         # Create FunctionDef
         funcs_def.append(FunctionDef(name = wrapper_name,
-            arguments = wrapper_args,
-            results = wrapper_results,
+            arguments = [FunctionDefArgument(a) for a in wrapper_args],
+            results = [FunctionDefResult(r) for r in wrapper_results],
             body = wrapper_body,
             scope = scope))
 
         sep = self._print(SeparatorComment(40))
 
         self.exit_scope()
 
@@ -1221,30 +1229,30 @@
             types = [elem[0] for elem in arg_type_check_list]
             description = [PythonType(v).print_string for v in types]
             error = ' or '.join([d.python_value for d in description])
             if len(arg_type_check_list) == 1:
                 elem = arg_type_check_list[0]
                 var_name = elem[0].name
                 assert elem[2] == 0
-                body.append(IfSection(PyccelNot(elem[1]), [PyErr_SetString('PyExc_TypeError', f'"{var_name} must be {error}"'), Return([PyccelUnarySub(LiteralInteger(1))])]))
+                body.append(IfSection(PyccelNot(elem[1]), [set_python_error_message('PyExc_TypeError', f'"{var_name} must be {error}"'), Return([PyccelUnarySub(LiteralInteger(1))])]))
             else:
                 arg_type_check_list.sort(key= lambda x : x[2])
                 for elem in arg_type_check_list:
                     var_name = elem[0].name
                     body.append(IfSection(elem[1], [AugAssign(check_var, '+' ,elem[2])]))
-                body.append(IfSection(LiteralTrue(), [PyErr_SetString('PyExc_TypeError', f'"{var_name} must be {error}"'), Return([PyccelUnarySub(LiteralInteger(1))])]))
+                body.append(IfSection(LiteralTrue(), [set_python_error_message('PyExc_TypeError', f'"{var_name} must be {error}"'), Return([PyccelUnarySub(LiteralInteger(1))])]))
             check_func_body += [If(*body)]
 
         check_func_body = [Assign(check_var, LiteralInteger(0))] + check_func_body
         check_func_body.append(Return([check_var]))
         # Creating check function definition
         check_func_name = self.scope.parent_scope.get_new_name(f'type_check_{func_name}')
         check_func_def = FunctionDef(name = check_func_name,
-            arguments = parse_args,
-            results = [check_var],
+            arguments = [FunctionDefArgument(a) for a in parse_args],
+            results = [FunctionDefResult(check_var)],
             body = check_func_body,
             scope = self.scope.new_child_scope(check_func_name))
         return check_func_def
 
     def _print_PyccelPyObject(self, expr):
         return 'pyobject'
 
@@ -1310,15 +1318,15 @@
                     new_v = v.clone(new_name)
                 local_arg_vars[new_v] = a
                 self.scope.insert_variable(new_v)
             else:
                 self.scope.functions[v.name] = v
                 local_arg_vars[v] = a
 
-        result_vars = [v.clone(self.scope.get_new_name(v.name)) for v in expr.results]
+        result_vars = [v.var.clone(self.scope.get_new_name(v.var.name)) for v in expr.results]
         for v in result_vars:
             self.scope.insert_variable(v)
         # update ndarray and optional local variables properties
 
         # Find a name for the wrapper function
         wrapper_name = self._get_wrapper_name(expr)
 
@@ -1397,16 +1405,16 @@
         self._to_free_PyObject_list.clear()
 
         #Return
         wrapper_body.append(Return(wrapper_results))
 
         # Create FunctionDef and write using classic method
         wrapper_func = FunctionDef(name = wrapper_name,
-            arguments = wrapper_args,
-            results = wrapper_results,
+            arguments = [FunctionDefArgument(a) for a in wrapper_args],
+            results = [FunctionDefResult(r) for r in wrapper_results],
             body = wrapper_body,
             scope = self.scope)
 
         self.exit_scope()
 
         return CCodePrinter._print_FunctionDef(self, wrapper_func)
```

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/fcode.py` & `pyccel-1.7.4/pyccel/codegen/printing/fcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
-# pylint: disable=missing-function-docstring
-
 """Print to F90 standard. Trying to follow the information provided at
 www.fortran90.org as much as possible."""
 
 
 import string
 import re
 from itertools import chain
@@ -70,15 +68,15 @@
 from pyccel.ast.numpyext import NumpyRand
 from pyccel.ast.numpyext import NumpyNewArray
 from pyccel.ast.numpyext import NumpyNonZero
 from pyccel.ast.numpyext import NumpySign
 from pyccel.ast.numpyext import Shape
 from pyccel.ast.numpyext import DtypePrecisionToCastFunction
 
-from pyccel.ast.utilities import builtin_import_registery as pyccel_builtin_import_registery
+from pyccel.ast.utilities import builtin_import_registry as pyccel_builtin_import_registry
 from pyccel.ast.utilities import expand_to_loops
 
 from pyccel.errors.errors import Errors
 from pyccel.errors.messages import *
 from pyccel.codegen.printing.codeprinter import CodePrinter
 
 
@@ -395,20 +393,31 @@
                 self.scope.insert_symbol(v.name)
 
         self.set_scope(scope)
         return code
 
     def _get_external_declarations(self):
         """
-        Look for external functions and declare their result type
+        Find external functions and declare their result type.
+
+        Look for any external functions in the local imports from
+        the scope and use their definitions to create declarations
+        from the results. These declarations are stored in a
+        dictionary whose keys are the result variable which will
+        be declared.
+
+        Returns
+        -------
+        dict
+            The declarations necessary to use the external function.
         """
         decs = {}
         for key,f in self.scope.imports['functions'].items():
             if isinstance(f, FunctionDef) and f.is_external:
-                i = Variable(f.results[0].dtype, name=str(key))
+                i = Variable(f.results[0].var.dtype, name=str(key))
                 dec = Declare(i.dtype, i, external=True)
                 decs[i] = dec
 
         return decs
 
     # ============ Elements ============ #
     def _print_PyccelSymbol(self, expr):
@@ -534,15 +543,15 @@
             source = expr.source
         if isinstance(source, DottedName):
             source = source.name[-1]
         else:
             source = self._print(source)
 
         # importing of pyccel extensions is not printed
-        if source in pyccel_builtin_import_registery:
+        if source in pyccel_builtin_import_registry:
             return ''
 
         if expr.source_module:
             source = expr.source_module.scope.get_expected_name(source)
 
         if 'mpi4py' == str(getattr(expr.source,'name',expr.source)):
             return 'use mpi\n' + 'use mpiext\n'
@@ -827,15 +836,15 @@
 
     def _print_Constant(self, expr):
         val = LiteralFloat(expr.value)
         return self._print(val)
 
     def _print_DottedVariable(self, expr):
         if isinstance(expr.lhs, FunctionCall):
-            base = expr.lhs.funcdef.results[0]
+            base = expr.lhs.funcdef.results[0].var
             if (not self._additional_code):
                 self._additional_code = ''
             var_name = self.scope.get_new_name()
             var = base.clone(var_name)
 
             self.scope.insert_variable(var)
 
@@ -1788,36 +1797,39 @@
         return ('{name} : Block\n'
                 '{prelude}\n'
                  '{body}\n'
                 'end Block {name}\n').format(name=expr.name, prelude=prelude, body=body_code)
 
     def _print_BindCFunctionDef(self, expr):
         name = self._print(expr.name)
-        results   = list(expr.results)
-        arguments = [a.var for a in expr.arguments]
-        if any(isinstance(a, FunctionAddress) for a in arguments):
-            # Functions with function addresses as arguments cannot be
-            # exposed to python so there is no need to print their signature
-            return ''
+        results = [r.var for r in expr.results]
 
         self.set_scope(expr.scope)
         self.scope.functions[expr.name] = expr
 
         body = self._print(expr.body)
 
-        arguments_inout = expr.arguments_inout
         decs = OrderedDict()
-        for i,arg in enumerate(arguments):
-            if arguments_inout[i]:
+        for arg in expr.arguments:
+            if arg.inout:
                 intent='inout'
             else:
                 intent='in'
 
-            dec = Declare(arg.dtype, arg, intent=intent , static=True)
-            decs[arg] = dec
+            arg_var = arg.var
+
+            if isinstance(arg_var, FunctionAddress):
+                # Functions with function addresses as arguments cannot be
+                # exposed to python so there is no need to print their signature
+                return ''
+
+            dec = Declare(arg_var.dtype, arg_var, intent=intent , static=True)
+            decs[arg_var] = dec
+
+        arguments = [a.var for a in expr.arguments]
 
         for result in results:
             dec = Declare(result.dtype, result, intent='out', static=True)
             decs[result] = dec
 
         decs.update(self._get_external_declarations())
 
@@ -1859,60 +1871,76 @@
                  'end {} {}\n'.format(func_type, name)]
         return '\n'.join(p for p in parts if p)
 
     def _print_FunctionAddress(self, expr):
         return expr.name
 
     def function_signature(self, expr, name):
+        """
+        Get the different parts of the signature of the function `expr`.
+
+        A helper function to print just the signature of the function
+        including the declarations of the arguments and results.
+
+        Parameters
+        ----------
+        expr : FunctionDef
+            The function whose signature should be printed.
+        name : str
+            The name which should be printed as the name of the function.
+            (May be different from expr.name in the case of interfaces).
+
+        Returns
+        -------
+        dict
+            A dictionary with the keys :
+                sig - The declaration of the function/subroutine with any necessary keywords.
+                arg_code - A string containing a list of the arguments.
+                func_end - Any code to be added to the signature after the arguments (ie result).
+                arg_decs - The code necessary to declare the arguments of the function/subroutine.
+                func_type - Subroutine or function.
+        """
         is_pure      = expr.is_pure
         is_elemental = expr.is_elemental
-        out_args = []
+        out_args = [r.var for r in expr.results if not r.is_argument]
         args_decs = OrderedDict()
-        arguments = [a.var for a in expr.arguments]
+        arguments = expr.arguments
+        argument_vars = [a.var for a in arguments]
 
         func_end  = ''
         rec = 'recursive ' if expr.is_recursive else ''
-        if len(expr.results) != 1 or expr.results[0].rank > 0:
+        if len(out_args) != 1 or out_args[0].rank > 0:
             func_type = 'subroutine'
-            out_args = list(expr.results)
             for result in out_args:
-                if result in arguments:
-                    dec = Declare(result.dtype, result, intent='inout')
-                else:
-                    dec = Declare(result.dtype, result, intent='out')
-                args_decs[result] = dec
+                args_decs[result] = Declare(result.dtype, result, intent='out')
 
             functions = expr.functions
 
         else:
            #todo: if return is a function
             func_type = 'function'
-            result = expr.results[0]
+            result = out_args[0]
             functions = expr.functions
 
             func_end = 'result({0})'.format(result.name)
 
-            dec = Declare(result.dtype, result)
-            args_decs[result] = dec
+            args_decs[result] = Declare(result.dtype, result)
+            out_args = []
         # ...
 
-        for i,arg in enumerate(arguments):
-            if isinstance(arg, Variable):
+        for i, arg in enumerate(arguments):
+            arg_var = arg.var
+            if isinstance(arg_var, Variable):
                 if i == 0 and expr.cls_name:
-                    dec = Declare(arg.dtype, arg, intent='inout', passed_from_dotted = True)
-                elif expr.arguments_inout[i]:
-                    dec = Declare(arg.dtype, arg, intent='inout')
+                    dec = Declare(arg_var.dtype, arg_var, intent='inout', passed_from_dotted = True)
+                elif arg.inout:
+                    dec = Declare(arg_var.dtype, arg_var, intent='inout')
                 else:
-                    dec = Declare(arg.dtype, arg, intent='in')
-                args_decs[arg] = dec
-
-        #remove parametres intent(inout) from out_args to prevent repetition
-        for i in arguments:
-            if i in out_args:
-                out_args.remove(i)
+                    dec = Declare(arg_var.dtype, arg_var, intent='in')
+                args_decs[arg_var] = dec
 
         # treat case of pure function
         sig = '{0}{1} {2}'.format(rec, func_type, name)
         if is_pure:
             sig = 'pure {}'.format(sig)
 
         # treat case of elemental function
@@ -1964,17 +1992,18 @@
         for i in expr.local_vars:
             dec = Declare(i.dtype, i)
             decs[i] = dec
 
         decs.update(self._get_external_declarations())
 
         arguments = [a.var for a in expr.arguments]
+        results = [a.var for a in expr.results]
         vars_to_print = self.scope.variables.values()
         for v in vars_to_print:
-            if (v not in expr.local_vars) and (v not in expr.results) and (v not in arguments):
+            if (v not in expr.local_vars) and (v not in results) and (v not in arguments):
                 decs[v] = Declare(v.dtype,v)
         prelude += ''.join(self._print(i) for i in decs.values())
         if len(functions)>0:
             functions_code = '\n'.join(self._print(i) for  i in functions)
             body_code = body_code +'\ncontains\n' + functions_code
 
         imports = ''.join(self._print(i) for i in expr.imports)
@@ -2949,15 +2978,15 @@
 #=======================================================================================
 
     def _print_FunctionCall(self, expr):
         func = expr.funcdef
 
         f_name = self._print(expr.func_name if not expr.interface else expr.interface_name)
         args   = expr.args
-        func_results  = func.results
+        func_results  = [r.var for r in func.results]
         parent_assign = expr.get_direct_user_nodes(lambda x: isinstance(x, Assign))
         is_function =  len(func_results) == 1 and func_results[0].rank == 0
 
         if (not self._additional_code):
             self._additional_code = ''
         if parent_assign:
             lhs = parent_assign[0].lhs
@@ -3028,15 +3057,15 @@
         else:
             return code
 
 #=======================================================================================
 
     def _print_DottedFunctionCall(self, expr):
         if isinstance(expr.prefix, FunctionCall):
-            base = expr.prefix.funcdef.results[0]
+            base = expr.prefix.funcdef.results[0].var
             if (not self._additional_code):
                 self._additional_code = ''
             var_name = self.scope.get_new_name()
             var = base.clone(var_name)
 
             self.scope.insert_variable(var)
```

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/luacode.py` & `pyccel-1.7.4/pyccel/codegen/printing/luacode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
-# pylint: disable=missing-function-docstring
-
 """
 Lua code printer
 
 The `LuaCodePrinter` converts SymPy expressions into Lua expressions.
 
 A complete code generator, which uses `lua_code` extensively, can be found
 in `sympy.utilities.codegen`. The `codegen` module can be used to generate
```

### Comparing `pyccel-1.7.3/pyccel/codegen/printing/pycode.py` & `pyccel-1.7.4/pyccel/codegen/printing/pycode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
-# pylint: disable=missing-function-docstring
 
 from pyccel.decorators import __all__ as pyccel_decorators
 
 from pyccel.ast.builtins   import PythonMin, PythonMax
 from pyccel.ast.core       import CodeBlock, Import, Assign, FunctionCall, For, AsName, FunctionAddress
 from pyccel.ast.core       import IfSection, FunctionDef, Module
 from pyccel.ast.datatypes  import default_precision
 from pyccel.ast.functionalexpr import FunctionalFor
 from pyccel.ast.literals   import LiteralTrue, LiteralString
 from pyccel.ast.literals   import LiteralInteger, LiteralFloat, LiteralComplex
 from pyccel.ast.numpyext   import Shape as NumpyShape, numpy_target_swap
 from pyccel.ast.numpyext   import NumpyArray, NumpyNonZero
 from pyccel.ast.numpyext   import DtypePrecisionToCastFunction
 from pyccel.ast.variable   import DottedName, HomogeneousTupleVariable, Variable
-from pyccel.ast.utilities  import builtin_import_registery as pyccel_builtin_import_registery
+from pyccel.ast.utilities  import builtin_import_registry as pyccel_builtin_import_registry
 from pyccel.ast.utilities  import decorators_mod
 
 from pyccel.codegen.printing.codeprinter import CodePrinter
 
 from pyccel.errors.errors import Errors
 from pyccel.errors.messages import PYCCEL_RESTRICTION_TODO
 
@@ -50,15 +49,26 @@
         'numpy.random' : {'random' : 'rand'}
         }
 import_source_swap = {
         'omp_lib' : 'pyccel.stdlib.internal.openmp'
         }
 
 class PythonCodePrinter(CodePrinter):
-    """A printer to convert pyccel expressions to strings of Python code"""
+    """
+    A printer for printing code in Python.
+
+    A printer to convert Pyccel's AST to strings of Python code.
+    As for all printers the navigation of this file is done via _print_X
+    functions.
+
+    Parameters
+    ----------
+    filename : str
+        The name of the file being pyccelised.
+    """
     printmethod = "_pycode"
     language = "python"
 
     _default_settings = {
         'tabwidth': 4,
     }
 
@@ -162,21 +172,28 @@
     def _print_NativeComplex(self, expr):
         return 'complex'
 
     def _print_Variable(self, expr):
         return self._print(expr.name)
 
     def _print_FunctionDefArgument(self, expr):
+        name = self._print(expr.name)
+        type_annotation = ''
+        default = ''
+
+        if expr.annotation:
+            type_annotation = f' : {expr.annotation}'
+
         if expr.has_default:
             if isinstance(expr.value, FunctionDef):
-                return '{} = {}'.format(self._print(expr.name), self._print(expr.value.name))
+                default = f' = {self._print(expr.value.name)}'
             else:
-                return '{} = {}'.format(self._print(expr.name), self._print(expr.value))
-        else:
-            return self._print(expr.name)
+                default = f' = {self._print(expr.value)}'
+
+        return f'{name}{type_annotation}{default}'
 
     def _print_FunctionCallArgument(self, expr):
         if expr.keyword:
             return '{} = {}'.format(expr.keyword, self._print(expr.value))
         else:
             return self._print(expr.value)
 
@@ -479,16 +496,16 @@
                 # If the source contains multiple names which reference the same object
                 # check if the target is referred to by another name in pyccel.
                 # Print the name used by pyccel (either the value from import_target_swap
                 # or the original name from the import
                 target = [AsName(i.object, import_target_swap[source].get(i.target,i.target)) for i in target]
 
             target = list(set(target))
-            if source in pyccel_builtin_import_registery:
-                self._aliases.update([(pyccel_builtin_import_registery[source][t.name].cls_name, t.target) for t in target if t.name != t.target])
+            if source in pyccel_builtin_import_registry:
+                self._aliases.update([(pyccel_builtin_import_registry[source][t.name].cls_name, t.target) for t in target if t.name != t.target])
 
             if expr.source_module:
                 if expr.source_module.init_func:
                     self._ignore_funcs.append(expr.source_module.init_func)
                 if expr.source_module.free_func:
                     self._ignore_funcs.append(expr.source_module.free_func)
             target = [self._print(t) for t in target if t.name not in (init_func_name, free_func_name)]
```

### Comparing `pyccel-1.7.3/pyccel/codegen/python_wrapper.py` & `pyccel-1.7.4/pyccel/codegen/python_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
     # get the include folder path and library files
     recompile_object(cwrapper_lib,
                       compiler = wrapper_compiler,
                       verbose  = verbose)
 
     wrapper_compile_obj.add_dependencies(cwrapper_lib)
-    extra_includes  = ['cwrapper']
 
     #---------------------------------------
     #      Print code specific cwrapper
     #---------------------------------------
     module_old_name = codegen.ast.name
     codegen.ast.set_name(sharedlib_modname)
     wrapper_codegen = CWrapperCodePrinter(codegen.parser.filename, language)
@@ -123,15 +122,14 @@
             stdlib.reset_folder(lib_dest_path) # pylint: disable=E1101
             # get the include folder path and library files
             recompile_object(stdlib,
                               compiler = wrapper_compiler,
                               verbose  = verbose)
 
             wrapper_compile_obj.add_dependencies(stdlib)
-        extra_includes.append('cwrapper_ndarrays')
 
     #---------------------------------------
     #         Compile code
     #---------------------------------------
     wrapper_compiler.compile_module(wrapper_compile_obj,
                                 output_folder = pyccel_dirpath,
                                 verbose = verbose)
```

### Comparing `pyccel-1.7.3/pyccel/codegen/utilities.py` & `pyccel-1.7.4/pyccel/codegen/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/commands/console.py` & `pyccel-1.7.4/pyccel/commands/console.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/commands/pyccel_clean.py` & `pyccel-1.7.4/pyccel/commands/pyccel_clean.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/commands/pyccel_init.py` & `pyccel-1.7.4/pyccel/commands/pyccel_init.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/compilers/default_compilers.py` & `pyccel-1.7.4/pyccel/compilers/default_compilers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Module responsible for the creation of the json files containing the default configuration for each available compiler.
 This module only needs to be imported once. Once the json files have been generated they can be used directly thus
 avoiding the need for a large number of imports
 """
+import glob
 import os
 import sys
 import sysconfig
 from numpy import get_include as get_numpy_include
 from pyccel import __version__ as pyccel_version
 
 gfort_info = {'exec' : 'gfortran',
@@ -171,22 +172,39 @@
                 },
             'family': 'nvidia',
             }
 
 #------------------------------------------------------------
 def change_to_lib_flag(lib):
     """
-    Convert a library to a library flag
+    Convert a library to a library flag.
+
+    Take a library file and return the associated library
+    flag by stripping the library suffix. If the file does
+    not begin with the expected 'lib' prefix then it is returned
+    unchanged.
+
+    Parameters
+    ----------
+    lib : str
+        The library file.
+
+    Returns
+    -------
+    str
+        The library flag.
     """
     if lib.startswith('lib'):
         end = len(lib)
         if lib.endswith('.a'):
             end = end-2
         if lib.endswith('.so'):
             end = end-3
+        if lib.endswith('.dylib'):
+            end = end-5
         return '-l{}'.format(lib[3:end])
     else:
         return lib
 
 config_vars = sysconfig.get_config_vars()
 
 python_info = {
@@ -196,41 +214,58 @@
                 + config_vars.get("CC","").split()[1:],
             'includes' : [*config_vars.get("INCLUDEPY","").split(), get_numpy_include()],
             "shared_suffix" : config_vars['EXT_SUFFIX'],
             }
         }
 
 if sys.platform == "win32":
-    python_lib = os.path.join(config_vars["prefix"], 'python{}.dll'.format(config_vars["VERSION"]))
-    if os.path.exists(python_lib):
-        python_info['python']['dependencies'] = (python_lib,)
+    expected_dir = config_vars["prefix"]
+    version = config_vars["VERSION"]
+    python_libs = glob.glob(f"{expected_dir}/python{version}.dll")
+    if python_libs:
+        python_info['python']['dependencies'] = tuple(python_libs)
     else:
-        python_info['python']['libs'] = ('python{}'.format(config_vars["VERSION"]),)
+        python_info['python']['libs'] = (f'python{version}',)
         python_info['python']['libdirs'] = config_vars.get("installed_base","").split()
 
 else:
     # Collect library according to python config file
-    python_lib_base = os.path.join(config_vars["prefix"], "lib", config_vars["LDLIBRARY"])
+    expected_dir = config_vars["LIBDIR"]
+    version = config_vars["VERSION"]
+    python_shared_libs = glob.glob(f"{expected_dir}/libpython{version}*")
 
     # Collect a list of all possible libraries matching the name in the configs
     # which can be found on the system
-    possible_shared_lib = python_lib_base.replace('.a','.so')
-    possible_shared_lib = possible_shared_lib if os.path.exists(possible_shared_lib) else ''
-    possible_static_lib = python_lib_base.replace('.so','.a')
-    possible_static_lib = possible_static_lib if os.path.exists(possible_static_lib) else ''
-    # Prefer the static library where possible to avoid unnecessary libdirs
-    # which may lead to the wrong libraries being linked
-    if possible_static_lib != '':
-        python_info['python']['dependencies'] = (possible_static_lib,)
+    shared_ending = '.dylib' if sys.platform == "darwin" else '.so'
+    possible_shared_lib = [l for l in python_shared_libs if shared_ending in l]
+    possible_static_lib = [l for l in python_shared_libs if '.a' in l]
+
+    # Prefer saving the library as a dependency where possible to avoid
+    # unnecessary libdirs which may lead to the wrong versions being linked
+    # for other libraries
+    # Prefer a shared library as it requires less memory
+    if possible_shared_lib:
+        if len(possible_shared_lib)>1:
+            preferred_lib = [l for l in possible_shared_lib if l.endswith(shared_ending)]
+            if preferred_lib:
+                possible_shared_lib = preferred_lib
+
+        python_info['python']['dependencies'] = (possible_shared_lib[0],)
+    elif possible_static_lib:
+        if len(possible_static_lib)>1:
+            preferred_lib = [l for l in possible_static_lib if l.endswith('.a')]
+            if preferred_lib:
+                possible_static_lib = preferred_lib
+        python_info['python']['dependencies'] = (possible_static_lib[0],)
     else:
         # If the proposed library does not exist use different config flags
         # to specify the library
         linker_flags = [change_to_lib_flag(l) for l in
-                        config_vars.get("LIBRARY","").split() + \
-                        config_vars.get("LDSHARED","").split()[1:]]
+                        config_vars.get("LDSHARED","").split() + \
+                        config_vars.get("LIBRARY","").split()[1:]]
         python_info['python']['libs'] = [l[2:] for l in linker_flags if l.startswith('-l')]
         python_info['python']['libdirs'] = [l[2:] for l in linker_flags if l.startswith('-L')] + \
                             config_vars.get("LIBPL","").split()+config_vars.get("LIBDIR","").split()
 
 #------------------------------------------------------------
 gcc_info.update(python_info)
 gfort_info.update(python_info)
```

### Comparing `pyccel-1.7.3/pyccel/complexity/arithmetic.py` & `pyccel-1.7.4/pyccel/complexity/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/complexity/basic.py` & `pyccel-1.7.4/pyccel/complexity/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/complexity/memory.py` & `pyccel-1.7.4/pyccel/complexity/memory.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/decorators.py` & `pyccel-1.7.4/pyccel/decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/epyccel.py` & `pyccel-1.7.4/pyccel/epyccel.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/errors/errors.py` & `pyccel-1.7.4/pyccel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/errors/messages.py` & `pyccel-1.7.4/pyccel/errors/messages.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/naming/__init__.py` & `pyccel-1.7.4/pyccel/naming/__init__.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/naming/cnameclashchecker.py` & `pyccel-1.7.4/pyccel/naming/cnameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/naming/fortrannameclashchecker.py` & `pyccel-1.7.4/pyccel/naming/fortrannameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/naming/pythonnameclashchecker.py` & `pyccel-1.7.4/pyccel/naming/pythonnameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/base.py` & `pyccel-1.7.4/pyccel/parser/base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/extend_tree.py` & `pyccel-1.7.4/pyccel/parser/extend_tree.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/grammar/headers.tx` & `pyccel-1.7.4/pyccel/parser/grammar/headers.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/grammar/openacc.tx` & `pyccel-1.7.4/pyccel/parser/grammar/openacc.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/grammar/openmp.tx` & `pyccel-1.7.4/pyccel/parser/grammar/openmp.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/grammar/pyccel.tx` & `pyccel-1.7.4/pyccel/parser/grammar/pyccel.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/parser.py` & `pyccel-1.7.4/pyccel/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/scope.py` & `pyccel-1.7.4/pyccel/parser/scope.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/semantic.py` & `pyccel-1.7.4/pyccel/parser/semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """ File containing SemanticParser. This class handles the semantic stage of the translation.
 See the developer docs for more details
 """
 
-# pylint: disable=missing-function-docstring
-
 from itertools import chain
 
 from sympy.utilities.iterables import iterable as sympy_iterable
 
 from sympy import Sum as Summation
 from sympy import Symbol as sp_Symbol
 from sympy import Integer as sp_Integer
@@ -31,15 +29,15 @@
                                  PythonTuple, Lambda)
 
 from pyccel.ast.core import Comment, CommentBlock, Pass
 from pyccel.ast.core import If, IfSection
 from pyccel.ast.core import Allocate, Deallocate
 from pyccel.ast.core import Assign, AliasAssign, SymbolicAssign
 from pyccel.ast.core import AugAssign, CodeBlock
-from pyccel.ast.core import Return, FunctionDefArgument
+from pyccel.ast.core import Return, FunctionDefArgument, FunctionDefResult
 from pyccel.ast.core import ConstructorCall, InlineFunctionDef
 from pyccel.ast.core import FunctionDef, Interface, FunctionAddress, FunctionCall, FunctionCallArgument
 from pyccel.ast.core import DottedFunctionCall
 from pyccel.ast.core import ClassDef
 from pyccel.ast.core import For
 from pyccel.ast.core import Module
 from pyccel.ast.core import While
@@ -102,15 +100,15 @@
 from pyccel.ast.operators import PyccelNot, PyccelEq, PyccelAdd, PyccelMul, PyccelPow
 from pyccel.ast.operators import PyccelAssociativeParenthesis, PyccelDiv
 
 from pyccel.ast.sympy_helper import sympy_to_pyccel, pyccel_to_sympy
 
 from pyccel.ast.utilities import builtin_function as pyccel_builtin_function
 from pyccel.ast.utilities import builtin_import as pyccel_builtin_import
-from pyccel.ast.utilities import builtin_import_registery as pyccel_builtin_import_registery
+from pyccel.ast.utilities import builtin_import_registry as pyccel_builtin_import_registry
 from pyccel.ast.utilities import split_positional_keyword_arguments
 from pyccel.ast.utilities import recognised_source
 
 from pyccel.ast.variable import Constant
 from pyccel.ast.variable import Variable
 from pyccel.ast.variable import TupleVariable, HomogeneousTupleVariable, InhomogeneousTupleVariable
 from pyccel.ast.variable import IndexedElement
@@ -166,24 +164,44 @@
     msg = f'Name of Object : {name} cannot be determined'
     return errors.report(PYCCEL_RESTRICTION_TODO+'\n'+msg, symbol=var,
                 severity='fatal')
 
 #==============================================================================
 
 class SemanticParser(BasicParser):
+    """
+    Class which handles the semantic stage as described in the developer docs.
 
-    """ Class for a Semantic Parser.
-    It takes a syntactic parser as input for the moment"""
+    This class is described in detail in developer_docs/semantic_stage.md.
+    It determines all semantic information which must be deduced in order to
+    print a representation of the AST resulting from the syntactic stage in one
+    of the target languages.
+
+    Parameters
+    ----------
+    inputs : SyntaxParser
+        A syntactic parser which has been used to generate a representation of
+        the input code using Pyccel nodes.
+
+    parents : list
+        A list of parsers describing the files which import this file.
+
+    d_parsers : list
+        A list of parsers describing files imported by this file.
+
+    **kwargs : dict
+        Additional keyword arguments for BasicParser.
+    """
 
-    def __init__(self, inputs, **kwargs):
+    def __init__(self, inputs, *, parents = (), d_parsers = (), **kwargs):
 
         # a Parser can have parents, who are importing it.
         # imports are then its sons.
-        self._parents = kwargs.pop('parents', [])
-        self._d_parsers = kwargs.pop('d_parsers', {})
+        self._parents = list(parents)
+        self._d_parsers = dict(d_parsers)
 
         # ...
         if not isinstance(inputs, SyntaxParser):
             raise TypeError('> Expecting a syntactic parser as input')
 
         parser = inputs
         # ...
@@ -230,14 +248,26 @@
     def d_parsers(self):
         """Returns the d_parsers parser."""
 
         return self._d_parsers
 
     @property
     def program_namespace(self):
+        """
+        Get the namespace relevant to the program.
+
+        Get the namespace which describes the section of
+        code which is executed as a program. In other words
+        the code inside an `if __name__ == '__main__':`
+        block.
+
+        Returns
+        -------
+        Scope : The program namespace.
+        """
         return self._program_namespace
 
     #================================================================
     #                     Public functions
     #================================================================
 
     def annotate(self, **settings):
@@ -271,19 +301,34 @@
         return ast
 
     #================================================================
     #              Utility functions for scope handling
     #================================================================
 
     def change_to_program_scope(self):
+        """
+        Switch the focus to the program scope.
+
+        Update the namespace variable so that it points at the
+        program namespace (which describes the scope inside
+        a `if __name__ == '__main__':` block). It is assumed that
+        the current namespace is the module namespace.
+        """
         self._allocs.append([])
         self._module_namespace = self.scope
         self.scope = self._program_namespace
 
     def change_to_module_scope(self):
+        """
+        Switch the focus to the module scope.
+
+        Update the namespace variable so that it points
+        at the module namespace. It is assumed that the
+        current namespace is the program namespace.
+        """
         self._program_namespace = self.scope
         self.scope = self._module_namespace
 
     def check_for_variable(self, name):
         """
         Search for a Variable object with the given name in the current scope,
         defined by the local and global Python scopes. Return None if not found.
@@ -311,14 +356,29 @@
                 errors.report(UNDEFINED_VARIABLE, symbol=name,
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='fatal')
 
         return var
 
     def get_variables(self, container):
+        """
+        Get all variables in the scope of interest.
+
+        Get a list of all variables which are
+
+        Parameters
+        ----------
+        container : Scope
+            The object describing the relevant scope.
+
+        Returns
+        -------
+        list
+            A list of variables.
+        """
         # this only works if called on a function scope
         # TODO needs more tests when we have nested functions
         variables = []
         variables.extend(container.variables.values())
         for sub_container in container.loops:
             variables.extend(self.get_variables(sub_container))
         return variables
@@ -690,25 +750,42 @@
                     severity='fatal')
             if isinstance(val, TupleVariable):
                 return PythonTuple(*(val.get_vars()*length))
             else:
                 return PythonTuple(*(val.args*length))
 
     def _handle_function_args(self, arguments, **settings):
+        """
+        Get a list of all function arguments.
+
+        Get a list of all the function arguments which are passed
+        to a function. This is done by visiting the syntactic
+        FunctionCallArguments. If this argument contains a
+        starred arguments object then the contents of this object
+        are extracted into the final list.
+
+        Parameters
+        ----------
+        arguments : list of FunctionCallArgument
+            The arguments which were passed to the function.
+
+        **settings : dict
+            Any settings to be passed to the `_visit` function.
+
+        Returns
+        -------
+        list of FunctionCallArgument
+            The arguments passed to the function.
+        """
         args  = []
         for arg in arguments:
             a = self._visit(arg, **settings)
             if isinstance(a.value, StarredArguments):
                 args.extend([FunctionCallArgument(av) for av in a.value.args_var])
             else:
-                if isinstance(a.value, PyccelArithmeticOperator) and a.value.rank:
-                    tmp_var = PyccelSymbol(self.scope.get_new_name(), is_temp=True)
-                    assign = self._visit(Assign(tmp_var, arg.value, fst= arg.value.fst))
-                    self._additional_exprs[-1].append(assign)
-                    a = FunctionCallArgument(self._visit(tmp_var))
                 args.append(a)
         return args
 
     def get_type_description(self, var, include_rank = True):
         """
         Provides a text description of the type of a variable
         (useful for error messages)
@@ -774,29 +851,37 @@
             if f_arg.rank > 1 and i_arg.order != f_arg.order:
                 errors.report(INCOMPATIBLE_ORDERING.format(idx=idx+1, arg=i_arg, func=expr.func_name, order=f_arg.order),
                         symbol = expr,
                         severity='error')
 
     def _handle_function(self, expr, func, args, **settings):
         """
+        Create the node representing the function call.
+
         Create a FunctionCall or an instance of a PyccelInternalFunction
-        from the function information and arguments
+        from the function information and arguments.
 
         Parameters
-        ==========
+        ----------
         expr : PyccelAstNode
-               The expression where this call is found (used for error output)
+               The expression where this call is found (used for error output).
+
         func : FunctionDef instance, Interface instance or PyccelInternalFunction type
-               The function being called
+               The function being called.
+
         args : tuple
-               The arguments passed to the function
+               The arguments passed to the function.
+
+        **settings : dict
+            The settings passed to _visit functions.
 
         Returns
-        =======
-        new_expr : FunctionCall or PyccelInternalFunction
+        -------
+        FunctionCall/PyccelInternalFunction
+            The semantic representation of the call.
         """
         if isinstance(func, PyccelFunctionDef):
             func = func.cls_name
             args, kwargs = split_positional_keyword_arguments(*args)
 
             try:
                 new_expr = func(*args, **kwargs)
@@ -804,19 +889,19 @@
                 errors.report(UNRECOGNISED_FUNCTION_CALL,
                         symbol = expr,
                         severity = 'fatal')
 
             return new_expr
         else:
             if self._current_function == func.name:
-                if len(func.results)>0 and not isinstance(func.results[0], PyccelAstNode):
+                if len(func.results)>0 and not isinstance(func.results[0].var, PyccelAstNode):
                     errors.report(RECURSIVE_RESULTS_REQUIRED, symbol=func, severity="fatal")
 
             parent_assign = expr.get_direct_user_nodes(lambda x: isinstance(x, Assign))
-            if not parent_assign and len(func.results) == 1 and func.results[0].rank > 0:
+            if not parent_assign and len(func.results) == 1 and func.results[0].var.rank > 0:
                 tmp_var = PyccelSymbol(self.scope.get_new_name())
                 assign = Assign(tmp_var, expr)
                 assign.set_fst(expr.fst)
                 self._additional_exprs[-1].append(self._visit(assign))
                 return self._visit(tmp_var)
 
             if isinstance(func, FunctionDef) and len(args) > len(func.arguments):
@@ -848,49 +933,56 @@
             elif isinstance(func, FunctionDef):
                 self._check_argument_compatibility(args, func_args,
                             expr, func.is_elemental)
             return new_expr
 
     def _create_variable(self, name, dtype, rhs, d_lhs, arr_in_multirets=False):
         """
+        Create a new variable.
+
         Create a new variable. In most cases this is just a call to
-        Variable.__init__
+        `Variable.__init__`
         but in the case of a tuple variable it is a recursive call to
         create all elements in the tuple.
         This is done separately to _assign_lhs_variable to ensure that
-        elements of a tuple do not exist in the scope
+        elements of a tuple do not exist in the scope.
 
         Parameters
         ----------
         name : str
-            The name of the new variable
+            The name of the new variable.
 
         dtype : DataType
-            The data type of the new variable
+            The data type of the new variable.
 
         rhs : Variable
             The value assigned to the lhs. This is required to call
-            self._infer_type recursively for tuples
+            self._infer_type recursively for tuples.
 
-        arr_in_multirets : bool
+        d_lhs : dict
+            Dictionary of properties for the new Variable.
+
+        arr_in_multirets : bool, default: False
             If True, the variable that will be created is an array
             in multi-values return, false otherwise.
 
-        d_lhs : dict
-            Dictionary of properties for the new Variable
+        Returns
+        -------
+        Variable
+            The variable that has been created.
         """
         if isinstance(name, PyccelSymbol):
             is_temp = name.is_temp
         else:
             is_temp = False
 
         if isinstance(rhs, (PythonTuple, InhomogeneousTupleVariable, NumpyNonZero)) or \
                 (isinstance(rhs, FunctionCall) and len(rhs.funcdef.results)>1):
             if isinstance(rhs, FunctionCall):
-                iterable = rhs.funcdef.results
+                iterable = [r.var for r in rhs.funcdef.results]
             else:
                 iterable = rhs
             elem_vars = []
             is_homogeneous = True
             elem_d_lhs_ref = None
             for i,r in enumerate(iterable):
                 elem_name = self.scope.get_new_name( name + '_' + str(i) )
@@ -1662,15 +1754,21 @@
             errors.report(PYCCEL_RESTRICTION_INHOMOG_LIST, symbol=expr,
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                 severity='fatal')
         return expr
 
     def _visit_FunctionCallArgument(self, expr, **settings):
         value = self._visit(expr.value, **settings)
-        return FunctionCallArgument(value, expr.keyword)
+        a = FunctionCallArgument(value, expr.keyword)
+        if isinstance(a.value, PyccelArithmeticOperator) and a.value.rank:
+            tmp_var = self.scope.get_new_name()
+            assign = self._visit(Assign(tmp_var, expr.value, fst = expr.value.fst))
+            self._additional_exprs[-1].append(assign)
+            a = FunctionCallArgument(self._visit(tmp_var))
+        return a
 
     def _visit_FunctionDefArgument(self, expr, **settings):
         var   = self._visit(expr.var, **settings)
         value = self._visit(expr.value, **settings)
         return FunctionDefArgument(var, value=value,
                 annotation=expr.annotation,
                 kwonly=expr.is_kwonly)
@@ -1850,15 +1948,15 @@
         if isinstance(visited_lhs, FunctionCall):
             results = visited_lhs.funcdef.results
             if len(results) != 1:
                 errors.report("Cannot get attribute of function call with multiple returns",
                         symbol=expr,
                         bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                         severity='fatal')
-            first = results[0]
+            first = results[0].var
         rhs_name = _get_name(rhs)
         attr_name = []
 
         # Handle case of imported module
         if isinstance(first, Module):
 
             if rhs_name in first:
@@ -2322,15 +2420,15 @@
             else:
                 master = macro.master
                 if isinstance(macro, MacroVariable):
                     rhs = master
                 else:
                     # If macro is function, create left-hand side variable
                     if isinstance(master, FunctionDef) and master.results:
-                        d_var = self._infer_type(master.results[0], **settings)
+                        d_var = self._infer_type(master.results[0].var, **settings)
                         dtype = d_var.pop('datatype')
                         lhs = Variable(dtype, lhs.name, **d_var, is_temp=lhs.is_temp)
                         var = self.check_for_variable(lhs.name)
                         if var is None:
                             self.scope.insert_variable(lhs)
 
                     name = macro.name
@@ -2395,17 +2493,17 @@
 
         elif isinstance(rhs, FunctionCall):
             func = rhs.funcdef
             if isinstance(func, FunctionDef):
                 results = func.results
                 if results:
                     if len(results)==1:
-                        d_var = self._infer_type(results[0], **settings)
+                        d_var = self._infer_type(results[0].var, **settings)
                     else:
-                        d_var = self._infer_type(PythonTuple(*results), **settings)
+                        d_var = self._infer_type(PythonTuple(*[r.var for r in results]), **settings)
                 elif expr.lhs.is_temp:
                     return rhs
                 else:
                     raise NotImplementedError("Cannot assign result of a function without a return")
 
                 # case of elemental function
                 # if the input and args of func do not have the same shape,
@@ -2424,15 +2522,15 @@
                         arg = call_args[0].value
                         d_var['shape'          ] = arg.shape
                         d_var['rank'           ] = arg.rank
                         d_var['memory_handling'] = arg.memory_handling
                         d_var['order'          ] = arg.order
 
             elif isinstance(func, Interface):
-                d_var = [self._infer_type(i, **settings) for i in
+                d_var = [self._infer_type(i.var, **settings) for i in
                          func.functions[0].results]
 
                 # TODO imporve this will not work for
                 # the case of different results types
                 d_var[0]['datatype'] = rhs.dtype
 
             else:
@@ -2483,15 +2581,15 @@
                         severity='error')
                     return None
             lhs = self._assign_lhs_variable(lhs, d_var, rhs, new_expressions, isinstance(expr, AugAssign), **settings)
         elif isinstance(lhs, PythonTuple):
             n = len(lhs)
             if isinstance(rhs, (PythonTuple, InhomogeneousTupleVariable, FunctionCall)):
                 if isinstance(rhs, FunctionCall):
-                    r_iter = rhs.funcdef.results
+                    r_iter = [r.var for r in rhs.funcdef.results]
                 else:
                     r_iter = rhs
                 new_lhs = []
                 for i,(l,r) in enumerate(zip(lhs,r_iter)):
                     d = self._infer_type(r, **settings)
                     new_lhs.append( self._assign_lhs_variable(l, d, r, new_expressions, isinstance(expr, AugAssign),arr_in_multirets=r.rank>0 ,**settings) )
                 lhs = PythonTuple(*new_lhs)
@@ -2613,15 +2711,14 @@
 
     def _visit_For(self, expr, **settings):
 
         scope = self.create_new_loop_scope()
 
         # treatment of the index/indices
         iterable = Iterable(self._visit(expr.iterable, **settings))
-        body     = list(expr.body.body)
 
         new_expr = []
 
         start = LiteralInteger(0)
         iterator_d_var = self._infer_type(start)
 
         iterator = expr.target
@@ -2660,15 +2757,15 @@
         else:
 
             errors.report(INVALID_FOR_ITERABLE, symbol=expr.target,
                    bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                    severity='error')
 
 
-        body = [self._visit(i, **settings) for i in body]
+        body = self._visit(expr.body, **settings)
 
         self.exit_loop_scope()
 
         if isinstance(iterable.iterable, Product):
             for_expr = body
             scopes = self.scope.create_product_loop_scope(scope, len(target))
 
@@ -3009,22 +3106,23 @@
     def _visit_Return(self, expr, **settings):
 
         results     = expr.expr
         f_name      = self._current_function
         if isinstance(f_name, DottedName):
             f_name = f_name.name[-1]
 
-        return_vars = self.scope.find(f_name, 'functions').results
+        return_objs = self.scope.find(f_name, 'functions').results
         assigns     = []
-        for v,r in zip(return_vars, results):
+        for o,r in zip(return_objs, results):
+            v = o.var
             if not (isinstance(r, PyccelSymbol) and r == (v.name if isinstance(v, Variable) else v)):
                 a = self._visit(Assign(v, r, fst=expr.fst))
                 assigns.append(a)
 
-        results = [self._visit(i, **settings) for i in return_vars]
+        results = [self._visit(i.var, **settings) for i in return_objs]
 
         # add the Deallocate node before the Return node and eliminating the Deallocate nodes
         # the arrays that will be returned.
         code = assigns + [Deallocate(i) for i in self._allocs[-1] if i not in results]
         if code:
             expr  = Return(results, CodeBlock(code))
         else:
@@ -3123,14 +3221,15 @@
 #            header_vec = header.vectorize(index_arg)
 #            vec_func   = expr.vectorize(body_vec, header_vec)
 
         interface_name = name
 
         for i, m in enumerate(interfaces):
             args           = []
+            arg_vars       = []
             results        = []
             global_vars    = []
             imports        = []
             arg            = None
             arguments      = expr.arguments
             header_results = m.results
 
@@ -3146,31 +3245,30 @@
                 dt        = self.get_class_construct(cls_name)()
                 cls_base  = self.scope.find(cls_name, 'classes')
                 var       = Variable(dt, 'self', cls_base=cls_base)
                 self.scope.insert_variable(var)
 
             if arguments:
                 for (a, ah) in zip(arguments, m.arguments):
-                    ah = ah.var
-                    additional_args = []
-                    if isinstance(ah, FunctionAddress):
+                    ahv = ah.var
+                    if isinstance(ahv, FunctionAddress):
                         d_var = {}
                         d_var['is_argument'] = True
                         d_var['memory_handling'] = 'alias'
                         if a.has_default:
                             # optional argument only if the value is None
                             if isinstance(a.value, Nil):
                                 d_var['is_optional'] = True
                         a_new = FunctionAddress(self.scope.get_expected_name(a.name),
-                                        ah.arguments, ah.results, [], **d_var)
+                                        ahv.arguments, ahv.results, [], **d_var)
                     else:
-                        d_var = self._infer_type(ah, **settings)
-                        d_var['shape'] = ah.alloc_shape
+                        d_var = self._infer_type(ahv, **settings)
+                        d_var['shape'] = ahv.alloc_shape
                         d_var['is_argument'] = True
-                        d_var['is_const'] = ah.is_const
+                        d_var['is_const'] = ahv.is_const
                         dtype = d_var.pop('datatype')
                         if not d_var['cls_base']:
                             d_var['cls_base'] = get_cls_base( dtype, d_var['precision'], d_var['rank'] )
 
                         if 'allow_negative_index' in self.scope.decorators:
                             if a.name in decorators['allow_negative_index']:
                                 d_var.update(allows_negative_indexes=True)
@@ -3186,35 +3284,34 @@
                             value.dtype is a_new.dtype and \
                             value.precision != a_new.precision:
                         value = convert_to_literal(value.python_value, a_new.dtype, a_new.precision)
 
                     arg_new = FunctionDefArgument(a_new,
                                 value=value,
                                 kwonly=a.is_kwonly,
-                                annotation=a.annotation)
-
-                    if additional_args:
-                        args += additional_args
+                                annotation=ah.annotation)
 
                     args.append(arg_new)
+                    arg_vars.append(a_new)
                     if isinstance(a_new, FunctionAddress):
                         self.insert_function(a_new)
                     else:
                         self.scope.insert_variable(a_new, a.name)
             results = expr.results
             if header_results:
                 new_results = []
 
                 for a, ah in zip(results, header_results):
-                    d_var = self._infer_type(ah, **settings)
+                    av = a.var
+                    d_var = self._infer_type(ah.var, **settings)
                     dtype = d_var.pop('datatype')
-                    a_new = Variable(dtype, self.scope.get_expected_name(a),
-                            **d_var, is_temp = a.is_temp)
-                    self.scope.insert_variable(a_new, a)
-                    new_results.append(a_new)
+                    a_new = Variable(dtype, self.scope.get_expected_name(av),
+                            **d_var, is_temp = av.is_temp)
+                    self.scope.insert_variable(a_new, av)
+                    new_results.append(FunctionDefResult(a_new, annotation = ah.annotation))
 
                 results = new_results
 
             # insert the FunctionDef into the scope
             # to handle the case of a recursive function
             # TODO improve in the case of an interface
             recursive_func_obj = FunctionDef(name, args, results, [])
@@ -3260,88 +3357,57 @@
             func_args = [i for i in self.scope.functions.values() if isinstance(i, FunctionAddress)]
             if func_args:
                 func_interfaces.append(Interface('', func_args, is_argument = True))
 
             namespace_imports = self.scope.imports
             self.exit_function_scope()
 
-            # ... computing inout arguments
-            args_inout = [False] * len(args)
-
-            results_names = [i.name for i in results]
+            results_names = [i.var.name for i in results]
 
             # Find all nodes which can modify variables
             assigns = body.get_attribute_nodes(Assign, excluded_nodes = (FunctionCall,))
             calls   = body.get_attribute_nodes(FunctionCall)
 
             # Collect the modified objects
             lhs_assigns   = [a.lhs for a in assigns]
-            modified_args = [func_arg for f in calls
-                                for func_arg, inout in zip(f.args,f.funcdef.arguments_inout) if inout]
+            modified_args = [call_arg.value for f in calls
+                                for call_arg, func_arg in zip(f.args, f.funcdef.arguments) if func_arg.inout]
             # Collect modified variables
             all_assigned = [v for a in (lhs_assigns + modified_args) for v in
                             (a.get_attribute_nodes(Variable) if not isinstance(a, Variable) else [a])]
 
-            permanent_assign = [a.name for a in all_assigned if a.rank > 0]
-            local_assign     = [i.name for i in all_assigned]
-
-            apps = [i for i in calls if (i.funcdef.name
-                    not in sub_funcs)]
-
-            d_apps = {a: [] for a in args}
-            for f in apps:
-                a_args = set(f.args) & set(args)
-                for a in a_args:
-                    d_apps[a].append(f)
-
-            for i, a in enumerate(args):
-                if a.name in chain(results_names, permanent_assign, ['self']):
-                    args_inout[i] = True
-
-                if d_apps[a] and not( args_inout[i] ):
-                    intent = False
-                    n_fa = len(d_apps[a])
-                    i_fa = 0
-                    while not(intent) and i_fa < n_fa:
-                        fa = d_apps[a][i_fa]
-                        f_name = fa.funcdef.name
-                        func = self.scope.find(f_name, 'functions')
-
-                        j = list(fa.args).index(a)
-                        intent = func.arguments_inout[j]
-                        if intent:
-                            args_inout[i] = True
-
-                        i_fa += 1
-                if isinstance(a.var, Variable):
+            # ... computing inout arguments
+            for a in args:
+                if a.name in chain(results_names, ['self']) or a.var in all_assigned:
                     v = a.var
-                    if v.is_const and (args_inout[i] or (v.name in local_assign)):
+                    if isinstance(v, Variable) and v.is_const:
                         msg = f"Cannot modify 'const' argument ({v})"
                         errors.report(msg, bounding_box=(self._current_fst_node.lineno,
                             self._current_fst_node.col_offset),
                             severity='fatal')
+                else:
+                    a.make_const()
             # ...
 
             # Raise an error if one of the return arguments is an alias.
             for r in results:
-                if r.is_alias:
+                if r.var.is_alias:
                     errors.report(UNSUPPORTED_POINTER_RETURN_VALUE,
                     symbol=r,bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='error')
 
             func_kwargs = {
                     'global_vars':global_vars,
                     'cls_name':cls_name,
                     'is_pure':is_pure,
                     'is_elemental':is_elemental,
                     'is_private':is_private,
                     'imports':imports,
                     'decorators':decorators,
                     'is_recursive':is_recursive,
-                    'arguments_inout':args_inout,
                     'functions': sub_funcs,
                     'interfaces': func_interfaces,
                     'doc_string': doc_string,
                     'scope': scope
                     }
             if is_inline:
                 func_kwargs['namespace_imports'] = namespace_imports
@@ -3561,15 +3627,15 @@
         if isinstance(expr.source, AsName):
             source        = expr.source.name
             source_target = expr.source.target
         else:
             source        = str(expr.source)
             source_target = source
 
-        if source in pyccel_builtin_import_registery:
+        if source in pyccel_builtin_import_registry:
             imports = pyccel_builtin_import(expr)
 
             def _insert_obj(location, target, obj):
                 F = self.scope.find(target)
 
                 if obj is F:
                     errors.report(FOUND_DUPLICATED_IMPORT,
@@ -3580,15 +3646,15 @@
                     errors.report(IMPORTING_EXISTING_IDENTIFIED,
                                   bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                                   severity='fatal')
 
             if expr.target:
                 for t in expr.target:
                     t_name = t.name if isinstance(t, AsName) else t
-                    if t_name not in pyccel_builtin_import_registery[source]:
+                    if t_name not in pyccel_builtin_import_registry[source]:
                         errors.report(f"Function '{t}' from module '{source}' is not currently supported by pyccel",
                                 symbol=expr,
                                 severity='error')
                 for (name, atom) in imports:
                     if not name is None:
                         if isinstance(atom, Decorator):
                             continue
@@ -3808,7 +3874,11 @@
         arg = func_call_args[0].value
         if not isinstance(arg, Variable):
             new_symbol = PyccelSymbol(self.scope.get_new_name())
             creation = self._visit(Assign(new_symbol, arg, fst=func_call.fst))
             self._additional_exprs[-1].append(creation)
             arg = self._visit(new_symbol)
         return NumpyWhere(arg)
+
+    def _visit_FunctionDefResult(self, expr, **settings):
+        var = self._visit(expr.var)
+        return FunctionDefResult(var, annotation = expr.annotation)
```

### Comparing `pyccel-1.7.3/pyccel/parser/syntactic.py` & `pyccel-1.7.4/pyccel/parser/syntactic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
-# pylint: disable=missing-function-docstring
-
 import os
 import re
 
 import ast
 
 #==============================================================================
 
@@ -32,14 +30,15 @@
 from pyccel.ast.core import If, IfSection
 from pyccel.ast.core import While
 from pyccel.ast.core import Del
 from pyccel.ast.core import Assert
 from pyccel.ast.core import Comment, EmptyNode
 from pyccel.ast.core import Break, Continue
 from pyccel.ast.core import FunctionDefArgument
+from pyccel.ast.core import FunctionDefResult
 from pyccel.ast.core import Import
 from pyccel.ast.core import AsName
 from pyccel.ast.core import CommentBlock
 from pyccel.ast.core import With
 from pyccel.ast.core import StarredArguments
 from pyccel.ast.core import CodeBlock
 from pyccel.ast.core import IndexedElement
@@ -100,19 +99,30 @@
 
 # use this to delete ansi_escape characters from a string
 # Useful for very coarse version differentiation.
 
 #==============================================================================
 
 class SyntaxParser(BasicParser):
+    """
+    Class which handles the syntactic stage as described in the developer docs.
 
-    """ Class for a Syntax Parser.
+    This class is described in detail in developer_docs/syntactic_stage.md.
+    It extracts all necessary information from the Python AST in order to create
+    a representation complete enough for the semantic stage to determine types, etc
+    as described in developer_docs/semantic_stage.md.
+
+    Parameters
+    ----------
+    inputs : str
+        A string containing code or containing the name of a file whose code
+        should be read.
 
-        inputs: str
-            filename or code to parse as a string
+    **kwargs : dict
+        Additional keyword arguments for BasicParser.
     """
 
     def __init__(self, inputs, **kwargs):
         BasicParser.__init__(self, **kwargs)
 
         # check if inputs is a file
         code = inputs
@@ -791,15 +801,15 @@
             name_available = all(r0 != a.name for a in arguments) and r0 in local_symbols
 
             if pyccel_symbol and same_results and name_available:
                 result_name = r0
             else:
                 result_name, result_counter = self.scope.get_new_incremented_symbol('Out', result_counter)
 
-            results.append(result_name)
+            results.append(FunctionDefResult(result_name))
 
         self.exit_function_scope()
 
         cls = InlineFunctionDef if is_inline else FunctionDef
         func = cls(
                name,
                arguments,
```

### Comparing `pyccel-1.7.3/pyccel/parser/syntax/basic.py` & `pyccel-1.7.4/pyccel/parser/syntax/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/syntax/headers.py` & `pyccel-1.7.4/pyccel/parser/syntax/headers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/syntax/himi.py` & `pyccel-1.7.4/pyccel/parser/syntax/himi.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/syntax/openacc.py` & `pyccel-1.7.4/pyccel/parser/syntax/openacc.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/syntax/openmp.py` & `pyccel-1.7.4/pyccel/parser/syntax/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/parser/utilities.py` & `pyccel-1.7.4/pyccel/parser/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/cwrapper/cwrapper.c` & `pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/cwrapper/cwrapper.h` & `pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c` & `pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h` & `pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/external/dfftpack.py` & `pyccel-1.7.4/pyccel/stdlib/external/dfftpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/external/fitpack.py` & `pyccel-1.7.4/pyccel/stdlib/external/fitpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/external/lapack.py` & `pyccel-1.7.4/pyccel/stdlib/external/lapack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/external/mpi4py.py` & `pyccel-1.7.4/pyccel/stdlib/external/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/blas.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/blas.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9585 8900 0000 0000 008c 2034 3262  ............ 42b
 00000010: 6161 3166 6235 3832 3336 3335 3866 3565  aa1fb58236358f5e
 00000020: 6636 6435 6530 3434 3362 3533 3894 8c05  f6d5e0443b538...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 911e 0000 2320 7079 6363 656c 2068 6561  ....# pyccel hea
 00000080: 6465 7220 666f 7220 424c 4153 2e0a 0a23  der for BLAS...#
 00000090: 2420 6865 6164 6572 206d 6574 6176 6172  $ header metavar
 000000a0: 206d 6f64 756c 655f 7665 7273 696f 6e3d   module_version=
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/blas.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/blas.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/dfftpack.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9529 1700 0000 0000 008c 2031 3362  ...)........ 13b
 00000010: 6133 3830 6537 3438 3037 6630 3830 3266  a380e74807f0802f
 00000020: 6366 3030 3564 6138 3432 6366 3894 8c05  cf005da842cf8...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 7804 0000 2320 7079 6363 656c 2068 6561  x...# pyccel hea
 00000080: 6465 7220 666f 7220 4446 5454 5041 434b  der for DFTTPACK
 00000090: 2e0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/dfftpack.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/fftw.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/fftw.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/fitpack.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9528 0b00 0000 0000 008c 2062 6362  ...(........ bcb
 00000010: 3932 6461 3730 6233 3364 3836 3939 3234  92da70b33d869924
 00000020: 6537 3333 3034 3531 3564 3365 3494 8c05  e73304515d3e4...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 5701 0000 2320 7079 6363 656c 2068 6561  W...# pyccel hea
 00000080: 6465 7220 666f 7220 4649 5450 4143 4b2e  der for FITPACK.
 00000090: 0a0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/hdf5.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/hdf5.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/lapack.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9599 0001 0000 0000 008c 2066 3964  ............ f9d
 00000010: 6365 6637 3662 6261 6633 6165 6261 6366  cef76bbaf3aebacf
 00000020: 3532 3330 3865 3364 3637 3736 3194 8c05  52308e3d67761...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 25e3 0000 2320 7079 6363 656c 2068 6561  %...# pyccel hea
 00000080: 6465 7220 666f 7220 4c41 5041 434b 2e0a  der for LAPACK..
 00000090: 0a23 2420 6865 6164 6572 206d 6574 6176  .#$ header metav
 000000a0: 6172 206d 6f64 756c 655f 7665 7273 696f  ar module_versio
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/lapack.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/mpi.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9597 6200 0000 0000 008c 2061 3734  ....b....... a74
 00000010: 6338 3636 3630 3230 6665 3735 6335 3935  c8666020fe75c595
 00000020: 3335 3238 6638 3532 3065 3939 3894 8c05  3528f8520e998...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 1717 0000 2320 7079 6363 656c 2068 6561  ....# pyccel hea
 00000080: 6465 7220 666f 7220 4d50 492e 0a23 0a0a  der for MPI..#..
 00000090: 2320 4f6e 2074 7261 7669 732c 2027 7573  # On travis, 'us
 000000a0: 6520 6d70 692c 206f 6e6c 793a 206d 7069  e mpi, only: mpi
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/mpi.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/mpiext.py` & `pyccel-1.7.4/pyccel/stdlib/internal/mpiext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/openacc.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 95fe 2a00 0000 0000 008c 2039 3265  ....*....... 92e
 00000010: 3531 6230 3535 3231 6330 3337 3164 3037  51b05521c0371d07
 00000020: 3034 6535 3738 3737 3135 3361 6294 8c05  04e57877153ab...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 730a 0000 2320 7079 6363 656c 2068 6561  s...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4143 432e  der for OpenACC.
 00000090: 0a23 204f 7065 6e41 4343 2064 6972 6563  .# OpenACC direc
 000000a0: 7469 7665 7320 616e 6420 436f 6e73 7472  tives and Constr
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/openacc.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/openmp.py` & `pyccel-1.7.4/pyccel/stdlib/internal/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/openmp.pyccel` & `pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 953a 2700 0000 0000 008c 2062 6331  ...:'....... bc1
 00000010: 3734 3231 3738 6137 6338 3035 6261 3062  742178a7c805ba0b
 00000020: 3630 3738 3263 6466 3138 3933 3194 8c05  60782cdf18931...
-00000030: 312e 372e 3394 8c17 7079 6363 656c 2e70  1.7.3...pyccel.p
+00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 550a 0000 2320 7079 6363 656c 2068 6561  U...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4d50 2e0a  der for OpenMP..
 00000090: 2320 4f70 656e 4d50 2064 6972 6563 7469  # OpenMP directi
 000000a0: 7665 7320 616e 6420 436f 6e73 7472 7563  ves and Construc
```

### Comparing `pyccel-1.7.3/pyccel/stdlib/internal/openmp.pyh` & `pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/math/pyc_math_c.c` & `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/math/pyc_math_c.h` & `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/math/pyc_math_f90.f90` & `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/ndarrays/ndarrays.c` & `pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/ndarrays/ndarrays.h` & `pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/numpy/numpy_c.c` & `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/numpy/numpy_c.h` & `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/numpy/numpy_f90.f90` & `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/stdlib/parallel/mpi.py` & `pyccel-1.7.4/pyccel/stdlib/parallel/mpi.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/symbolic/lambdify.py` & `pyccel-1.7.4/pyccel/symbolic/lambdify.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/utilities/metaclasses.py` & `pyccel-1.7.4/pyccel/utilities/metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/utilities/stage.py` & `pyccel-1.7.4/pyccel/utilities/stage.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel/utilities/strings.py` & `pyccel-1.7.4/pyccel/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/pyccel.egg-info/PKG-INFO` & `pyccel-1.7.4/pyccel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.7.3
+Version: 1.7.4
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 # Welcome to Pyccel
 
- [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade)
+ [![master_tests](https://github.com/pyccel/pyccel/actions/workflows/master.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/master.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -296,15 +296,15 @@
     ```
 
 -   **Development mode**:
 
     ```sh
     git clone git@github.com:pyccel/pyccel.git
     cd pyccel
-    pip3 install --user -e .[test]
+    pip3 install --user -e ".[test]"
     ```
 
 this will install a _python_ library **Pyccel** and a _binary_ called **`pyccel`**.
 Any required Python packages will be installed automatically from PyPI.
 
 ### On a read-only system
 
@@ -318,15 +318,15 @@
 A warning, reminding the user to execute this command, will be printed to the screen when pyccelising files which rely on these packages if the pickling step has not been executed.
 
 ## Additional packages
 
 In order to run the unit tests and to get a coverage report, a few additional Python packages should be installed:
 
 ```sh
-pip install --user -e .[test]
+pip install --user -e ".[test]"
 ```
 
 Most of the unit tests can also be run in parallel.
 
 ## Testing
 
 To test your Pyccel installation please run the script `tests/run\_tests\_py3.sh` (Unix), or `tests/run\_tests.bat` (Windows).
@@ -358,10 +358,13 @@
 Alternatively you may have docker or podman set the context using `-v $PWD:/data:rwz` instead of `-v $PWD:/data:rw` .
 
 ## Developer Documentation
 
 -   [Overview](./developer_docs/overview.md)
 -   [How to solve an issue](./developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](./developer_docs/review_process.md)
+-   [Development Conventions](./developer_docs/development_conventions.md)
 -   [Tips and Tricks](./developer_docs/tips_and_tricks.md)
+-   [Scope](./developer_docs/scope.md)
+-   [Array Ordering](./developer_docs/order_docs.md)
```

### Comparing `pyccel-1.7.3/pyccel.egg-info/SOURCES.txt` & `pyccel-1.7.4/pyccel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 AUTHORS
-CHANGES
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 pyccel/__init__.py
@@ -174,15 +173,14 @@
 tests/codegen/fcode/scripts/concatenation.py
 tests/codegen/fcode/scripts/context.py
 tests/codegen/fcode/scripts/decorators.py
 tests/codegen/fcode/scripts/decorators_elemental.py
 tests/codegen/fcode/scripts/decorators_pure.py
 tests/codegen/fcode/scripts/decorators_types.py
 tests/codegen/fcode/scripts/expressions.py
-tests/codegen/fcode/scripts/functions.py
 tests/codegen/fcode/scripts/functions_inout.py
 tests/codegen/fcode/scripts/generic_methods.py
 tests/codegen/fcode/scripts/headers.py
 tests/codegen/fcode/scripts/ifs.py
 tests/codegen/fcode/scripts/imports.py
 tests/codegen/fcode/scripts/issue_177.py
 tests/codegen/fcode/scripts/lists.py
@@ -482,14 +480,15 @@
 tests/pyccel/scripts/bool_comp.py
 tests/pyccel/scripts/c_arrays.py
 tests/pyccel/scripts/decorators_elemental.py
 tests/pyccel/scripts/decorators_inline.py
 tests/pyccel/scripts/default_args_mod.py
 tests/pyccel/scripts/expressions.py
 tests/pyccel/scripts/funcs.py
+tests/pyccel/scripts/functions.py
 tests/pyccel/scripts/generic_functions.py
 tests/pyccel/scripts/lapack_subroutine.py
 tests/pyccel/scripts/module_init.py
 tests/pyccel/scripts/module_init2.py
 tests/pyccel/scripts/print_integers.py
 tests/pyccel/scripts/print_sp_and_end.py
 tests/pyccel/scripts/print_strings.py
```

### Comparing `pyccel-1.7.3/samples/mxm_openmp.py` & `pyccel-1.7.4/samples/mxm_openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/setup.cfg` & `pyccel-1.7.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/setup.py` & `pyccel-1.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/ast/test_basic.py` & `pyccel-1.7.4/tests/ast/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     assert(all(isinstance(a, Variable) for a in atts))
 
     expected = [Variable('int', 'a'),
                 Variable('int', 'b'),
                 Variable('int', 'c'),
                 Variable('int', 'd'),
                 Variable('int', 'e'),
-                Variable('int', 'f')]
+                Variable('int', 'g')]
 
     for e in expected:
         assert(e in atts)
 
 def test_get_attribute_nodes_exclude():
     filename = os.path.join(path_dir, "math.py")
 
@@ -89,19 +89,16 @@
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
 
-    ret_assign = a_var.get_user_nodes(Assign, excluded_nodes = (PyccelAdd,PyccelMinus))
-
-    assert(len(ret_assign) == 1)
-    ret = ret_assign[0].get_user_nodes(Return)
-    assert(len(ret)==1)
+    plus_assign = a_var.get_user_nodes(Assign, excluded_nodes = PyccelMinus)
+    assert(len(plus_assign)==2)
 
 def test_get_direct_user_nodes():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
 
     fst = get_functions(filename)[0]
@@ -148,15 +145,15 @@
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
     old_parents = set(a_var.get_user_nodes(Basic))
     assert(len(a_var.get_user_nodes(Basic))>0)
 
-    fst.substitute(a_var, new_var, excluded_nodes=(Return))
+    fst.substitute(a_var, new_var, excluded_nodes=(PyccelMinus))
 
     assert(len(a_var.get_user_nodes(Basic))==1)
 
     atts = set(fst.get_attribute_nodes(Variable))
     assert(new_var in atts)
 
     new_parents = set(new_var.get_user_nodes(Basic))
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/arrays.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 #==============================================================================
 
 @types( 'int[:,:](order=C)' )
 def double_loop_on_2d_array_C( z ):
 
     from numpy import shape
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_create.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #==============================================================================
 
 def array_create_C_literal_value():
 
     from numpy import array
 
     a = array([0, 0, 0]) #pylint:disable=unused-variable
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_indexing.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_indexing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #==============================================================================
 from pyccel.decorators import allow_negative_index
 
 def array_getitem_C():
 
     from numpy import array
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_pointers.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_pointers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #==============================================================================
 
 def allocatable_to_pointer():
 
     from numpy import array
 
     a = array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/arrays_slicing.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_slicing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import allow_negative_index
 #==============================================================================
 
 def array_view_C_literals():
 
     from numpy import array
     z = array([[1, 2, 3], [4, 5, 6]])
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/functions.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=unused-variable
-
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function fib(int) results(int)
 def fib(n):
     if n < 2:
         return n
     i = fib(n-1)
     j = fib(n-2)
@@ -45,13 +43,15 @@
 z = f1(1)
 
 z1 = f2(1)
 z2 = f2(1, m=0)
 
 helloworld()
 
+print(y)
+print(z)
+
 print(z1)
 print(z2)
 
 def pass_fun():
     pass
-
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/ifs.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/ifs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 x = 0
 y = 0
 z = 3
 
 if 1<0:
     x=4
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/scripts/loops.py` & `pyccel-1.7.4/tests/codegen/ccode/scripts/loops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 #==============================================================================
 
 @types( int )
 def sum_natural_numbers( n ):
     x = 0
```

### Comparing `pyccel-1.7.3/tests/codegen/ccode/test_ccode_codegen.py` & `pyccel-1.7.4/tests/codegen/fcode/test_fcode_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 import os
 import pytest
@@ -10,23 +10,22 @@
 from pyccel.parser.parser   import Parser
 from pyccel.codegen.codegen import Codegen
 from pyccel.errors.errors   import Errors
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 path_dir = os.path.join(base_dir, 'scripts')
 
-failing_files = {}
 files = sorted(os.listdir(path_dir))
 files = [os.path.join(path_dir,f) \
-         if f not in failing_files \
-         else pytest.param(os.path.join(path_dir,f), marks = pytest.mark.xfail(reason=failing_files[f])) \
+         #if f not in failing_files \
+         #else pytest.param(os.path.join(path_dir,f), marks = pytest.mark.xfail(reason=failing_files[f])) \
          for f in files \
          if f.endswith(".py") \
         ]
-@pytest.mark.c
+@pytest.mark.fortran
 @pytest.mark.parametrize("f", files)
 def test_codegen(f):
 
     # reset Errors singleton
     errors = Errors()
     errors.reset()
 
@@ -42,26 +41,25 @@
     # Assert semantic success
     assert(not errors.has_errors())
 
     name = os.path.basename(f)
     name = os.path.splitext(name)[0]
 
     codegen = Codegen(ast, name)
-    codegen.doprint(language='c')
+    codegen.doprint()
 
     # Assert codegen success
     assert(not errors.has_errors())
 
 ######################
 if __name__ == '__main__':
     print('*********************************')
     print('***                           ***')
-    print('***  TESTING CODEGEN CCODE   ***')
+    print('***   TESTING CODEGEN FCODE   ***')
     print('***                           ***')
     print('*********************************')
 
     for f in files:
         print('> testing {0}'.format(str(os.path.basename(f))))
         test_codegen(f)
 
     print('\n')
-
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/CommentBlock.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/CommentBlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 """
    ___________________THIS IS A LONG STRING ___________________
    ___________________THIS IS A LONG STRING ___________________
    ___________________THIS IS A LONG STRING ___________________
    ___________________THIS IS A LONG STRING ___________________
    ___________________THIS IS A LONG STRING ___________________
    ___________________THIS IS A LONG STRING ___________________
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/Functional_Stmts.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/Functional_Stmts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 a0 = [6]*10
 a1 = sum(a0[i] for i in range(len(a0)))
 a2 = sum(i for i in a0)
 a3 = max(i if i>k else k for i in range(5) for k in range(10))
 a4 = min(k if i>k else 0 if i==k else i for i in range(5) for k in range(10))
 
 #$ header function incr(int)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/classes.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #$ header class Point(public)
 #$ header method __init__(Point, double, double)
 #$ header method __del__(Point)
 #$ header method translate(Point, double, double)
 
 class Point(object):
     def __init__(self, x, y):
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/classes_2.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 from numpy import ones
 #$ header class Point(public)
 #$ header method __init__(Point, double [:])
 #$ header method __del__(Point)
 #$ header method translate(Point, double [:])
 
 #$ header class Points(public)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/classes_3.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 from numpy import ones
 #$ header class Point(public)
 #$ header method __init__(Point, [double])
 #$ header method __del__(Point)
 #$ header method translate(Point, [double])
 
 #$ header class Points(public)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/classes_4.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #An example of a class
 #$ header class Shape(public)
 #$ header method __init__(Shape, double, double)
 #$ header method area(Shape) results(double)
 #$ header method perimeter(Shape) results(double)
 #$ header method describe(Shape,str)
 #$ header method authorName(Shape,str)
@@ -12,18 +12,20 @@
 
     def __init__(self, x, y):
         self.x = x
         self.y = y
         self.description = "This shape has not been described yet"
         self.author = "Nobody has claimed to make this shape yet"
 
+    @property
     def area(self):
         y = self.x * self.y
         return y
 
+    @property
     def perimeter(self):
         x = 2 * self.x + 2 * self.y
         return x
 
     def describe(self, text):
         self.description = text
 
@@ -32,20 +34,24 @@
 
     def scaleSize(self, scale):
         self.x = self.x * scale
         self.y = self.y * scale
 
 rectangle = Shape(100., 45.)
 #finding the area of your rectangle:
-print(rectangle.area())
+print(rectangle.area)
 
-#finding the perimeter of your rectangle:
-print(rectangle.perimeter())
+#$ header function f(int)
+#@inline
+#def f(t):
+#    x = 5*t
+#    return x
+# y = f(6)
+
+#$ header function g(int)
+@vectorize(z)
+def g(z):
+    x= 5+z
+    return x
 
-#describing the rectangle
-rectangle.describe("A wide rectangle, more than twice as wide as it is tall")
 
-#making the rectangle 50% smaller
-rectangle.scaleSize(0.5)
 
-#re-printing the new area of the rectangle
-print(rectangle.area())
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/context.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 # coding: utf-8
 
 #$ header class Parallel(public, with, openmp)
 #$ header method __init__(Parallel, str, str, str [:], str [:], str [:], str [:], str, str [:], str)
 #$ header method __del__(Parallel)
 #$ header method __enter__(Parallel)
 #$ header method __exit__(Parallel, str, str, str)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/decorators.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_4.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #An example of a class
 #$ header class Shape(public)
 #$ header method __init__(Shape, double, double)
 #$ header method area(Shape) results(double)
 #$ header method perimeter(Shape) results(double)
 #$ header method describe(Shape,str)
 #$ header method authorName(Shape,str)
@@ -12,20 +12,18 @@
 
     def __init__(self, x, y):
         self.x = x
         self.y = y
         self.description = "This shape has not been described yet"
         self.author = "Nobody has claimed to make this shape yet"
 
-    @property
     def area(self):
         y = self.x * self.y
         return y
 
-    @property
     def perimeter(self):
         x = 2 * self.x + 2 * self.y
         return x
 
     def describe(self, text):
         self.description = text
 
@@ -34,24 +32,20 @@
 
     def scaleSize(self, scale):
         self.x = self.x * scale
         self.y = self.y * scale
 
 rectangle = Shape(100., 45.)
 #finding the area of your rectangle:
-print(rectangle.area)
+print(rectangle.area())
 
-#$ header function f(int)
-#@inline
-#def f(t):
-#    x = 5*t
-#    return x
-# y = f(6)
-
-#$ header function g(int)
-@vectorize(z)
-def g(z):
-    x= 5+z
-    return x
+#finding the perimeter of your rectangle:
+print(rectangle.perimeter())
 
+#describing the rectangle
+rectangle.describe("A wide rectangle, more than twice as wide as it is tall")
 
+#making the rectangle 50% smaller
+rectangle.scaleSize(0.5)
 
+#re-printing the new area of the rectangle
+print(rectangle.area())
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/decorators_types.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types(int)
 def incr_(x):
     @types(int)
     def decr_(y): # pylint: disable=unused-variable
         y = y-1
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/functions.py` & `pyccel-1.7.4/tests/semantic/scripts/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=unused-variable
-
-#$ header function incr_(int)
-def incr_(x):
-    #$ header function decr_(int)
-    def decr_(y):
-        y = y-1
-    x = x + 1
+# pylint: disable=missing-function-docstring, missing-module-docstring
+# this file is used inside imports.py
+# make sure that you update the imports.py file if needed
 
 def helloworld():
     print('hello world')
 
 #$ header function incr(int)
 def incr(x):
     x = x + 1
@@ -23,33 +17,29 @@
 # TODO [YG, 30.01.2020] function behavior in Python not correct:
 #      must change to x += 1
 #
 #$ header function incr_array(int [:])
 def incr_array(x):
     x = x + 1
 
-y_=[1,2,3]
-
-# #$ header function decr_array([int]) results([int])
-# def decr_array(x):
-#     y_[1] = 6
-#     z = y_
-#     t = y_+x
-#     return t
+##$ header function decr_array(int [:]) results(int [:])
+#def decr_array(x):
+#    y = x - 1
+#    return y
 
 # TODO [YG, 30.01.2020] function behavior in Python not correct:
 #      must change to x -= 1
 #
 #$ header function decr_array(int [:])
 def decr_array(x):
     x = x - 1
 
 #$ header function f1(int, int, int) results(int)
-def f1(x, n=2, m=3):
-    y = x - n*m
+def f1(x, n=2, m=None):
+    y = x - n
     return y
 
 #$ header function f2(int, int) results(int)
 def f2(x, m=None):
     if m is None:
         y = x + 1
     else:
@@ -58,15 +48,10 @@
 
 y = decr(2)
 z = f1(1)
 
 z1 = f2(1)
 z2 = f2(1, m=0)
 
-helloworld()
-
+# TODO add messages. for the moment there's a bug in Print
 print(z1)
 print(z2)
-
-def pass_fun():
-    pass
-
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/functions_inout.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/functions_inout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # TODO add AugAssign to these tests
 
 #$ header function f_assign(int, double [:])
 def f_assign(m1, x):
     x[:] = 0.
     for i in range(0, m1):
         x[i] = i * 1.
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/ifs.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/ifs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 
 x = 0
 y = 0
 z = 3
 b = zeros(64,'int')
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/loops.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 x = 0
 for i in range(0,4):
     x = 2 *i
 
 x = 0
 for i in range(0,10):
     x = x + 1
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/macros.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/macros.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 
 # .....................................
 #           1d case
 # .....................................
 #$ header function f(int, int [:])
 #$ header macro __f(x) := f(x.shape, x)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/matrix_assembly.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 w_u = zeros(4, 'double')
 w_v = zeros(4, 'double')
 
 b_0 = zeros((4,4), 'double')
 b_s = zeros((4,4), 'double')
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/matrix_mul.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_mul.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 from numpy import shape
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     n, m = shape(a)
     m, p = shape(b)
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/numpyext.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/numpyext.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 from numpy import ones
 from numpy import sum as np_sum
 from numpy import array
 from numpy import shape
 #from numpy import diag
 from numpy import zeros_like
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/precision.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/precision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # pylint: disable=unused-variable
 
 #$ header function incr_(int*8)
 def incr_(x):
     #$ header function decr_(int*8)
     def decr_(y):
         y = y-1
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/scripts/recursive_functions.py` & `pyccel-1.7.4/tests/codegen/fcode/scripts/recursive_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 @types(int, results=int)
 def fact(n):
     if n == 0:
        z = 1
        return z
     else:
```

### Comparing `pyccel-1.7.3/tests/codegen/fcode/test_fcode_codegen.py` & `pyccel-1.7.4/tests/codegen/ccode/test_ccode_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 import os
 import pytest
@@ -10,22 +10,23 @@
 from pyccel.parser.parser   import Parser
 from pyccel.codegen.codegen import Codegen
 from pyccel.errors.errors   import Errors
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 path_dir = os.path.join(base_dir, 'scripts')
 
+failing_files = {}
 files = sorted(os.listdir(path_dir))
 files = [os.path.join(path_dir,f) \
-         #if f not in failing_files \
-         #else pytest.param(os.path.join(path_dir,f), marks = pytest.mark.xfail(reason=failing_files[f])) \
+         if f not in failing_files \
+         else pytest.param(os.path.join(path_dir,f), marks = pytest.mark.xfail(reason=failing_files[f])) \
          for f in files \
          if f.endswith(".py") \
         ]
-@pytest.mark.fortran
+@pytest.mark.c
 @pytest.mark.parametrize("f", files)
 def test_codegen(f):
 
     # reset Errors singleton
     errors = Errors()
     errors.reset()
 
@@ -41,25 +42,26 @@
     # Assert semantic success
     assert(not errors.has_errors())
 
     name = os.path.basename(f)
     name = os.path.splitext(name)[0]
 
     codegen = Codegen(ast, name)
-    codegen.doprint()
+    codegen.doprint(language='c')
 
     # Assert codegen success
     assert(not errors.has_errors())
 
 ######################
 if __name__ == '__main__':
     print('*********************************')
     print('***                           ***')
-    print('***   TESTING CODEGEN FCODE   ***')
+    print('***  TESTING CODEGEN CCODE   ***')
     print('***                           ***')
     print('*********************************')
 
     for f in files:
         print('> testing {0}'.format(str(os.path.basename(f))))
         test_codegen(f)
 
     print('\n')
+
```

### Comparing `pyccel-1.7.3/tests/codegen/pycode/scripts/loops.py` & `pyccel-1.7.4/tests/codegen/pycode/scripts/loops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 #==============================================================================
 
 @types( int )
 def sum_natural_numbers( n ):
     x = 0
```

### Comparing `pyccel-1.7.3/tests/codegen/pycode/test_pycode_codegen.py` & `pyccel-1.7.4/tests/codegen/pycode/test_pycode_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 import os
 import pytest
```

### Comparing `pyccel-1.7.3/tests/complexity/test_complexity.py` & `pyccel-1.7.4/tests/complexity/test_complexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.complexity.memory import MemComplexity
 from pyccel.complexity.arithmetic import OpComplexity
 import os
 import pytest
 
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
```

### Comparing `pyccel-1.7.3/tests/conftest.py` & `pyccel-1.7.4/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import os
 import shutil
 import pytest
 from mpi4py import MPI
 from pyccel.commands.pyccel_clean import pyccel_clean
 
 # Uncomment to debug  pytest-xdist errors
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/Module_5.py` & `pyccel-1.7.4/tests/epyccel/modules/Module_5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('int')
 def nothing(x = None):
     if x is None :
         return 2
     return x
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/Module_6.py` & `pyccel-1.7.4/tests/epyccel/modules/Module_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 def set_i(x : 'float[:]', i : 'int', val : 'float'):
     x[i] = val
 
 def swap(x : 'float[:]', i : 'int', j : 'int'):
     temp = x[i]
     x[i] = x[j]
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/Module_7.py` & `pyccel-1.7.4/tests/epyccel/modules/Module_7.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 
 def fill_a( r: float, a: 'int[:]' ):
 
     if ( r == 0.0 ):
         return 0
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/array_consts.py` & `pyccel-1.7.4/tests/epyccel/modules/array_consts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/epyccel/modules/arrays.py` & `pyccel-1.7.4/tests/epyccel/modules/arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 
 from pyccel.decorators import types, template, stack_array, allow_negative_index
 
 a_1d   = np.array([1 << i for i in range(21)], dtype=int)
 a_1d_overflow = np.array([(1 << i) - 1 for i in range(32)], dtype=int)
 a_2d_f = np.array([[1 << j for j in range(21)] for i in range(21)], dtype=int, order='F')
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/augassign.py` & `pyccel-1.7.4/tests/epyccel/modules/augassign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 from pyccel.decorators import types
 
 # +=
 
 @types('int[:]')
 def augassign_add_1d_int(a):
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/base.py` & `pyccel-1.7.4/tests/epyccel/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('bool')
 def is_false(a):
     c = False
     if a is False:
         c = True
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/bitwise.py` & `pyccel-1.7.4/tests/epyccel/modules/bitwise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('bool', 'bool')
 def right_shift_b_b(a, b):
     return a >> b
 
 @types('int', 'int')
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/call_user_defined_funcs.py` & `pyccel-1.7.4/tests/epyccel/modules/call_user_defined_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # This module test call user defined functions
 # through nested functions
 
 from pyccel.decorators import types
 
 def do_nothing():
     x = 0
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/complex_func.py` & `pyccel-1.7.4/tests/epyccel/modules/complex_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 def create_complex_literal__int_int():
     a = complex(1,-2)
     return a
 
 def create_complex_literal__int_float():
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/external_functions.py` & `pyccel-1.7.4/tests/epyccel/modules/external_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 
 # ==============================================================================
 def blas_dnrm2(x: 'float64[:]',
                incx: 'int32' = 1,
               ):
     """
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/functionals.py` & `pyccel-1.7.4/tests/epyccel/modules/functionals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 def functional_for_1d_range():
     a = [i+1 for i in range(4)]
     return len(a), a[0], a[1], a[2], a[3]
 
 def functional_for_overwrite_1d_range():
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/generic_functions.py` & `pyccel-1.7.4/tests/epyccel/modules/generic_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 from pyccel.decorators import template
 
 #$ header function gen_2(real, int)
 #$ header function gen_2(int, real)
 #$ header function gen_4(T, T)
 #$ header function tmplt_head_1(int, real)
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/generic_functions_2.py` & `pyccel-1.7.4/tests/epyccel/modules/generic_functions_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 from pyccel.decorators import template
 
 
 @template('Z', types=['int', 'real'])
 @types('Z', 'Z')
 def tmplt_1(x, y):
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/highorder_functions.py` & `pyccel-1.7.4/tests/epyccel/modules/highorder_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
- # pylint: disable=missing-function-docstring, missing-module-docstring/
+ # pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 #$ header function function(int)
 def function(a):
     return a
 
 #$ header function f1(int)
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/loops.py` & `pyccel-1.7.4/tests/epyccel/modules/loops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 #==============================================================================
 
 @types( int )
 def sum_natural_numbers( n ):
     x = 0
@@ -240,7 +240,21 @@
     return x
 
 def for_loop3():
     x = 0
     for i in range(10, 1, -2):
         x += i
     return x
+
+def temp_array_in_loop(a : 'int[:]', b : 'int[:]'):
+    import numpy as np
+    c = np.zeros_like(a)
+    d1 = np.zeros_like(a)
+    d2 = np.zeros_like(a)
+    for _ in range(1):
+        for d in range(2):
+            b[d] += d
+        c[:] = b - a
+        d1[:] = np.abs(c)
+        d2[:] = np.abs(b - a)
+    return d1, d2
+
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/mpi_collective.py` & `pyccel-1.7.4/tests/epyccel/modules/mpi_collective.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy  import empty
 
 from pyccel.decorators import types
 
 # TODO: avoid declaration of integer variables 'ierr' and 'rank'
 # TODO: allow access to process rank through property 'comm.rank'
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/mpi_point_to_point.py` & `pyccel-1.7.4/tests/epyccel/modules/mpi_point_to_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 from pyccel.decorators import types
 
 #==============================================================================
 
 #
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/multi_rank.py` & `pyccel-1.7.4/tests/epyccel/modules/multi_rank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('real[:,:]','real[:,:](order=F)')
 def add_mixed_order(a,b):
     a[:] = a + b
 
 @types('real[:,:]','real[:,:](order=F)')
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/numpy_sign.py` & `pyccel-1.7.4/tests/epyccel/modules/numpy_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring\
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 from pyccel.decorators import types
 
 def complex_nul():
     import numpy as np
     b = np.sign(complex(0+0j))
     return b
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/openmp.py` & `pyccel-1.7.4/tests/epyccel/modules/openmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=wildcard-import
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types(int)
 def set_num_threads(n):
     import numpy as np
     from pyccel.stdlib.internal.openmp import omp_set_num_threads
     omp_set_num_threads(np.int32(n))
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/pointers.py` & `pyccel-1.7.4/tests/epyccel/modules/pointers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 __all__ = [
         'slice_is_pointer_idx_0',
         'array_copy_is_pointer',
         'pointer_to_pointer_is_pointer',
         'reassigned_pointer',
         'reassigned_pointer_shape'
         ]
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/python_annotations.py` & `pyccel-1.7.4/tests/epyccel/modules/python_annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 def array_int32_1d_scalar_add( x:'int32[:]', a:'int32' ):
     x[:] += a
 
 def array_int32_2d_C_scalar_add( x:'int32[:,:]', a:'int32' ):
     x[:,:] += a
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/strings.py` & `pyccel-1.7.4/tests/epyccel/modules/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 __all__ = [
         'one_quote',
         'two_quote',
         'three_quote',
         'concatenate',
         'concatenate_multiple',
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/tuples.py` & `pyccel-1.7.4/tests/epyccel/modules/tuples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types, pure
 
 __all__ = [
         'homogenous_tuple_int',
         'homogenous_tuple_bool',
         'homogenous_tuple_float',
         'homogenous_tuple_string',
```

### Comparing `pyccel-1.7.3/tests/epyccel/modules/types.py` & `pyccel-1.7.4/tests/epyccel/modules/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 def test_int_default(x : 'int'):
     return x
 
 def test_int64(x : 'int64'):
     return x
```

### Comparing `pyccel-1.7.3/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py` & `pyccel-1.7.4/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import sys
 import pytest
 from numpy.random import randint, uniform
 from numpy import isclose
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/epyccel/recognised_functions/test_math_funcs.py` & `pyccel-1.7.4/tests/epyccel/recognised_functions/test_math_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 from numpy.random import rand, randint, uniform
 from numpy import isclose
 
 from pyccel.decorators import types
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/recognised_functions/test_numpy_funcs.py` & `pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/epyccel/recognised_functions/test_numpy_types.py` & `pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/epyccel/test_array_as_func_args.py` & `pyccel-1.7.4/tests/epyccel/test_array_as_func_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/epyccel/test_arrays.py` & `pyccel-1.7.4/tests/epyccel/test_arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 from numpy import iinfo
 from numpy.random import randint
 
 from pyccel.epyccel import epyccel
 from modules        import arrays
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_arrays_multiple_assignments.py` & `pyccel-1.7.4/tests/epyccel/test_arrays_multiple_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import stack_array, types
 from pyccel.errors.errors import Errors, PyccelSemanticError
 from pyccel.errors.messages import (ARRAY_REALLOCATION,
                                     ARRAY_DEFINITION_IN_LOOP,
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_base.py` & `pyccel-1.7.4/tests/epyccel/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 
 from modules import base
 from utilities import epyccel_test
 
 
 def test_is_false(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_bitwise.py` & `pyccel-1.7.4/tests/epyccel/test_bitwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 
 from pyccel.epyccel import epyccel
 from modules import bitwise
 
 @pytest.mark.parametrize("a, b",[(True, False),(True, True)])
 def test_right_shift_b_b(language, a, b):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_builtins.py` & `pyccel-1.7.4/tests/epyccel/test_builtins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 from numpy.random import randint, uniform
 from numpy import iinfo, finfo
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types, template
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_class_expressions.py` & `pyccel-1.7.4/tests/epyccel/test_class_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 import pytest
 from numpy.random import randint
 from pyccel.epyccel import epyccel
 
 def test_complex_imag(language):
     def f():
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_compare_expressions.py` & `pyccel-1.7.4/tests/epyccel/test_compare_expressions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from utilities import epyccel_test
 from pyccel.decorators import types
 
 #==============================================================================
 @types('int, int, int')
 def mod_eq_pow(a, m, n):
     return a%m == n**2
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_default_precision_template.py` & `pyccel-1.7.4/tests/epyccel/test_default_precision_template.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/epyccel/test_docstrings.py` & `pyccel-1.7.4/tests/epyccel/test_docstrings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.epyccel import epyccel
 
 def test_1_line_docstring(language):
     def f():
         """ short doc string """
         return 1
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_IfTernaryOperator.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_IfTernaryOperator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import pytest
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
 # wp suffix means With Parentheses
 #------------------------------------------------------------------------------
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_augassign.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_augassign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import numpy as np
 import modules.augassign as mod
 
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_complex_func.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_complex_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 import pytest
 
 from numpy.random import rand, randint
 
 import modules.complex_func as mod
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_decorators.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import pytest
 import numpy as np
 from pyccel.epyccel import epyccel
 from pyccel.decorators import private, inline
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_default_args.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_default_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_division.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_division.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=wildcard-import
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy.random import randint, uniform
 from numpy import isclose
-from conftest       import *
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
 
 RTOL = 2e-14
 ATOL = 1e-15
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_functions.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_generators.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 from numpy.random import randint, rand
 
 from pyccel.epyccel import epyccel
 
 def test_sum_range(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_mod.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_mod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import sys
 from numpy.random import randint, uniform
 from numpy import allclose
 
 from pyccel.decorators import types
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_modules.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.epyccel import epyccel
 
 RTOL = 2e-14
 ATOL = 1e-15
 
 def test_module_1(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_multi_rank.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_multi_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 from numpy.random import rand, randint
 
 from modules        import multi_rank
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_openmp.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_openmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=wildcard-import
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import multiprocessing
 import os
 import sys
 import pytest
 import numpy as np
 import modules.openmp as openmp
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_optional_args.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_optional_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_pow.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_pow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import sys
 from numpy.random import rand, randint, uniform
 from numpy import isclose
 
 from pyccel.decorators import types
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_python_annotations.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_python_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from numpy.random import randint
 
 from pyccel.epyccel import epyccel
 from modules import python_annotations
 
 def test_array_int32_1d_scalar_add(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_return_arrays.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_return_arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy.random import randint, uniform
 import numpy as np
 import pytest
 
 from recognised_functions.test_numpy_funcs import (min_int, max_int, min_int8, max_int8,
                                 min_int16, max_int16, min_int32, max_int32, max_int64, min_int64)
 from recognised_functions.test_numpy_funcs import max_float, min_float, max_float32, min_float32,max_float64, min_float64
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_sign.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import numpy as np
 import modules.numpy_sign as mod
 
 from pyccel.epyccel import epyccel
 
 def test_sign_complex(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_transpose.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import empty, array_equal
 from numpy.random import randint
 
 from pyccel.epyccel import epyccel
 
 
 def test_transpose_shape(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_epyccel_types.py` & `pyccel-1.7.4/tests/epyccel/test_epyccel_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import numpy as np
 from numpy.random import randint, uniform
 
 from modules import types
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_external_functions.py` & `pyccel-1.7.4/tests/epyccel/test_external_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import sys
 import pytest
 import numpy as np
 import scipy.linalg.blas as sp_blas
 import modules.external_functions as mod
 from pyccel.epyccel import epyccel
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_functionals.py` & `pyccel-1.7.4/tests/epyccel/test_functionals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy.random import randint
 from numpy import equal
 
 from pyccel.epyccel import epyccel
 from modules import functionals
 
 def compare_epyccel(f, language, *args):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_generic_functions.py` & `pyccel-1.7.4/tests/epyccel/test_generic_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 import modules.generic_functions as mod
 import modules.generic_functions_2 as mod2
 from pyccel.epyccel import epyccel
 
 @pytest.fixture(scope="module")
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_higherorder_functions.py` & `pyccel-1.7.4/tests/epyccel/test_higherorder_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 import modules.highorder_functions as mod
 from pyccel.epyccel import epyccel
 
 @pytest.fixture(scope="module")
 def modnew(language):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_imports.py` & `pyccel-1.7.4/tests/epyccel/test_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 import pytest
 from numpy import ones
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_kind.py` & `pyccel-1.7.4/tests/epyccel/test_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import platform
 from pyccel.decorators import types
 from pyccel.epyccel import epyccel
 
 def test_or_boolean(language):
     @types('bool', 'bool')
     def or_bool(a, b):
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_loops.py` & `pyccel-1.7.4/tests/epyccel/test_loops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from modules        import loops
 
 #==============================================================================
@@ -196,14 +196,32 @@
     max_val = 12
 
     out1 = f1(fizz, buzz, max_val)
     out2 = f2(fizz, buzz, max_val)
 
     assert( out1 == out2 )
 
+def test_temp_array_in_loop(language):
+    f1 = loops.temp_array_in_loop
+    f2 = epyccel( f1, language = language )
+
+    a = np.zeros(6, dtype=int)
+    b = np.zeros(6, dtype=int)
+
+    c_py,d_py = f1(a,b)
+
+    a[:] = 0
+    b[:] = 0
+
+    c_ep,d_ep = f2(a,b)
+
+    assert np.array_equal(c_py, c_ep)
+    assert np.array_equal(d_py, d_ep)
+
+
 ##==============================================================================
 ## CLEAN UP GENERATED FILES AFTER RUNNING TESTS
 ##==============================================================================
 #
 #def teardown_module():
 #    import os, glob
 #    dirname  = os.path.dirname( loops.__file__ )
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_mpi_collective.py` & `pyccel-1.7.4/tests/epyccel/test_mpi_collective.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 import numpy as np
 import pytest
 
 from pyccel.epyccel import epyccel
 from modules        import mpi_collective as pmod
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_mpi_point_to_point.py` & `pyccel-1.7.4/tests/epyccel/test_mpi_point_to_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 import numpy as np
 import pytest
 
 from pyccel.epyccel import epyccel
 from modules        import mpi_point_to_point as pmod
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_multiple_results.py` & `pyccel-1.7.4/tests/epyccel/test_multiple_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import pure, types
 from pyccel.epyccel import epyccel
 
 #==============================================================================
 def compare_epyccel(f1, *args, language):
     f2 = epyccel(f1, language=language)
     out1 = f1(*args)
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_parallel_epyccel.py` & `pyccel-1.7.4/tests/epyccel/test_parallel_epyccel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 
 RTOL = 2e-14
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_pointers.py` & `pyccel-1.7.4/tests/epyccel/test_pointers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import inspect
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from modules import pointers as pointers_module
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_return.py` & `pyccel-1.7.4/tests/epyccel/test_return.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, disable=unused-variable, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, reimported
 import numpy as np
 from pyccel.decorators import types
 from pyccel.epyccel import epyccel
 
 def test_single_return_var_assign(language):
     def single_return_var_assign():
         y = 3
@@ -80,15 +80,15 @@
         return a
     epyc_scalare_multi_return_stmts = epyccel(scalare_multi_return_stmts, language=language, fflags="-Werror -Wunused-variable")
     assert (epyc_scalare_multi_return_stmts(7) == scalare_multi_return_stmts(7))
 
 def test_create_arr(language):
     def create_arr(i : int):
         import numpy as np
-        a = np.ones(i)
+        _ = np.ones(i)
         return True
     epyc_create_arr = epyccel(create_arr, language=language, fflags="-Werror -Wunused-variable")
     assert (epyc_create_arr(7) == create_arr(7))
 
 def test_return_arr_element(language):
     def return_arr_element(i : int):
         import numpy as np
@@ -96,17 +96,17 @@
         return a[0]
     epyc_return_arr_element = epyccel(return_arr_element, language=language, fflags="-Werror -Wunused-variable")
     assert (epyc_return_arr_element(7) == return_arr_element(7))
 
 def test_create_multi_arrs(language):
     def create_multi_arrs(i : int):
         import numpy as np
-        a = np.ones(i)
-        b = np.zeros(i)
-        c = np.zeros(i)
+        _ = np.ones(i)
+        _ = np.zeros(i)
+        _ = np.zeros(i)
         return True
     epyc_create_multi_arrs = epyccel(create_multi_arrs, language=language, fflags="-Werror -Wunused-variable")
     assert (epyc_create_multi_arrs(7) == create_multi_arrs(7))
 
 def test_expr_arrs_elements(language):
     def expr_arrs_elements(i : int):
         import numpy as np
@@ -144,38 +144,38 @@
             a[i] = ai/b
 
     epyc_divide_by = epyccel(divide_by, language=language)
     x = np.ones(5)
     x_copy = x.copy()
     b = 0.01
     divide_by(x,b)
-    divide_by(x_copy,b)
+    epyc_divide_by(x_copy,b)
     assert np.allclose(x, x_copy, rtol=1e-13, atol=1e-14)
-    b = 4
+    b = 4.0
     divide_by(x,b)
-    divide_by(x_copy,b)
+    epyc_divide_by(x_copy,b)
     assert np.allclose(x, x_copy, rtol=1e-13, atol=1e-14)
 
 def test_return_None(language):
     def divide_by(a : 'float[:]', b : 'float'): # pylint: disable=inconsistent-return-statements
         if abs(b)<0.1:
             return None
         for i,ai in enumerate(a):
             a[i] = ai/b
 
     epyc_divide_by = epyccel(divide_by, language=language)
     x = np.ones(5)
     x_copy = x.copy()
     b = 0.01
     divide_by(x,b)
-    divide_by(x_copy,b)
+    epyc_divide_by(x_copy,b)
     assert np.allclose(x, x_copy, rtol=1e-13, atol=1e-14)
-    b = 4
+    b = 4.0
     divide_by(x,b)
-    divide_by(x_copy,b)
+    epyc_divide_by(x_copy,b)
     assert np.allclose(x, x_copy, rtol=1e-13, atol=1e-14)
 
 def test_arg_arr_element_op(language):
     def return_mult_arr_arg_element(i: 'int', arg:'float[:]'):
         import numpy as np
         a = np.ones(i)
         return a[0] * arg[0]
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_strings.py` & `pyccel-1.7.4/tests/epyccel/test_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import inspect
 import pytest
 
 from pyccel.epyccel import epyccel
 from modules import strings as strings_module
 
 string_funcs = [(f, getattr(strings_module,f)) for f in strings_module.__all__ if inspect.isfunction(getattr(strings_module,f))]
```

### Comparing `pyccel-1.7.3/tests/epyccel/test_tuples.py` & `pyccel-1.7.4/tests/epyccel/test_tuples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import inspect
 import pytest
 import numpy as np
 
 from pyccel.epyccel import epyccel
 from modules import tuples as tuples_module
```

### Comparing `pyccel-1.7.3/tests/epyccel/utilities.py` & `pyccel-1.7.4/tests/epyccel/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.epyccel import epyccel
 
 
 #==============================================================================
 class epyccel_test:
     """
```

### Comparing `pyccel-1.7.3/tests/errors/known_bugs/generic_methods.py` & `pyccel-1.7.4/tests/errors/known_bugs/generic_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #$ header class Point(public)
 #$ header method __init__(Point, double, double)
 #$ header method __del__(Point)
 #$ header method translate(Point, double|int, double|int)
 
 class Point(object):
     def __init__(self, x, y):
```

### Comparing `pyccel-1.7.3/tests/errors/known_bugs/header_interface.py` & `pyccel-1.7.4/tests/errors/known_bugs/header_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.stdlib.internal.blas import daxpy
 from pyccel.stdlib.internal.blas import saxpy
 
 #$header interface axpy=daxpy|saxpy
 
 # > Usage:
 #
```

### Comparing `pyccel-1.7.3/tests/errors/known_bugs/inheritance.py` & `pyccel-1.7.4/tests/errors/known_bugs/inheritance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #$ header class Point2d(public)
 #$ header method __init__(Point2d, double, double)
 #$ header method translate(Point2d, double, double)
 
 class Point2d:
     def __init__(self, x, y):
         self.x = x
```

### Comparing `pyccel-1.7.3/tests/errors/test_errors.py` & `pyccel-1.7.4/tests/errors/test_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 # TODO - syntax errors tests
 #      - expected errors in log files for every script
```

### Comparing `pyccel-1.7.3/tests/external/scripts/lapack/ex1.py` & `pyccel-1.7.4/tests/external/scripts/lapack/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/bcast.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/bcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 comm = MPI.COMM_WORLD
 rank_in_world = comm.Get_rank()
 
 size_ = comm.Get_size()
 master = 0
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/bugs/ex6.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 
 # we need to declare these variables somehow,
 # since we are calling mpi subroutines
 
 size = -1
 rank = -1
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/bugs/ex8.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 rank = -1
 #we must initialize rank
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/gather.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
 size_ = comm.Get_size()
 
 master    = 1
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/np_Bcast.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Bcast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 
 size_ = -1
 rank_in_world = -1
 
 comm = MPI.COMM_WORLD
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/np_Gather.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Gather.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 
 # we need to declare these variables somehow,
 # since we are calling mpi subroutines
 size_ = -1
 rank = -1
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/np_Sendrecv.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Sendrecv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
 size = comm.Get_size()
 
 # Send messages around in a ring
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/np_point_to_point.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 from numpy import ones
 
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/np_point_to_point_3.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
 size_ = comm.Get_size()
```

### Comparing `pyccel-1.7.3/tests/external/scripts/mpi4py/point_to_point_3.py` & `pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
 size_ = comm.Get_size()
 
 nx = 4
```

### Comparing `pyccel-1.7.3/tests/external/test_external.py` & `pyccel-1.7.4/tests/external/test_external.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # TODO test if compiler exists before running mpi, openacc
 #      execute the binary file
 
 import pytest
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/blas/ex1.py` & `pyccel-1.7.4/tests/internal/scripts/blas/ex1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # > Usage:
 #
 #   pyccel test.py -t
 #   gfortran test.f90 -lblas
 #   ./a.out
 
 # TODO add saxpy test
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/blas/ex2.py` & `pyccel-1.7.4/tests/internal/scripts/blas/ex2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.stdlib.internal.blas import dgemv
 import numpy as np
 
 if __name__ == '__main__':
     n = np.int32(4)
     m = np.int32(5)
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/blas/ex3.py` & `pyccel-1.7.4/tests/internal/scripts/blas/ex3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.stdlib.internal.blas import dger
 import numpy as np
 
 if __name__ == '__main__':
     n = np.int32(4)
     m = np.int32(5)
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/blas/ex4.py` & `pyccel-1.7.4/tests/internal/scripts/blas/ex4.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.stdlib.internal.blas import dgemm
 import numpy as np
 
 if __name__ == '__main__':
     m = np.int32(4)
     k = np.int32(5)
     n = np.int32(4)
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/blas/ex5.py` & `pyccel-1.7.4/tests/internal/scripts/blas/ex5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import inline
 
 def f(x: 'float32[:]'):
     import pyccel.stdlib.internal.blas as blas_mod
     n = np.int32(x.shape[0])
     incx = np.int32(1)
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/lapack/ex1.py` & `pyccel-1.7.4/tests/internal/scripts/lapack/ex1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # > Usage:
 #
 #   pyccel test.py -t
 #   gfortran test.f90 -lblas -llapack
 #   ./a.out
 
 # TODO: - assert
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/allgather.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/allgather.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/allreduce.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/allreduce.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/alltoall.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/alltoall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/bcast.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/bcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/column.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/gather.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/gather.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/line.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/nonblocking.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/nonblocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/point_to_point_1.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/point_to_point_2.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/reduce.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/reduce.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/scatter.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/scatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/sendrecv.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/sendrecv_replace.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv_replace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/split.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/split.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/mpi/who_am_i.py` & `pyccel-1.7.4/tests/internal/scripts/mpi/who_am_i.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/openacc/sum.py` & `pyccel-1.7.4/tests/internal/scripts/openacc/sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from numpy import zeros
 
 if __name__ == '__main__':
     nx = 1024
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/openacc/sum_kernels.py` & `pyccel-1.7.4/tests/internal/scripts/openacc/sum_kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from numpy import zeros
 
 if __name__ == '__main__':
     nx = 1024
```

### Comparing `pyccel-1.7.3/tests/internal/scripts/openmp/ex1.py` & `pyccel-1.7.4/tests/internal/scripts/openmp/ex1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.openmp import omp_get_num_threads
 from pyccel.stdlib.internal.openmp import omp_get_max_threads
 from pyccel.stdlib.internal.openmp import omp_get_thread_num
 
 if __name__ == '__main__':
```

### Comparing `pyccel-1.7.3/tests/internal/test_internal.py` & `pyccel-1.7.4/tests/internal/test_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # TODO test if compiler exists before execute_pyccelning mpi, openacc
 #      execute the binary file
 
 import os
 import pytest
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/bcast.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/bcast.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 if __name__ == '__main__':
     size = -1
     rank_in_world = -1
 
     comm = MPI.COMM_WORLD
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/bug/ex6.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.stdlib.internal.mpi import mpi_init
 from pyccel.stdlib.internal.mpi import mpi_finalize
 from pyccel.stdlib.internal.mpi import mpi_comm_size
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
 from pyccel.stdlib.internal.mpi import mpi_comm_world
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/bug/ex8.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 rank = -1
 #we must initialize rank
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/gather.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/gather.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 if __name__ == '__main__':
     # we need to declare these variables somehow,
     # since we are calling mpi subroutines
     size = -1
     rank = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/mpi4py.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/mpi4py.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #$ header class MPI_(public)
 #$ header method __init__(MPI_)
 
 
 
 from pyccel.stdlib.internal.mpi import mpi_comm_world
 from pyccel.stdlib.internal.mpi import mpi_comm_rank
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_Allreduce.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_Reduce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import ones
 from numpy import zeros
 
 if __name__ == '__main__':
     rank = -1
     #we must initialize rank
@@ -13,12 +13,12 @@
 
     if rank == 0:
         value = ones(50,'int')
     else:
         value = zeros(50,'int')
 
     sum_value = zeros(50,'int')
-    comm.Allreduce (value, sum_value, MPI.SUM)
+    comm.Reduce (value, sum_value, MPI.SUM, root)
 
     if rank == 0:
         print('I, process ', root,', have the global sum value ', sum_value)
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_Bcast.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_Bcast.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 
 if __name__ == '__main__':
     size = -1
     rank_in_world = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_Gather.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_Gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 
 if __name__ == '__main__':
     # we need to declare these variables somehow,
     # since we are calling mpi subroutines
     size = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_Reduce.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_Sendrecv.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
-from numpy import ones
-from numpy import zeros
 
 if __name__ == '__main__':
     rank = -1
     #we must initialize rank
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
 
-    root = 0
-
     if rank == 0:
-        value = ones(50,'int')
-    else:
-        value = zeros(50,'int')
-
-    sum_value = zeros(50,'int')
-    comm.Reduce (value, sum_value, MPI.SUM, root)
+        partner = 1
 
-    if rank == 0:
-        print('I, process ', root,', have the global sum value ', sum_value)
+    if rank == 1:
+        partner = 0
 
+    msg = rank + 1000
+    val = -1
+    tag = 1234
+
+    val=comm.Sendrecv(msg, 1, tag, source=partner, recvtag=tag)
+    #both of these works
+    #comm.Sendrecv(msg, 1, tag, val, partner, tag)
+    print('I, process ', rank, ', I received', val, ' from process ', partner)
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 from numpy import ones
 
 
 if __name__ == '__main__':
     rank = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point_2.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 from mpi4py import MPI
 from numpy import zeros
 
 if __name__ == '__main__':
     # we need to declare these variables somehow,
     # since we are calling mpi subroutines
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/np_point_to_point_3.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 from numpy import zeros
 # we need to declare these variables somehow,
 # since we are calling mpi subroutines
 
 if __name__ == '__main__':
     size = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/point_to_point_2.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 from mpi4py import MPI
 
 if __name__ == '__main__':
     # we need to declare these variables somehow,
     # since we are calling mpi subroutines
     size = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/MPI/point_to_point_3.py` & `pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from mpi4py import MPI
 
 if __name__ == '__main__':
     # we need to declare these variables somehow,
     # since we are calling mpi subroutines
 
     size = -1
```

### Comparing `pyccel-1.7.3/tests/macro/scripts/blas/runtest_daxpy.py` & `pyccel-1.7.4/tests/macro/scripts/blas/runtest_daxpy.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/scripts/blas/runtest_dgemm.py` & `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemm.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/scripts/blas/runtest_dgemv.py` & `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/scripts/blas/runtest_dger.py` & `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dger.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/scripts/blas/runtest_dswap.py` & `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dswap.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/scripts/lapack/runtest_dgbtrf.py` & `pyccel-1.7.4/tests/macro/scripts/lapack/runtest_dgbtrf.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/macro/test_macro.py` & `pyccel-1.7.4/tests/macro/test_macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # TODO test if compiler exists before execute_pyccelning mpi, openacc
 #      execute the binary file
 
 from pyccel.codegen.pipeline import execute_pyccel
 import os
```

### Comparing `pyccel-1.7.3/tests/ndarrays/conftest.py` & `pyccel-1.7.4/tests/ndarrays/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-# pylint: disable=arguments-differ, inconsistent-return-statements, protected-access, abstract-method/
+# pylint: disable=missing-function-docstring, missing-module-docstring
+# pylint: disable=arguments-differ, inconsistent-return-statements, protected-access, abstract-method
 import subprocess
 import os
 import pathlib
 import sys
 import shutil
 import pytest
```

### Comparing `pyccel-1.7.3/tests/ndarrays/leaks_check.py` & `pyccel-1.7.4/tests/ndarrays/leaks_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import array, zeros
 
 def create_array():
     a = array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])# pylint: disable=unused-variable
 
 def array_to_pointer():
     a = array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])
```

### Comparing `pyccel-1.7.3/tests/ndarrays/test_ndarrays.c` & `pyccel-1.7.4/tests/ndarrays/test_ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/parser/scripts/comments.py` & `pyccel-1.7.4/tests/parser/scripts/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 def f(a: int):
     # 1
     if a:
         # 2
         b = (a + 2)
```

### Comparing `pyccel-1.7.3/tests/parser/test_comments.py` & `pyccel-1.7.4/tests/parser/test_comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 import os
 import pytest
```

### Comparing `pyccel-1.7.3/tests/parser/test_headers.py` & `pyccel-1.7.4/tests/parser/test_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 from pyccel.parser.syntax.headers import parse
 
 def test_variable():
     print (parse(stmts='#$ header variable x :: int'))
     print (parse(stmts='#$ header variable x float [:, :]'))
```

### Comparing `pyccel-1.7.3/tests/preprocess/scripts/omp.py` & `pyccel-1.7.4/tests/preprocess/scripts/omp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # this tests shows that OpenMP directives are moved to the appropriate parent
 
 #$ omp for nowait schedule(runtime)
 for i in range(0, n):
     for j in range(0, m):
```

### Comparing `pyccel-1.7.3/tests/preprocess/test_preprocess.py` & `pyccel-1.7.4/tests/syntax/test_syntax.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import os
 import pytest
 
 from pyccel.parser.parser import Parser
 from pyccel.errors.errors import Errors
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 path_dir = os.path.join(base_dir, 'scripts')
 
 files = sorted(os.listdir(path_dir))
-files = [os.path.join(path_dir,f) for f in files if (f.endswith(".py"))]
-
-@pytest.mark.parametrize("f", files)
-def test_preprocess(f):
-    pyccel = Parser(f)
-    pyccel.parse()
-    print(pyccel.fst)
+files = [os.path.join(path_dir, f) for f in files if (f.endswith(".py"))]
 
+@pytest.mark.parametrize( "f", files)
+def test_syntax(f):
     # reset Errors singleton
     errors = Errors()
     errors.reset()
 
+    pyccel = Parser(f)
+    pyccel.parse()
+
+    # Assert syntactic success
+    assert not errors.has_errors()
+
 ######################
 if __name__ == '__main__':
     print('*********************************')
     print('***                           ***')
-    print('***     TESTING preprocess    ***')
+    print('***      TESTING SYNTAX       ***')
     print('***                           ***')
     print('*********************************')
 
     for f in files:
         print('> testing {0}'.format(str(os.path.basename(f))))
-        test_preprocess(f)
-
-    print('\n')
+        test_syntax(f)
+        print('\n')
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/array_binary_operation.py` & `pyccel-1.7.4/tests/pyccel/scripts/array_binary_operation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import types
 
 @types('int', 'int')
 def my_pow(n, m):
     return n ** m
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/arrays_view.py` & `pyccel-1.7.4/tests/pyccel/scripts/arrays_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import allow_negative_index, types
 
 def array_view():
     a = np.array([[1, 2, 3, 4, 5], [6, 7, 8, 9, 10]])
     b = a[:, :]
     for i in range(2):
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/bool_comp.py` & `pyccel-1.7.4/tests/pyccel/scripts/bool_comp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('bool')
 def is_false(a):
     c = False
     if a is False:
         c = True
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/c_arrays.py` & `pyccel-1.7.4/tests/pyccel/scripts/c_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 
 if __name__ == '__main__':
     # ---------------------------- Array creation ---------------------------------
     ac0 = np.array([0])
 
     ac1 = np.array([0, 0, 0, 0])
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/classes/classes.py` & `pyccel-1.7.4/tests/pyccel/scripts/classes/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-class-docstring,  disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-class-docstring,  missing-function-docstring, missing-module-docstring
 #$ header class Point(public)
 #$ header method __init__(Point, double, double)
 #$ header method __del__(Point)
 #$ header method translate(Point, double, double)
 
 class Point(object):
     def __init__(self, x, y):
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/classes/classes_1.py` & `pyccel-1.7.4/tests/pyccel/scripts/classes/classes_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-class-docstring,  disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-class-docstring, missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 #$ header class Point(public)
 #$ header method __init__(Point, double[:])
 #$ header method __del__(Point)
 #$ header method translate(Point, double[:])
 import numpy as np
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/decorators_inline.py` & `pyccel-1.7.4/tests/pyccel/scripts/decorators_inline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import inline
 
 pi = 3.14159
 
 @inline
 def get_powers(s : int):
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/default_args_mod.py` & `pyccel-1.7.4/tests/pyccel/scripts/default_args_mod.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 from pyccel.decorators import types
 
 #------------------------------------------------------------------------------
 @types('int')
 def f1(x = 1):
     y = x - 1
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/expressions.py` & `pyccel-1.7.4/tests/pyccel/scripts/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 a1 = 2/2
 a2 = 2/2j
 
 a3 = 2//2
 a4 = 2.//2
 a5 = 2//4.
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/generic_functions.py` & `pyccel-1.7.4/tests/pyccel/scripts/generic_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import types
 from pyccel.decorators import template
 
 #$ header function gen_2(real, int)
 #$ header function gen_2(int, real)
 #$ header function gen_4(T, T)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function ln_python(double)
 def ln_python (X) :
     return (X-1) - (X-1)**2 / 2 + (X-1)**3 / 3 - (X-1)**4 / 4 + (X-1)**5 / 5 - (X-1)**6 / 6 + (X-1)**7 / 7 - (X-1)**8 / 8 + (X-1)**9 / 9
 
 #$ header function ln_python_exp(double)
 def ln_python_exp (Y) :
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function pairwise_python(double[:,:],double[:,:])
 def pairwise_python (X, D) :
     from numpy import sqrt, shape
 
     M, N = shape( X )
     for i in range (M) :
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
+from pyccel.decorators import types
 
-#$ header function pdf(double[:,:],int,int,double,double,double[:,:],double,double,double)
+@types('double[:,:]','int','int','double','double','double[:,:]','double','double','double')
 def pdf ( density , x_range , y_range , x_center , y_center , w2D, r50 , b , a) :
     from numpy import sqrt, pi, sum as np_sum
     for x in range ( x_range ) :
         for y in range ( y_range ) :
             dr = sqrt ( ( x - x_center ) ** 2 + ( y - y_center ) ** 2)
             tmp = 2 * (b - 1) / (2 * pi * ( r50 * a ) **2) * (1 + ( dr / ( r50 * a ) ) **2)**(-b)
             density [ x , y ] = tmp * np_sum(w2D)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks/quicksort.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/quicksort.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function qsort_kernel(double[:],int,int)
 def qsort_kernel ( a , lo , hi ) :
     i = lo
     j = hi
     while i < hi :
         pivot = a[ ( lo + hi ) // 2 ]
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('double')
 def ln_python (X) :
     return (X-1) - (X-1)**2 / 2 + (X-1)**3 / 3 - (X-1)**4 / 4 + (X-1)**5 / 5 - (X-1)**6 / 6 + (X-1)**7 / 7 - (X-1)**8 / 8 + (X-1)**9 / 9
 
 @types('double')
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('double[:,:]','double[:,:]')
 def pairwise_python (X, D) :
     from numpy import sqrt, shape
 
     M, N = shape( X )
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
-from pyccel.decorators import types
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
-@types('double[:,:]','int','int','double','double','double[:,:]','double','double','double')
+#$ header function pdf(double[:,:],int,int,double,double,double[:,:],double,double,double)
 def pdf ( density , x_range , y_range , x_center , y_center , w2D, r50 , b , a) :
     from numpy import sqrt, pi, sum as np_sum
     for x in range ( x_range ) :
         for y in range ( y_range ) :
             dr = sqrt ( ( x - x_center ) ** 2 + ( y - y_center ) ** 2)
             tmp = 2 * (b - 1) / (2 * pi * ( r50 * a ) **2) * (1 + ( dr / ( r50 * a ) ) **2)**(-b)
             density [ x , y ] = tmp * np_sum(w2D)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py` & `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import types
 
 @types('double[:]','int','int')
 def qsort_kernel ( a , lo , hi ) :
     i = lo
     j = hi
     while i < hi :
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros, shape
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     n, m = shape(a)
     m, p = shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros as zilch
 from numpy import shape as form
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     nm = form(a)
     mp = form(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     from numpy import shape as form
     nm = form(a)
     mp = form(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/from_mod_import_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from numpy import zeros
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     from numpy import shape
     n, m = shape(a)
     m, p = shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     n, m = numpy.shape(a)
     m, p = numpy.shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     n, m = np.shape(a)
     m, p = np.shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_as_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function matmat(double [:, :], double [:, :], double [:, :])
 def matmat(a, b, c):
     import numpy as np #pylint: disable=W0404
     n, m = np.shape(a)
     m, p = np.shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/import_syntax/import_mod_func.py` & `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 
 #$ header function matmat(double [:,:], double [:,:], double [:,:])
 def matmat(a,b,c):
     import numpy #pylint: disable=W0404
     n, m = numpy.shape(a)
     m, p = numpy.shape(b)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/lapack_subroutine.py` & `pyccel-1.7.4/tests/pyccel/scripts/lapack_subroutine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # Matrix inverse test using dgetri and dgetrf subroutines
 
 from numpy import zeros,float64,int32
 from pyccel.stdlib.internal.lapack import dgetrf
 from pyccel.stdlib.internal.lapack  import dgetri
 
 def dgetrf_test(A: 'float64[:,:](order=F)',piv:'int32[:]'):
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/numpy/numpy_kernels.py` & `pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_kernels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #
 # Testing various kernels, adapted from
 # https://github.com/redmod-team/profit/blob/master/profit/sur/backend/kernels.py
 #
 
 import numpy as np
 from pyccel.decorators import types
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/numpy/numpy_sign.py` & `pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 
 if __name__ == "__main__":
     print(np.sign(0))
     print(np.sign(-0))
     print(np.sign(np.int8(0)))
     print(np.sign(np.int8(-0)))
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/print_integers.py` & `pyccel-1.7.4/tests/pyccel/scripts/print_integers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # ------------------------------- Strings ------------------------------------
 
 from numpy import int32, int64, int16, int8
 if __name__ == '__main__':
     print(0)
     print(00)
     print(1)
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/print_sp_and_end.py` & `pyccel-1.7.4/tests/pyccel/scripts/print_sp_and_end.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #  ------------------------string with sep and end ---------------------------
 
 if __name__ == '__main__':
     print('ahoy', 'world', sep=' ')
     print('ohoy', 'awa', sep='')
     print('bonjour', 'Le monde', sep='\n')
     print('home', 'user', 'documents', sep='/')
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/print_strings.py` & `pyccel-1.7.4/tests/pyccel/scripts/print_strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # ------------------------------- Strings ------------------------------------
 
 if __name__ == '__main__':
     print("mcha bba lsbata")
     print('voilaaa')
     print("3...2...1...Go!")
     print('line1 \n line2\nline3')
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/return_numpy_arrays.py` & `pyccel-1.7.4/tests/pyccel/scripts/return_numpy_arrays.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, disable=unused-variable, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import numpy as np
 from pyccel.decorators import types
 
 def single_return():
     a = np.array([1,2,3,4])
     return a
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/runtest_default_args.py` & `pyccel-1.7.4/tests/pyccel/scripts/runtest_default_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 import numpy as np
 
 if __name__ == '__main__':
     from default_args_mod import f1, f5, f3, is_nil_default_arg, recursivity, print_var
 
     print(f1(2))
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/runtest_degree_in.py` & `pyccel-1.7.4/tests/pyccel/scripts/runtest_degree_in.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import stack_array, pure
 
 @pure
 @stack_array('tmp')
 def test_degree(degree : int):
     from numpy import empty
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/runtest_generic_functions.py` & `pyccel-1.7.4/tests/pyccel/scripts/runtest_generic_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import generic_functions as mod
 
 if __name__ == '__main__':
     print(mod.tst_gen_1())
     print(mod.tst_gen_2())
     print(mod.tst_gen_3())
     print(mod.tst_gen_4())
```

### Comparing `pyccel-1.7.3/tests/pyccel/scripts/runtest_multiple_results.py` & `pyccel-1.7.4/tests/pyccel/scripts/runtest_multiple_results.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 from pyccel.decorators import pure, types
 
 @pure
 def const_int_float():
     return 1, 3.4
 
 if __name__ == '__main__':
```

### Comparing `pyccel-1.7.3/tests/pyccel/test_pyccel.py` & `pyccel-1.7.4/tests/pyccel/test_pyccel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 import subprocess
 import json
 import os
 import shutil
 import sys
 import re
 import pytest
@@ -131,16 +131,20 @@
     value = conversion(match.group())
     string = string[match.span()[1]:]
     return value, string
 
 def compare_pyth_fort_output_by_type( p_output, f_output, dtype=float, language=None):
 
     if dtype is str:
-        p_list = [e.strip() for e in re.split('\n', p_output)]
-        f_list = [e.strip() for e in re.split('\n', f_output)]
+        p_output_split = re.split('\n', p_output)
+        f_output_split = re.split('\n', f_output)
+        p_list = p_output_split[0].strip()
+        f_list = f_output_split[0].strip()
+        p_output = '\n'.join(p_output_split[1:])
+        f_output = '\n'.join(f_output_split[1:])
         assert(p_list==f_list)
     elif dtype is complex:
         rx = re.compile('[-0-9.eEj]+')
         p, p_output = get_value(p_output, rx, complex)
         if p.imag == 0:
             p2, p_output = get_value(p_output, rx, complex)
             p = p+p2
@@ -949,14 +953,20 @@
     compare_pyth_fort_output(pyth_out, lang_out, [float, float, float, int, float, float, float, int], language)
 
 def test_function_aliasing():
     pyccel_test("scripts/runtest_function_alias.py",
             language = 'fortran')
 
 #------------------------------------------------------------------------------
+
+def test_function(language):
+    pyccel_test("scripts/functions.py",
+            language = language, output_dtype=[str]+[int]*7 )
+
+#------------------------------------------------------------------------------
 @pytest.mark.xdist_incompatible
 def test_inline(language):
     pyccel_test("scripts/decorators_inline.py", language = language)
 
 #------------------------------------------------------------------------------
 @pytest.mark.xdist_incompatible
 @pytest.mark.parametrize( 'language', (
```

### Comparing `pyccel-1.7.3/tests/run_tests.bat` & `pyccel-1.7.4/tests/run_tests.bat`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/run_tests_py3.sh` & `pyccel-1.7.4/tests/run_tests_py3.sh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tests/semantic/scripts/expressions.py` & `pyccel-1.7.4/tests/semantic/scripts/expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # this file is used inside imports.py
 # make sure that you update the imports.py file if needed
 # pylint: disable=unused-variable
 
 ai = 1
 bi = ai
 ci = ai + 1
```

### Comparing `pyccel-1.7.3/tests/semantic/test_semantic.py` & `pyccel-1.7.4/tests/semantic/test_semantic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import os
 import pytest
 
 from pyccel.parser.parser import Parser
 from pyccel.errors.errors import Errors
```

### Comparing `pyccel-1.7.3/tests/symbolic/scripts/decorator.py` & `pyccel-1.7.4/tests/symbolic/scripts/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 #@sympy
 #def g_sympy(t,i0):
 #    #This function must return a sympy expression
 #    #that depends on the arguments of the function
 #    from sympy import symbols, Eq, dsolve, solve, Derivative, sin
```

### Comparing `pyccel-1.7.3/tests/symbolic/scripts/neural_net.py` & `pyccel-1.7.4/tests/symbolic/scripts/neural_net.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 #$ header function f(double[:],double[:,:,:],int)
 @sympy
 def g(v,w,i):
     from sympy import Lambda, Function ,symbols ,IndexedBase,Idx ,Max, Sum
     x = Function('x')
     i, n, j, dim, k =symbols('i, n, j, dim, k')
     v=IndexedBase('v')
```

### Comparing `pyccel-1.7.3/tests/symbolic/test_symbolic.py` & `pyccel-1.7.4/tests/symbolic/test_symbolic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import os
 import pytest
 
 from pyccel.parser.parser   import Parser
 from pyccel.codegen.codegen import Codegen
```

### Comparing `pyccel-1.7.3/tests/syntax/scripts/Functional_Stmts.py` & `pyccel-1.7.4/tests/syntax/scripts/Functional_Stmts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 a0 = [6]*10
 a1 = sum(a0[i] for i in range(len(a0)))
 a2 = sum(i for i in a0)
 a3 = max(i if i>k else k for i in range(5) for k in range(10))
 a4 = min(k if i>k else 0 if i==k else i for i in range(5) for k in range(10))
 
 #$ header function incr(int)
```

### Comparing `pyccel-1.7.3/tests/syntax/scripts/expressions.py` & `pyccel-1.7.4/tests/syntax/scripts/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 # pylint: disable=pointless-statement, undefined-variable
 
 None
 
 
 1
```

### Comparing `pyccel-1.7.3/tests/syntax/test_syntax.py` & `pyccel-1.7.4/tests/preprocess/test_preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 import os
 import pytest
 
 from pyccel.parser.parser import Parser
 from pyccel.errors.errors import Errors
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 path_dir = os.path.join(base_dir, 'scripts')
 
 files = sorted(os.listdir(path_dir))
-files = [os.path.join(path_dir, f) for f in files if (f.endswith(".py"))]
-
-@pytest.mark.parametrize( "f", files)
-def test_syntax(f):
-    # reset Errors singleton
-    errors = Errors()
-    errors.reset()
+files = [os.path.join(path_dir,f) for f in files if (f.endswith(".py"))]
 
+@pytest.mark.parametrize("f", files)
+def test_preprocess(f):
     pyccel = Parser(f)
     pyccel.parse()
+    print(pyccel.fst)
 
-    # Assert syntactic success
-    assert not errors.has_errors()
+    # reset Errors singleton
+    errors = Errors()
+    errors.reset()
 
 ######################
 if __name__ == '__main__':
     print('*********************************')
     print('***                           ***')
-    print('***      TESTING SYNTAX       ***')
+    print('***     TESTING preprocess    ***')
     print('***                           ***')
     print('*********************************')
 
     for f in files:
         print('> testing {0}'.format(str(os.path.basename(f))))
-        test_syntax(f)
-        print('\n')
+        test_preprocess(f)
+
+    print('\n')
```

### Comparing `pyccel-1.7.3/tests/warnings/test_warnings.py` & `pyccel-1.7.4/tests/warnings/test_warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=missing-function-docstring, missing-module-docstring/
+# pylint: disable=missing-function-docstring, missing-module-docstring
 # coding: utf-8
 
 # Note that we need to change the directory for tests involving the import
 # statement
 
 # TODO warnings for syntax and semantic stages
```

### Comparing `pyccel-1.7.3/tutorial/builtin-functions.md` & `pyccel-1.7.4/tutorial/builtin-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/compiler.md` & `pyccel-1.7.4/tutorial/compiler.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/const_keyword.md` & `pyccel-1.7.4/tutorial/const_keyword.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/decorators.md` & `pyccel-1.7.4/tutorial/decorators.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/function-pointers-as-arguments.md` & `pyccel-1.7.4/tutorial/function-pointers-as-arguments.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/header-files.md` & `pyccel-1.7.4/tutorial/header-files.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/ndarrays.md` & `pyccel-1.7.4/tutorial/ndarrays.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/numpy-functions.md` & `pyccel-1.7.4/tutorial/numpy-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/openmp.md` & `pyccel-1.7.4/tutorial/openmp.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/quickstart.md` & `pyccel-1.7.4/tutorial/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.3/tutorial/templates.md` & `pyccel-1.7.4/tutorial/templates.md`

 * *Files identical despite different names*

