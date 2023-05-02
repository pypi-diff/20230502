# Comparing `tmp/waveforms-1.5.93.tar.gz` & `tmp/waveforms-1.5.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveforms-1.5.93.tar", last modified: Fri Apr 28 02:47:16 2023, max compression
+gzip compressed data, was "waveforms-1.5.94.tar", last modified: Tue May  2 04:26:41 2023, max compression
```

## Comparing `waveforms-1.5.93.tar` & `waveforms-1.5.94.tar`

### file list

```diff
@@ -1,202 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-28 02:46:20.000000 waveforms-1.5.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 02:46:20.000000 waveforms-1.5.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-28 02:47:16.784312 waveforms-1.5.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 02:46:20.000000 waveforms-1.5.93/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-28 02:46:20.000000 waveforms-1.5.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:47:16.784312 waveforms-1.5.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-28 02:46:20.000000 waveforms-1.5.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.756312 waveforms-1.5.93/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/ikcp.c
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/ikcp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/kcp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/prime.c
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/waveform.c
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-28 02:46:20.000000 waveforms-1.5.93/src/waveform.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.760312 waveforms-1.5.93/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_lisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_scan_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-28 02:46:20.000000 waveforms-1.5.93/tests/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.760312 waveforms-1.5.93/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.764312 waveforms-1.5.93/waveforms/math/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fibheap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.764312 waveforms-1.5.93/waveforms/math/fit/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/qubit_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/resonator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/fit/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.764312 waveforms-1.5.93/waveforms/math/group/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/group/_SU_n_.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/prime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.768312 waveforms-1.5.93/waveforms/math/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/signal/demodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/signal/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/signal/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/math/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.768312 waveforms-1.5.93/waveforms/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.768312 waveforms-1.5.93/waveforms/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.768312 waveforms-1.5.93/waveforms/qlisp/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/prog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.772312 waveforms-1.5.93/waveforms/qlisp/qasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.772312 waveforms-1.5.93/waveforms/qlisp/qasm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/libs/qelib1.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.776312 waveforms-1.5.93/waveforms/qlisp/qasm/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/binaryop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/binaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/creg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/customunitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/expressionlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/gatebody.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/indexedid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/intnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/nodeexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/primarylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/qreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/node/unaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/qasmlexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/qasm/qasmparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.776312 waveforms-1.5.93/waveforms/qlisp/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/simulator/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/simulator/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.780312 waveforms-1.5.93/waveforms/quantum/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.780312 waveforms-1.5.93/waveforms/quantum/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.780312 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.780312 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/arch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/assembly_left.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/assembly_right.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/library.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/qlisp.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.780312 waveforms-1.5.93/waveforms/quantum/circuit/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/circuit/simulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/quantum/clifford/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/clifford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/clifford/clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/clifford/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/clifford/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/clifford/seq2mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/rb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/quantum/xeb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/scan_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/security/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/security/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/server/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/server/umsgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/sys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/sys/device/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/device/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/device/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/sys/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/ipy_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/sys/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/net/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/net/dhcpd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/net/kad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/net/kcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/sys/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/storage/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/sys/storage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/units/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.784312 waveforms-1.5.93/waveforms/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/visualization/plot_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/visualization/plot_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    38227 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-28 02:46:20.000000 waveforms-1.5.93/waveforms/waveform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:47:16.764312 waveforms-1.5.93/waveforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 02:47:16.000000 waveforms-1.5.93/waveforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.726226 waveforms-1.5.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 04:25:46.000000 waveforms-1.5.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 04:25:46.000000 waveforms-1.5.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-02 04:26:41.726226 waveforms-1.5.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-02 04:25:46.000000 waveforms-1.5.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-02 04:25:46.000000 waveforms-1.5.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:26:41.726226 waveforms-1.5.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-02 04:25:46.000000 waveforms-1.5.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.710226 waveforms-1.5.94/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/ikcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/ikcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/kcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/prime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/waveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-02 04:25:46.000000 waveforms-1.5.94/src/waveform.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_scan_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-02 04:25:46.000000 waveforms-1.5.94/tests/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fibheap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms/math/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/qubit_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/resonator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/fit/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms/math/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/group/_SU_n_.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/prime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms/math/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/signal/demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/signal/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/signal/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/math/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/qasm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/libs/qelib1.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.718226 waveforms-1.5.94/waveforms/qlisp/qasm/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/binaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/binaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/creg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/customunitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/expressionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/gatebody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/indexedid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/intnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/nodeexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/primarylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/qreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/node/unaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/qasmlexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/qasm/qasmparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/qlisp/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/simulator/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/simulator/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/arch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/assembly_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/assembly_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/qlisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/circuit/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/circuit/simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/quantum/clifford/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/clifford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/clifford/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/clifford/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/clifford/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/clifford/seq2mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/quantum/xeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/scan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/scan/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/scan/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/scan_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/security/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/server/umsgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23607 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/sys/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/device/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/device/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/sys/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/ipy_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.722226 waveforms-1.5.94/waveforms/sys/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/net/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/net/dhcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/net/kad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/net/kcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.726226 waveforms-1.5.94/waveforms/sys/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/storage/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/sys/storage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.726226 waveforms-1.5.94/waveforms/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.726226 waveforms-1.5.94/waveforms/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/visualization/plot_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/visualization/plot_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-02 04:25:46.000000 waveforms-1.5.94/waveforms/waveform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:26:41.714226 waveforms-1.5.94/waveforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 04:26:41.000000 waveforms-1.5.94/waveforms.egg-info/top_level.txt
```

### Comparing `waveforms-1.5.93/LICENSE` & `waveforms-1.5.94/LICENSE`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/PKG-INFO` & `waveforms-1.5.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.93
+Version: 1.5.94
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.93/README.md` & `waveforms-1.5.94/README.md`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/pyproject.toml` & `waveforms-1.5.94/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/setup.py` & `waveforms-1.5.94/setup.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/ikcp.c` & `waveforms-1.5.94/src/ikcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/ikcp.h` & `waveforms-1.5.94/src/ikcp.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/kcp.c` & `waveforms-1.5.94/src/kcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/prime.c` & `waveforms-1.5.94/src/prime.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/waveform.c` & `waveforms-1.5.94/src/waveform.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/src/waveform.h` & `waveforms-1.5.94/src/waveform.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_compile.py` & `waveforms-1.5.94/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_dicttree.py` & `waveforms-1.5.94/tests/test_dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_lisp.py` & `waveforms-1.5.94/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_msgpack.py` & `waveforms-1.5.94/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_namespace.py` & `waveforms-1.5.94/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_registry.py` & `waveforms-1.5.94/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_scan_iter.py` & `waveforms-1.5.94/tests/test_scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_tomo.py` & `waveforms-1.5.94/tests/test_tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_vm.py` & `waveforms-1.5.94/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/tests/test_waveform.py` & `waveforms-1.5.94/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/__init__.py` & `waveforms-1.5.94/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/autoreload.py` & `waveforms-1.5.94/waveforms/autoreload.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/baseconfig.py` & `waveforms-1.5.94/waveforms/baseconfig.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/cache.py` & `waveforms-1.5.94/waveforms/cache.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/dicttree.py` & `waveforms-1.5.94/waveforms/dicttree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,95 @@
 import copy
 import pickle
 import sys
 from typing import Any, Generator
 
 
-def flattenDictIter(d: dict,
-                    prefix: list = []
-                    ) -> Generator[tuple[str, Any], None, None]:
-    for k in d:
-        if isinstance(d[k], dict):
-            yield from flattenDictIter(d[k], prefix=[*prefix, k])
-        else:
-            yield '.'.join(prefix + [k]), d[k]
-
-
-def flattenDict(d: dict[str, Any]) -> dict[str, Any]:
-    return {k: v for k, v in flattenDictIter(d)}
-
-
-def foldDict(d: dict[str, Any]) -> dict[str, Any]:
-    ret = {}
-    for k, v in d.items():
-        keys = k.split('.')
-        d = ret
-        for key in keys[:-1]:
-            if key not in d:
-                d[key] = dict()
-            d = d[key]
-        d[keys[-1]] = v
-    return ret
-
-
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton,
                                         cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
+class _SELF(metaclass=Singleton):
+    __slots__ = ()
+
+    def __repr__(self):
+        return "self"
+
+
 class _NOTSET(metaclass=Singleton):
     __slots__ = ()
 
     def __repr__(self):
         return 'N/A'
 
 
 class _UNKNOW(metaclass=Singleton):
     __slots__ = ()
 
     def __repr__(self) -> str:
         return "Unknow"
 
 
+class _DELETE(metaclass=Singleton):
+    __slots__ = ()
+
+    def __repr__(self):
+        return 'Delete'
+
+
+SELF = _SELF()
 NOTSET = _NOTSET()
 UNKNOW = _UNKNOW()
+DELETE = _DELETE()
 
 
-class Delete(metaclass=Singleton):
-    __slots__ = ()
+def flattenDictIter(d: dict,
+                    prefix: list = []
+                    ) -> Generator[tuple[str, Any], None, None]:
+    for k in d:
+        if isinstance(d[k], dict):
+            yield from flattenDictIter(d[k], prefix=[*prefix, k])
+        else:
+            yield '.'.join(prefix + [k]), d[k]
 
-    def __repr__(self):
-        return 'Delete'
 
+def flattenDict(d: dict[str, Any]) -> dict[str, Any]:
+    return {k: v for k, v in flattenDictIter(d)}
+
+
+def foldDict(d: dict[str, Any]) -> dict[str, Any]:
+    ret = {}
+
+    for k, v in d.items():
+        keys = k.split('.')
+        d = ret
+        parent = None
 
-DELETE = Delete()
+        for key in keys[:-1]:
+            if not isinstance(d, dict):
+                parent[0][parent[1]] = {SELF: d}
+                d = parent[0][parent[1]]
+            if key not in d:
+                d[key] = dict()
+            parent = d, key
+            d = d[key]
+        if not isinstance(d, dict):
+            parent[0][parent[1]] = {SELF: d}
+            d = parent[0][parent[1]]
+        if keys[-1] in d and isinstance(d[keys[-1]], dict):
+            d[keys[-1]][SELF] = v
+        else:
+            d[keys[-1]] = v
+    return ret
 
 
 class Update():
     __slots__ = ('o', 'n')
 
     def __init__(self, o, n):
         self.o = o
```

### Comparing `waveforms-1.5.93/waveforms/loader.py` & `waveforms-1.5.94/waveforms/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/bayes.py` & `waveforms-1.5.94/waveforms/math/bayes.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fibheap.py` & `waveforms-1.5.94/waveforms/math/fibheap.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/__init__.py` & `waveforms-1.5.94/waveforms/math/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/_fit.py` & `waveforms-1.5.94/waveforms/math/fit/_fit.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/delay.py` & `waveforms-1.5.94/waveforms/math/fit/delay.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/geo.py` & `waveforms-1.5.94/waveforms/math/fit/geo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/qubit_dynamics.py` & `waveforms-1.5.94/waveforms/math/fit/qubit_dynamics.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/readout.py` & `waveforms-1.5.94/waveforms/math/fit/readout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/resonator.py` & `waveforms-1.5.94/waveforms/math/fit/resonator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/simple.py` & `waveforms-1.5.94/waveforms/math/fit/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/fit/spectrum.py` & `waveforms-1.5.94/waveforms/math/fit/spectrum.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/graph.py` & `waveforms-1.5.94/waveforms/math/graph.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/prime.py` & `waveforms-1.5.94/waveforms/math/prime.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/signal/demodulate.py` & `waveforms-1.5.94/waveforms/math/signal/demodulate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/signal/distortion.py` & `waveforms-1.5.94/waveforms/math/signal/distortion.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/math/signal/func.py` & `waveforms-1.5.94/waveforms/math/signal/func.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/namespace.py` & `waveforms-1.5.94/waveforms/namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/arch/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/assembly.py` & `waveforms-1.5.94/waveforms/qlisp/assembly.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/base.py` & `waveforms-1.5.94/waveforms/qlisp/base.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/commands.py` & `waveforms-1.5.94/waveforms/qlisp/commands.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/compiler.py` & `waveforms-1.5.94/waveforms/qlisp/compiler.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/config.py` & `waveforms-1.5.94/waveforms/qlisp/config.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/interpreter.py` & `waveforms-1.5.94/waveforms/qlisp/interpreter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/library.py` & `waveforms-1.5.94/waveforms/qlisp/library.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/libs/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/macro.py` & `waveforms-1.5.94/waveforms/qlisp/macro.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/parse.py` & `waveforms-1.5.94/waveforms/qlisp/parse.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/prog.py` & `waveforms-1.5.94/waveforms/qlisp/prog.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/eval.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/eval.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/exceptions.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/libs/qelib1.inc` & `waveforms-1.5.94/waveforms/qlisp/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/barrier.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/binaryop.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/binaryoperator.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/creg.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/customunitary.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/expressionlist.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/external.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/format.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/gate.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/gatebody.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/id.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/idlist.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/if_.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/indexedid.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/intnode.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/measure.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/node.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/nodeexception.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/opaque.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/prefix.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/primarylist.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/program.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/qreg.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/real.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/reset.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/node/unaryoperator.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/qasm.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/qasmlexer.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/qasm/qasmparser.py` & `waveforms-1.5.94/waveforms/qlisp/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/simulator/__init__.py` & `waveforms-1.5.94/waveforms/qlisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/simulator/mat.py` & `waveforms-1.5.94/waveforms/qlisp/simulator/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/simulator/simple.py` & `waveforms-1.5.94/waveforms/qlisp/simulator/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/tokenize.py` & `waveforms-1.5.94/waveforms/qlisp/tokenize.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/qlisp/utils.py` & `waveforms-1.5.94/waveforms/qlisp/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/clifford/clifford.py` & `waveforms-1.5.94/waveforms/quantum/clifford/clifford.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/clifford/db.py` & `waveforms-1.5.94/waveforms/quantum/clifford/db.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/clifford/mat.py` & `waveforms-1.5.94/waveforms/quantum/clifford/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/clifford/seq2mat.py` & `waveforms-1.5.94/waveforms/quantum/clifford/seq2mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/math.py` & `waveforms-1.5.94/waveforms/quantum/math.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/rb.py` & `waveforms-1.5.94/waveforms/quantum/rb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/tomo.py` & `waveforms-1.5.94/waveforms/quantum/tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/transmon.py` & `waveforms-1.5.94/waveforms/quantum/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/quantum/xeb.py` & `waveforms-1.5.94/waveforms/quantum/xeb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/registry.py` & `waveforms-1.5.94/waveforms/registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/scan_iter.py` & `waveforms-1.5.94/waveforms/scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/security/verify.py` & `waveforms-1.5.94/waveforms/security/verify.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/server/__init__.py` & `waveforms-1.5.94/waveforms/server/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/server/__main__.py` & `waveforms-1.5.94/waveforms/server/__main__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/server/umsgpack.py` & `waveforms-1.5.94/waveforms/server/umsgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/device/basedevice.py` & `waveforms-1.5.94/waveforms/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/device/loader.py` & `waveforms-1.5.94/waveforms/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/device/utils.py` & `waveforms-1.5.94/waveforms/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/drivers/FakeInstrument.py` & `waveforms-1.5.94/waveforms/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/ipy_events.py` & `waveforms-1.5.94/waveforms/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/net/dhcp.py` & `waveforms-1.5.94/waveforms/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/net/dhcpd.py` & `waveforms-1.5.94/waveforms/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/net/kad.py` & `waveforms-1.5.94/waveforms/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/net/kcp.py` & `waveforms-1.5.94/waveforms/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/progress.py` & `waveforms-1.5.94/waveforms/sys/progress.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/storage/crud.py` & `waveforms-1.5.94/waveforms/sys/storage/crud.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/sys/storage/models.py` & `waveforms-1.5.94/waveforms/sys/storage/models.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/units/__init__.py` & `waveforms-1.5.94/waveforms/units/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/visualization/__init__.py` & `waveforms-1.5.94/waveforms/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/visualization/plot_layout.py` & `waveforms-1.5.94/waveforms/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/visualization/plot_seq.py` & `waveforms-1.5.94/waveforms/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms/waveform.py` & `waveforms-1.5.94/waveforms/waveform.py`

 * *Files 2% similar despite different names*

```diff
@@ -992,26 +992,40 @@
                                                       NDIGITS), +inf),
                         seq=(_zero, _one, _zero))
     else:
         return ((step(edge, type=type) << width / 2) -
                 (step(edge, type=type) >> width / 2))
 
 
-def gaussian(width):
-    if width <= 0:
+def gaussian(width, plateau=0.0):
+    if width <= 0 and plateau <= 0.0:
         return zero()
     # width is two times FWHM
     # std_sq2 = width / (4 * np.sqrt(np.log(2)))
     std_sq2 = width / 3.3302184446307908
     # std is set to give total pulse area same as a square
     #std_sq2 = width/np.sqrt(np.pi)
-    return Waveform(bounds=(round(-0.75 * width,
-                                  NDIGITS), round(0.75 * width,
-                                                  NDIGITS), +inf),
-                    seq=(_zero, _basic_wave(GAUSSIAN, std_sq2), _zero))
+    if round(0.5 * plateau, NDIGITS) <= 0.0:
+        return Waveform(bounds=(round(-0.75 * width,
+                                      NDIGITS), round(0.75 * width,
+                                                      NDIGITS), +inf),
+                        seq=(_zero, _basic_wave(GAUSSIAN, std_sq2), _zero))
+    else:
+        return Waveform(bounds=(round(-0.75 * width - 0.5 * plateau,
+                                      NDIGITS), round(-0.5 * plateau, NDIGITS),
+                                round(0.5 * plateau, NDIGITS),
+                                round(0.75 * width + 0.5 * plateau,
+                                      NDIGITS), +inf),
+                        seq=(_zero,
+                             _basic_wave(GAUSSIAN,
+                                         std_sq2,
+                                         shift=-0.5 * plateau), _one,
+                             _basic_wave(GAUSSIAN,
+                                         std_sq2,
+                                         shift=0.5 * plateau), _zero))
 
 
 def cos(w, phi=0):
     if w == 0:
         return const(np.cos(phi))
     if w < 0:
         phi = -phi
@@ -1043,51 +1057,68 @@
         return zero()
     width = 100 / bw
     return Waveform(bounds=(round(-0.5 * width,
                                   NDIGITS), round(0.5 * width, NDIGITS), +inf),
                     seq=(_zero, _basic_wave(SINC, bw), _zero))
 
 
-def cosPulse(width):
+def cosPulse(width, plateau=0.0):
     # cos = _basic_wave(COS, 2*np.pi/width)
     # pulse = _mul(_add(cos, _one), _half)
+    if round(0.5 * plateau, NDIGITS) > 0:
+        return square(plateau + 0.5 * width, edge=0.5 * width, type='cos')
     if width <= 0:
         return zero()
     pulse = ((((), ()), (((COS, 6.283185307179586 / width, 0), ), (1, ))),
              (0.5, 0.5))
     return Waveform(bounds=(round(-0.5 * width,
                                   NDIGITS), round(0.5 * width, NDIGITS), +inf),
                     seq=(_zero, pulse, _zero))
 
 
-def hanning(width):
-    return cosPulse(width)
+def hanning(width, plateau=0.0):
+    return cosPulse(width, plateau=plateau)
 
 
 def cosh(w):
     return Waveform(seq=(_basic_wave(COSH, w), ))
 
 
 def sinh(w):
     return Waveform(seq=(_basic_wave(SINH, w), ))
 
 
-def coshPulse(width, steepness=1.0, plateau=0.0):
-    """
+def coshPulse(width, eps=1.0, plateau=0.0):
+    """Cosine hyperbolic pulse with the following im
+
     pulse edge shape:
-            cosh(w * T / 2) - cosh(w * t)
-    f(t) = -------------------------------
-                cosh(w * T / 2) - 1
-    where T is the pulse width and w = steepness / width
-    plateau is the fraction of the pulse width where the pulse is flat.
+            cosh(eps / 2) - cosh(eps * t / T)
+    f(t) = -----------------------------------
+                  cosh(eps / 2) - 1
+    where T is the pulse width and eps is the pulse edge steepness.
+    The pulse is defined for t in [-T/2, T/2].
+
+    In case of plateau > 0, the pulse is defined as:
+           | f(t + plateau/2)   if t in [-T/2 - plateau/2, - plateau/2]
+    g(t) = | 1                  if t in [-plateau/2, plateau/2]
+           | f(t - plateau/2)   if t in [plateau/2, T/2 + plateau/2]
+
+    Parameters
+    ----------
+    width : float
+        Pulse width.
+    eps : float
+        Pulse edge steepness.
+    plateau : float
+        Pulse plateau.
     """
     if width <= 0 and plateau <= 0:
         return zero()
-    w = steepness / width
-    A = np.cosh(steepness / 2)
+    w = eps / width
+    A = np.cosh(eps / 2)
 
     if plateau == 0.0 or round(-0.5 * plateau, NDIGITS) == round(
             0.5 * plateau, NDIGITS):
         pulse = ((((), ()), (((COSH, w, 0), ), (1, ))), (A / (A - 1),
                                                          -1 / (A - 1)))
         return Waveform(bounds=(round(-0.5 * width,
                                       NDIGITS), round(0.5 * width,
```

### Comparing `waveforms-1.5.93/waveforms/waveform_parser.py` & `waveforms-1.5.94/waveforms/waveform_parser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.93/waveforms.egg-info/PKG-INFO` & `waveforms-1.5.94/waveforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.93
+Version: 1.5.94
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.93/waveforms.egg-info/SOURCES.txt` & `waveforms-1.5.94/waveforms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,17 @@
 waveforms/quantum/circuit/qlisp/arch/base.py
 waveforms/quantum/circuit/simulator/__init__.py
 waveforms/quantum/clifford/__init__.py
 waveforms/quantum/clifford/clifford.py
 waveforms/quantum/clifford/db.py
 waveforms/quantum/clifford/mat.py
 waveforms/quantum/clifford/seq2mat.py
+waveforms/scan/__init__.py
+waveforms/scan/dataset.py
+waveforms/scan/transforms.py
 waveforms/security/__init__.py
 waveforms/security/verify.py
 waveforms/server/__init__.py
 waveforms/server/__main__.py
 waveforms/server/umsgpack.py
 waveforms/sys/__init__.py
 waveforms/sys/chat.py
```

