# Comparing `tmp/merlin-systems-23.2.0.tar.gz` & `tmp/merlin-systems-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-systems-23.2.0.tar", last modified: Wed Mar  8 16:26:55 2023, max compression
+gzip compressed data, was "merlin-systems-23.4.0.tar", last modified: Tue May  2 21:26:48 2023, max compression
```

## Comparing `merlin-systems-23.2.0.tar` & `merlin-systems-23.4.0.tar`

### file list

```diff
@@ -1,80 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-08 16:26:55.827624 merlin-systems-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.815624 merlin-systems-23.2.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.827624 merlin-systems-23.2.0/merlin/systems/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-08 16:26:55.827624 merlin-systems-23.2.0/merlin/systems/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.819624 merlin-systems-23.2.0/merlin/systems/dag/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/dictarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/op_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.819624 merlin-systems-23.2.0/merlin/systems/dag/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/feast.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/fil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/session_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/softmax_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/unroll_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/ops/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.819624 merlin-systems-23.2.0/merlin/systems/dag/runtimes/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/base_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.819624 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.819624 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/fil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/model_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/merlin/systems/triton/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/merlin/systems/triton/models/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/models/executor_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/models/oprunner_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/models/pytorch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/models/workflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/triton/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/merlin/systems/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/workflow/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/workflow/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/merlin/systems/workflow/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/merlin_systems.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-08 16:26:55.000000 merlin-systems-23.2.0/merlin_systems.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-08 16:26:55.000000 merlin-systems-23.2.0/merlin_systems.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:26:55.000000 merlin-systems-23.2.0/merlin_systems.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:24:37.000000 merlin-systems-23.2.0/merlin_systems.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-08 16:26:55.000000 merlin-systems-23.2.0/merlin_systems.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 16:26:55.000000 merlin-systems-23.2.0/merlin_systems.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:26:55.823624 merlin-systems-23.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/test-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/test-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-08 16:26:55.827624 merlin-systems-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-03-08 16:20:16.000000 merlin-systems-23.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.744853 merlin-systems-23.4.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin/systems/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.748853 merlin-systems-23.4.0/merlin/systems/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/feast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18177 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/fil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/session_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/softmax_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/unroll_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/ops/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/base_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/fil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/model_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/triton/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/executor_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/pytorch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/models/workflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/triton/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.752853 merlin-systems-23.4.0/merlin/systems/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/merlin/systems/workflow/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/merlin_systems.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 21:26:48.000000 merlin-systems-23.4.0/merlin_systems.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 21:26:48.756853 merlin-systems-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81388 2023-05-02 21:26:38.000000 merlin-systems-23.4.0/versioneer.py
```

### Comparing `merlin-systems-23.2.0/LICENSE` & `merlin-systems-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/PKG-INFO` & `merlin-systems-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-systems
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/systems
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-systems-23.2.0/README.md` & `merlin-systems-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/__init__.py` & `merlin-systems-23.4.0/merlin/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/__init__.py` & `merlin-systems-23.4.0/merlin/systems/dag/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,11 +12,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # alias submodules here to avoid breaking everything with moving to submodules
 # flake8: noqa
-from .dictarray import Column, DictArray
 from .ensemble import Ensemble
 from .node import Node
-from .op_runner import OperatorRunner
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ensemble.py` & `merlin-systems-23.4.0/merlin/systems/dag/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         the necessary ensemble graph. This will traverse each node of
         the graph and mutate the input according to the operator in each
         node.
 
         Parameters
         ----------
         transformable : Transformable
-            Input data to the graph (DataFrame or DictArray).
+            Input data to the graph (DataFrame or TensorTable).
         runtime : Runtime, optional
             The graph runtime to use to transform the inputs, by default None
 
         Returns
         -------
         Transformable
             transformed data
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/node.py` & `merlin-systems-23.4.0/merlin/systems/dag/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,48 +10,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
+import warnings
 from typing import Union
 
 from merlin.dag import Node
 from merlin.schema import Schema
 
 
 class InferenceNode(Node):
     """Specialized node class used in Triton Ensemble DAGs"""
 
-    def exportable(self, backend: str = None):
-        """
-        Determine whether the current node's operator is exportable for a given back-end
-
-        Parameters
-        ----------
-        backend : str, optional
-            The Merlin Systems (not Triton) back-end to use,
-            either "ensemble" or "executor", by default None
-
-        Returns
-        -------
-        bool
-            True if the node's operator is exportable for the supplied back-end
-        """
-        backends = getattr(self.op, "exportable_backends", [])
-
-        return hasattr(self.op, "export") and backend in backends
-
     def export(
         self,
         output_path: Union[str, os.PathLike],
         node_id: int = None,
         version: int = 1,
-        backend="ensemble",
     ):
         """
         Export a Triton config directory for this node.
 
         Parameters
         ----------
         output_path : Union[str, os.PathLike]
@@ -68,15 +49,14 @@
         """
         return self.op.export(
             output_path,
             self.input_schema,
             self.output_schema,
             node_id=node_id,
             version=version,
-            backend=backend,
         )
 
     @property
     def export_name(self):
         """
         Name for the exported Triton config directory.
 
@@ -113,11 +93,12 @@
             for elem in self.children:
                 childrens_schema += elem.input_schema
 
             for col_name, col_schema in self.output_schema.column_schemas.items():
                 sink_col_schema = childrens_schema.get(col_name)
 
                 if not sink_col_schema:
-                    raise ValueError(
-                        f"Output column '{col_name}' not detected in any "
-                        f"child inputs for '{self.op.__class__.__name__}'."
+                    warnings.warn(
+                        f"Operator '{self.op.__class__.__name__}' is producing the output column "
+                        f"'{col_name}', which is not being used by any downstream operator "
+                        f"in the ensemble graph."
                     )
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/__init__.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,38 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 
-def compute_dims(col_schema, scalar_shape=None):
+def compute_dims(col_schema):
     """
     Compute Triton dimensions for a column from its schema
 
     Parameters
     ----------
     col_schema : ColumnSchema
         Schema of the column to compute dimensions for
-    scalar_shape : List[int], optional
-        The shape of a single scalar element, by default None
 
     Returns
     -------
     List[int]
         Triton dimensions for the column
     """
-    batch_dim = [-1]
+    dims = [-1]
 
-    default_scalar_shape = col_schema.properties.get("triton_scalar_shape", [1])
-    column_dims = scalar_shape if scalar_shape is not None else default_scalar_shape
-    assert isinstance(column_dims, list)
-
-    if col_schema.is_list:
-        column_dims = []
-        for dim in col_schema.shape.dims[1:]:
-            if dim.is_fixed:
-                column_dims.append(dim.max)
-            else:
-                column_dims.append(-1)
+    if col_schema.shape is not None and col_schema.shape.dims is not None:
+        for dim in col_schema.shape.as_tuple[1:]:
+            dim = dim if isinstance(dim, int) else -1
+            dims.append(dim)
 
-    return batch_dim + column_dims
+    return dims
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/compat.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/compat.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/faiss.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/faiss.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-import json
 import os
-import pathlib
 from pathlib import Path
 from shutil import copy2
-from typing import Dict, List, Tuple
 
 import faiss
 import numpy as np
 
 from merlin.core.dispatch import HAS_GPU
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector
@@ -57,136 +53,63 @@
         """
         super().__init__()
 
         self.index_path = str(index_path)
         self.topk = topk
         self._index = None
 
-    def load_artifacts(self, artifact_path):
+    def load_artifacts(self, artifact_path: str) -> None:
         filename = Path(self.index_path).name
         path_artifact = Path(artifact_path)
         if path_artifact.is_file():
             path_artifact = path_artifact.parent
         full_index_path = str(path_artifact / filename)
         index = faiss.read_index(full_index_path)
 
         if HAS_GPU:
             res = faiss.StandardGpuResources()
             index = faiss.index_cpu_to_gpu(res, 0, index)
         self._index = index
 
-    @classmethod
-    def from_config(cls, config: dict, **kwargs) -> "QueryFaiss":
-        """
-        Instantiate a class object given a config.
-
-        Parameters
-        ----------
-        config : dict
-
-
-        Returns
-        -------
-        QueryFaiss
-            class object instantiated with config values
-        """
-        parameters = json.loads(config.get("params", ""))
-        index_path = parameters["index_path"]
-        topk = parameters["topk"]
-
-        operator = QueryFaiss(index_path, topk=topk)
-        operator.load_artifacts(index_path)
-
-        return operator
-
-    @property
-    def exportable_backends(self):
-        return ["ensemble", "executor"]
-
-    def export(
-        self,
-        path: str,
-        input_schema: Schema,
-        output_schema: Schema,
-        params: dict = None,
-        node_id: int = None,
-        version: int = 1,
-        backend: str = "ensemble",
-    ) -> Tuple[Dict, List]:
-        """
-        Export the class object as a config and all related files to the user defined path.
+    def save_artifacts(self, artifact_path: str) -> None:
+        index_filename = os.path.basename(os.path.realpath(self.index_path))
+        new_index_path = Path(artifact_path) / index_filename
+        copy2(self.index_path, new_index_path)
 
-        Parameters
-        ----------
-        path : str
-            Artifact export path
-        input_schema : Schema
-            A schema with information about the inputs to this operator
-        output_schema : Schema
-            A schema with information about the outputs of this operator
-        params : dict, optional
-            Parameters dictionary of key, value pairs stored in exported config, by default None
-        node_id : int, optional
-            The placement of the node in the graph (starts at 1), by default None
-        version : int, optional
-            The version of the model, by default 1
+    def __getstate__(self) -> dict:
+        """Return state of instance when pickled.
 
         Returns
         -------
-        Ensemble_config: dict
-        Node_configs: list
+        dict
+            Returns object state excluding index attribute.
         """
-        params = params or {}
-
-        self_params = {
-            # TODO: Write the (relative) path from inside the export directory
-            "index_path": self.index_path,
-            "topk": self.topk,
-        }
-        self_params.update(params)
-        index_filename = os.path.basename(os.path.realpath(self.index_path))
-
-        if backend == "ensemble":
-            full_path = (
-                pathlib.Path(path) / f"{node_id}_{QueryFaiss.__name__.lower()}" / str(version)
-            )
-        else:
-            full_path = pathlib.Path(path) / "executor_model" / str(version) / "ensemble"
-
-        new_index_path = full_path / index_filename
-        full_path.mkdir(parents=True, exist_ok=True)
-        copy2(self.index_path, new_index_path)
-        self.index_path = str(new_index_path)
-
-        if backend == "ensemble":
-            return super().export(path, input_schema, output_schema, self_params, node_id, version)
-        else:
-            return ({}, [])
+        return {k: v for k, v in self.__dict__.items() if k != "_index"}
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """
         Transform input dataframe to output dataframe using function logic.
 
         Parameters
         ----------
-        df : DictArray
+        df : TensorTable
             Input tensor dictionary, data that will be manipulated
 
         Returns
         -------
-        DictArray
+        TensorTable
             Transformed tensor dictionary
         """
         user_vector = list(transformable.values())[0]
 
         _, indices = self._index.search(user_vector.values, self.topk)
 
-        candidate_ids = np.array(indices).T.astype(np.int32)
+        candidate_ids = np.array(indices).astype(np.int32).flatten()
 
         return type(transformable)({"candidate_ids": candidate_ids})
 
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
@@ -245,42 +168,41 @@
         Returns
         -------
         Schema
             A schema object representing all outputs of this node.
         """
         return Schema(
             [
-                ColumnSchema("candidate_ids", dtype=np.int32),
+                ColumnSchema("candidate_ids", dtype=np.int32, dims=(None, self.topk)),
             ]
         )
 
     def validate_schemas(
         self, parents_schema, deps_schema, input_schema, output_schema, strict_dtypes=False
     ):
         if len(input_schema.column_schemas) > 1:
             raise ValueError(
                 "More than one input has been detected for this node,"
                 / f"inputs received: {input_schema.column_names}"
             )
 
 
-def setup_faiss(item_vector, output_path: str):
+def setup_faiss(item_vector, output_path: str, metric=faiss.METRIC_INNER_PRODUCT):
     """
-    Utiltiy function that will create a Faiss index from an embedding vector. Currently only
-    supports L2 distance.
+    Utiltiy function that will create a Faiss index from a set of embedding vectors
 
     Parameters
     ----------
     item_vector : Numpy.ndarray
         This is a matrix representing all the nodes embeddings, represented as a numpy ndarray.
     output_path : string
         target output path
     """
     ids = item_vector[:, 0].astype(np.int64)
     item_vectors = np.ascontiguousarray(item_vector[:, 1:].astype(np.float32))
 
-    index = faiss.index_factory(item_vectors.shape[1], "IVF32,Flat")
+    index = faiss.index_factory(item_vectors.shape[1], "IVF32,Flat", metric)
     index.nprobe = 8
 
     index.train(item_vectors)
     index.add_with_ids(item_vectors, ids)
     faiss.write_index(index, str(output_path))
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/feast.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/feast.py`

 * *Files 9% similar despite different names*

```diff
@@ -194,31 +194,31 @@
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """
         Transform input dataframe to output dataframe using function logic.
 
         Parameters
         ----------
-        df : DictArray
+        df : TensorTable
             Input tensor dictionary, data that will be manipulated
 
         Returns
         -------
-        DictArray
+        TensorTable
             Transformed tensor dictionary
         """
         entity_ids = transformable[self.entity_column]
-        array_lib = entity_ids._array_lib
+        array_constructor = entity_ids.array_constructor()
 
         if len(entity_ids) < 1:
             raise ValueError(
                 "No entity ids provided when querying Feast. Must provide "
                 "at least one id in order to fetch features."
             )
-        entity_rows = [{self.entity_id: int(entity_id)} for entity_id in entity_ids]
+        entity_rows = [{self.entity_id: int(entity_id)} for entity_id in entity_ids.values]
 
         feature_names = self.features + self.mh_features
         feature_refs = [
             ":".join([self.entity_view, feature_name]) for feature_name in feature_names
         ]
 
         feast_response = self.store.get_online_features(
@@ -231,51 +231,51 @@
             output_tensors[self.entity_id] = entity_ids
 
         # Numerical and single-hot categorical
         for feature_name in self.features:
             prefixed_name = self.__class__._prefixed_name(self.output_prefix, feature_name)
 
             feature_value = feast_response[feature_name]
-            feature_array = array_lib.array([feature_value]).T.astype(
+            feature_array = array_constructor(feature_value).astype(
                 self.output_schema[prefixed_name].dtype.to_numpy
             )
             output_tensors[prefixed_name] = feature_array
 
         # Multi-hot categorical
         for feature_name in self.mh_features:
             feature_value = feast_response[feature_name]
             prefixed_name = self.__class__._prefixed_name(self.output_prefix, feature_name)
 
-            row_lengths = None
+            offsets = None
             if isinstance(feature_value[0], list) and self.output_schema[prefixed_name].is_ragged:
                 # concatenate lists we got back from Feast
                 flattened_value = []
                 for val in feature_value:
                     flattened_value.extend(val)
 
                 # get the lengths of the lists
                 row_lengths = [len(vals) for vals in feature_value]
-
-                # wrap the flattened values with a list to get the shape right
-                feature_value = [flattened_value]
+                offsets = np.cumsum([0] + row_lengths)
+                feature_value = flattened_value
 
             # create a numpy array
-            feature_array = array_lib.array(feature_value).T.astype(
+            feature_array = array_constructor(feature_value).astype(
                 self.output_schema[prefixed_name].dtype.to_numpy
             )
 
             # if we're a list but not ragged, construct row lengths
-            if not row_lengths:
-                row_lengths = [len(feature_array)]
+            if offsets is None:
+                offsets = [0, len(feature_array)]
 
-            feature_row_lengths = array_lib.array(
-                [row_lengths], dtype=self.output_schema[prefixed_name].dtype.to_numpy
-            ).T
+            feature_offsets = array_constructor(
+                offsets, dtype=self.output_schema[prefixed_name].dtype.to_numpy
+            )
 
-            output_tensors[prefixed_name] = (feature_array, feature_row_lengths)
+            output_tensors[f"{prefixed_name}__values"] = feature_array
+            output_tensors[f"{prefixed_name}__offsets"] = feature_offsets
 
         return type(transformable)(output_tensors)
 
     @classmethod
     def _prefixed_name(cls, output_prefix, col_name):
         if output_prefix and col_name and not col_name.startswith(output_prefix):
             return f"{output_prefix}_{col_name}"
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/fil.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/fil.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 
 import numpy as np
 
 from merlin.core.dispatch import HAS_GPU
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector  # noqa
 from merlin.schema import ColumnSchema, Schema  # noqa
-from merlin.systems.dag.dictarray import DictArray
 from merlin.systems.dag.ops.compat import (
     cuml_ensemble,
     cuml_fil,
     lightgbm,
     sklearn_ensemble,
     treelite_model,
     treelite_sklearn,
     xgboost,
 )
 from merlin.systems.dag.ops.operator import InferenceOperator
+from merlin.table import TensorTable
 
 
 class PredictForest(InferenceOperator):
     """Operator for running inference on Forest models.
 
     This works for gradient-boosted decision trees (GBDTs) and Random forests (RF).
     While RF and GBDT algorithms differ in the way they train the models,
@@ -84,77 +84,40 @@
         parents_schema: Schema,
         deps_schema: Schema,
         selector: ColumnSelector,
     ) -> Schema:
         """Return the input schema representing the input columns this operator expects to use."""
         return self.input_schema
 
-    @property
-    def exportable_backends(self):
-        return ["ensemble", "executor"]
-
-    def export(
-        self,
-        path: str,
-        input_schema: Schema,
-        output_schema: Schema,
-        params: dict = None,
-        node_id: int = None,
-        version: int = 1,
-        backend: str = "ensemble",
-    ):
-        """Export the class and related files to the path specified."""
-        fil_model_config = self.fil_op.export(
-            path,
-            input_schema,
-            output_schema,
-            params=params,
-            node_id=node_id,
-            version=version,
-        )
-
-        return fil_model_config
-
-    @property
-    def fil_model_name(self):
-        return self._fil_model_name
-
-    def set_fil_model_name(self, fil_model_name):
-        self._fil_model_name = fil_model_name
-
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """Transform the dataframe by applying this FIL operator to the set of input columns.
 
         Parameters
         -----------
-        df: DictArray
+        df: TensorTable
             A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
-        DictArray
+        TensorTable
             Returns a transformed dataframe for this operator"""
 
         input0 = (
             np.array([column.values.ravel() for column in transformable.values()])
             .astype(np.float32)
             .T
         )
         predictions = self.fil_op.predict(input0).astype(np.float32)
 
         outputs = {"output__0": predictions}
 
         return type(transformable)(outputs)
 
-    def load_artifacts(self, artifact_path):
-        # need variable that tells me what type of model this is.
-        self.fil_op.load_model(artifact_path)
-
 
 class FIL(InferenceOperator):
     """Operator for Forest Inference Library (FIL) models.
 
     Packages up XGBoost models to run on Triton inference server using the fil backend.
     """
 
@@ -261,33 +224,14 @@
         input_schema: Schema,
         col_selector: ColumnSelector,
         prev_output_schema: Schema = None,
     ) -> Schema:
         """Returns output schema for FIL op"""
         return Schema([ColumnSchema("output__0", dtype=np.float32)])
 
-    def export(
-        self,
-        path,
-        input_schema,
-        output_schema,
-        params: dict = None,
-        node_id=None,
-        version=1,
-    ):
-        """Export the model to the supplied path. Returns the config"""
-        node_name = f"{node_id}_{self.export_name}" if node_id is not None else self.export_name
-        node_export_path = pathlib.Path(path) / node_name
-        version_path = node_export_path / str(version)
-        version_path.mkdir(parents=True, exist_ok=True)
-
-        self.fil_model_class.save(version_path)
-
-        return version_path
-
     def load_model(self, version_path):
         version_path = pathlib.Path(version_path)
         self.fil_model_class.load(version_path)
 
     def predict(self, inputs):
         return self.fil_model_class.predict(inputs)
 
@@ -301,14 +245,20 @@
 
     @abstractmethod
     def save(self, version_path):
         """
         Save model to version_path
         """
 
+    @abstractmethod
+    def load(self, version_path):
+        """
+        Load model from path
+        """
+
     @property
     @abstractmethod
     def num_classes(self):
         """
         The number of classes
         """
 
@@ -421,15 +371,15 @@
 
             if num_targets > 1:
                 raise ValueError("Only single target objectives are supported.")
 
             super().__init__(model)
 
     def predict(self, inputs):
-        if isinstance(inputs, DictArray):
+        if isinstance(inputs, TensorTable):
             inputs = inputs.to_df()
         inputs = xgboost.DMatrix(inputs)
         return self.model.predict(inputs)
 
     def save(self, version_path) -> None:
         """Save model to version_path."""
         model_path = pathlib.Path(version_path) / self.model_filename
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/implicit.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/implicit.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,18 @@
         model_module_name = self.model_module_name
         model_class_name = self.model_class_name
         model_module = importlib.import_module(model_module_name)
         model_cls = getattr(model_module, model_class_name)
 
         self.model = model_cls.load(str(model_file))
 
+    def save_artifacts(self, artifact_path: str):
+        model_path = pathlib.Path(artifact_path) / "model.npz"
+        self.model.save(str(model_path))
+
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
         deps_schema: Schema,
         selector: ColumnSelector,
     ) -> Schema:
@@ -81,31 +85,27 @@
         input_schema: Schema,
         col_selector: ColumnSelector,
         prev_output_schema: Schema = None,
     ) -> Schema:
         """Return the output schema representing the columns this operator returns."""
         return Schema([ColumnSchema("ids", dtype="int64"), ColumnSchema("scores", dtype="float64")])
 
-    @property
-    def exportable_backends(self):
-        return ["ensemble", "executor"]
-
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """Transform the dataframe by applying this operator to the set of input columns.
 
         Parameters
         -----------
-        df: DictArray
+        df: TensorTable
             A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
-        DictArray
+        TensorTable
             Returns a transformed dataframe for this operator"""
         user_id = transformable["user_id"].values.ravel()
         user_items = None
         ids, scores = self.model.recommend(
             user_id, user_items, N=self.num_to_recommend, filter_already_liked_items=False
         )
         return type(transformable)(
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/operator.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,38 +50,41 @@
         """
         raise NotImplementedError(
             f"{self.__class__.__name__} does not have a Transform function."
             "Please create one in the operator class, where you inherited "
             "from the base operator."
         )
 
-    def load_artifacts(self, artifact_path):
-        """
-        Hook method that provides a way to load saved artifacts for the operator
+    def load_artifacts(self, artifact_path: str) -> None:
+        """Load artifacts from disk required for operator function.
 
         Parameters
         ----------
         artifact_path : str
-            Path where artifacts for the operator are stored.
+            The path where artifacts are loaded from
         """
 
-    @property
-    def exportable_backends(self):
-        return ["ensemble"]
+    def save_artifacts(self, artifact_path: str) -> None:
+        """Save artifacts required to be reload operator state from disk
+
+        Parameters
+        ----------
+        artifact_path : str
+            The path where artifacts are to be saved
+        """
 
     @abstractmethod
     def export(
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
         """
         Export the class object as a config and all related files to the user defined path.
 
         Parameters
         ----------
         path : str
@@ -95,23 +98,21 @@
         node_id : int, optional
             The placement of the node in the graph (starts at 1), by default None.
         version : int, optional
             The version of the model, by default 1.
 
         Returns
         -------
-        Ensemble_config: dict
-            The config for the entire ensemble.
-        Node_configs: list
-            A list of individual configs for each step (operator) in graph.
+        model_config: dict
+            The config for the exported operator (Triton model).
         """
         raise NotImplementedError(
-            "Exporting an operator to run in a particular context (i.e. Triton)"
-            " only makres sense when a runtime is specified. To select an "
-            f"operator for the appropriate runtime, replace {self.__class__.__name__}"
+            "Exporting an operator to run in a particular context (i.e. Triton) "
+            "only makes sense when a runtime is specified. To select an "
+            f"operator for the appropriate runtime, replace {self.__class__.__name__} "
             f"with a runtime-specific operator class, possibly {self.__class__.__name__}Triton"
         )
 
     def create_node(self, selector: ColumnSelector) -> InferenceNode:
         """_summary_
 
         Parameters
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/pytorch.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/pytorch.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
 
 import numpy as np
-import torch  # noqa
-import torch.utils.dlpack  # noqa
 
-from merlin.core.protocols import Transformable  # noqa
-from merlin.dag import ColumnSelector  # noqa
-from merlin.schema import Schema  # noqa
-from merlin.systems.dag.dictarray import DictArray
-from merlin.systems.dag.ops.operator import InferenceOperator  # noqa
+from merlin.core.compat.torch import torch
+from merlin.core.protocols import Transformable
+from merlin.dag import ColumnSelector
+from merlin.schema import Schema
+from merlin.systems.dag.ops.operator import InferenceOperator
+from merlin.table import TensorTable
 
 
 class PredictPyTorch(InferenceOperator):
     """
     This operator takes a pytorch model and packages it correctly for tritonserver
     to run, on the pytorch backend.
     """
@@ -94,28 +93,28 @@
         """
         Use the output schema supplied during object creation.
         """
         return self.output_schema
 
     def transform(self, col_selector: ColumnSelector, transformable: Transformable):
         output_type = type(transformable)
-        if not isinstance(transformable, DictArray):
-            transformable = DictArray.from_df(transformable)
+        if not isinstance(transformable, TensorTable):
+            transformable = TensorTable.from_df(transformable)
 
         tensor_dict = {}
         for column in transformable.columns:
             tensor_dict[column] = torch.from_numpy(np.squeeze(transformable[column].values))
 
         result = self.model(tensor_dict)
         output = {}
         for idx, col in enumerate(self.output_schema.column_names):
             output[col] = result[:, idx].detach().numpy()
 
-        output = DictArray(output)
+        output = TensorTable(output)
         if not isinstance(output, output_type):
-            output = output.to_df(transformable)
+            output = output.to_df()
 
         return output
 
     @property
     def scalar_shape(self):
         return []
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/session_filter.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/session_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import json
-
 import numpy as np
 
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector, Node
 from merlin.schema import ColumnSchema, Schema
 from merlin.systems.dag.ops.operator import InferenceOperator
 
@@ -46,33 +44,14 @@
             A class object is instantiated with param values passed.
         """
         self.filter_out = Node.construct_from(filter_out)
         self._input_col = input_col
         self._filter_out_col = filter_out
         super().__init__()
 
-    @classmethod
-    def from_config(cls, config, **kwargs) -> "FilterCandidates":
-        """
-        Instantiate a class object given a config.
-
-        Parameters
-        ----------
-        config : dict
-
-
-        Returns
-        -------
-            Class object instantiated with config values
-        """
-        parameters = json.loads(config.get("params", ""))
-        filter_out_col = parameters["filter_out_col"]
-        input_col = parameters["input_col"]
-        return FilterCandidates(filter_out_col, input_col)
-
     @property
     def dependencies(self):
         return self.filter_out
 
     def compute_input_schema(
         self,
         root_schema: Schema,
@@ -165,61 +144,20 @@
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """
         Transform input dataframe to output dataframe using function logic.
 
         Parameters
         ----------
-        df : DictArray
+        df : TensorTable
             Input tensor dictionary, data that will be manipulated
 
         Returns
         -------
-        DictArray
+        TensorTable
             Transformed tensor dictionary
         """
         candidate_ids = transformable[self._input_col]
         filter_ids = transformable[self._filter_out_col]
 
-        filtered_results = candidate_ids[~np.isin(candidate_ids, filter_ids)]
+        filtered_results = candidate_ids.values[~np.isin(candidate_ids.values, filter_ids.values)]
         return type(transformable)({"filtered_ids": filtered_results})
-
-    def export(
-        self,
-        path: str,
-        input_schema: Schema,
-        output_schema: Schema,
-        params: dict = None,
-        node_id: int = None,
-        version: int = 1,
-        backend: str = "ensemble",
-    ):
-        """
-        Export the class object as a config and all related files to the user defined path.
-
-        Parameters
-        ----------
-        path : str
-            Artifact export path
-        input_schema : Schema
-            A schema with information about the inputs to this operator
-        output_schema : Schema
-            A schema with information about the outputs of this operator
-        params : dict, optional
-            Parameters dictionary of key, value pairs stored in exported config, by default None
-        node_id : int, optional
-            The placement of the node in the graph (starts at 1), by default None
-        version : int, optional
-            The version of the model, by default 1
-
-        Returns
-        -------
-        Ensemble_config: dict
-        Node_configs: list
-        """
-        params = params or {}
-        self_params = {
-            "input_col": self._input_col,
-            "filter_out_col": self._filter_out_col,
-        }
-        self_params.update(params)
-        return super().export(path, input_schema, output_schema, self_params, node_id, version)
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/softmax_sampling.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/softmax_sampling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-
 import numpy as np
 
 from merlin.core.protocols import Transformable
 from merlin.dag.node import Node
 from merlin.dag.selector import ColumnSelector
 from merlin.schema import ColumnSchema, Schema
 from merlin.systems.dag.ops.operator import InferenceOperator
@@ -33,52 +31,18 @@
         self.relevance_col = Node.construct_from(relevance_col)
         self.temperature = temperature
         self.topk = topk
         self._input_col_name = _input_col
         self._relevance_col_name = relevance_col
         super().__init__()
 
-    @classmethod
-    def from_config(cls, config, **kwargs) -> "SoftmaxSampling":
-        """Load operator and properties from Triton config"""
-        parameters = json.loads(config.get("params", ""))
-        relevance_col = parameters["relevance_col"]
-        input_col = parameters["input_col"]
-        temperature = parameters["temperature"]
-        topk = parameters["topk"]
-
-        return SoftmaxSampling(
-            relevance_col, temperature=temperature, topk=topk, _input_col=input_col
-        )
-
     @property
     def dependencies(self):
         return self.relevance_col
 
-    def export(
-        self,
-        path: str,
-        input_schema: Schema,
-        output_schema: Schema,
-        params: dict = None,
-        node_id: int = None,
-        version: int = 1,
-        backend: str = "ensemble",
-    ):
-        """Write out a Triton model config directory"""
-        params = params or {}
-        self_params = {
-            "input_col": self._input_col_name,
-            "relevance_col": self._relevance_col_name,
-            "temperature": self.temperature,
-            "topk": self.topk,
-        }
-        self_params.update(params)
-        return super().export(path, input_schema, output_schema, self_params, node_id, version)
-
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
         deps_schema: Schema,
         selector: ColumnSelector,
     ) -> Schema:
@@ -97,16 +61,22 @@
 
     def compute_output_schema(
         self, input_schema: Schema, col_selector: ColumnSelector, prev_output_schema: Schema = None
     ) -> Schema:
         """Describe the operator's outputs"""
         return Schema(
             [
-                ColumnSchema("ordered_ids", dtype=np.int32, dims=(None, 1)),
-                ColumnSchema("ordered_scores", dtype=np.float32, dims=(None, 1)),
+                ColumnSchema(
+                    "ordered_ids", dtype=input_schema[self._input_col_name].dtype, dims=(None, 1)
+                ),
+                ColumnSchema(
+                    "ordered_scores",
+                    dtype=input_schema[self._relevance_col_name].dtype,
+                    dims=(None, 1),
+                ),
             ]
         )
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """Transform the dataframe by applying this operator to the set of input columns"""
@@ -135,13 +105,13 @@
         exponentials = -np.log(np.random.uniform(0, 1, size=(num_items,)))
         exponentials /= weights
 
         # This is just bookkeeping to produce the final ordered list of recs
         sorted_indices = np.argsort(exponentials)
         topk_item_ids = candidate_ids[sorted_indices][: self.topk]
         topk_item_scores = predicted_scores[sorted_indices][: self.topk]
-        ordered_item_ids = topk_item_ids.reshape(1, -1).T
-        ordered_item_scores = topk_item_scores.reshape(1, -1).T
+        ordered_item_ids = topk_item_ids.reshape(1, -1)
+        ordered_item_scores = topk_item_scores.reshape(1, -1)
 
         return type(transformable)(
             {"ordered_ids": ordered_item_ids, "ordered_scores": ordered_item_scores}
         )
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/tensorflow.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/tensorflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,26 +16,27 @@
 import os
 import pathlib
 import tempfile
 
 # this needs to be before any modules that import protobuf
 os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"
 
-import tensorflow as tf  # noqa
-
+from merlin.core.compat.tensorflow import tensorflow as tf  # noqa
 from merlin.core.protocols import Transformable  # noqa
 from merlin.dag import ColumnSelector  # noqa
 from merlin.schema import ColumnSchema, Schema  # noqa
 from merlin.systems.dag.ops.operator import InferenceOperator  # noqa
+from merlin.table import TensorflowColumn, TensorTable  # noqa
+from merlin.table.conversions import convert_col  # noqa
 
 
 class PredictTensorflow(InferenceOperator):
     """TensorFlow Model Prediction Operator."""
 
-    def __init__(self, model_or_path, custom_objects: dict = None, backend="tensorflow"):
+    def __init__(self, model_or_path, custom_objects: dict = None):
         """
         Instantiate a PredictTensorflow inference operator.
 
         Parameters
         ----------
         model_or_path : Tensorflow model or string
             This can be a tensorflow model or a path to a tensorflow model.
@@ -50,15 +51,15 @@
             if isinstance(model_or_path, (str, os.PathLike)):
                 self.path = model_or_path
                 self.model = tf.keras.models.load_model(self.path, custom_objects=custom_objects)
             else:
                 self.path = None
                 self.model = model_or_path
 
-            self.input_schema, self.output_schema = self._construct_schemas_from_model(self.model)
+            self.input_schema, self.output_schema = _construct_schemas_from_model(self.model)
 
     def __getstate__(self) -> dict:
         """Return state of instance when pickled.
 
         Returns
         -------
         dict
@@ -81,36 +82,35 @@
         Returns
         -------
         Transformable
             Model Predictions
         """
         # TODO: Validate that the inputs match the schema
         # TODO: Should we coerce the dtypes to match the schema here?
-        input_tensors = {}
-        for col in transformable.columns:
-            input_tensors[col] = tf.convert_to_tensor(transformable[col].values)
-        outputs = self.model(input_tensors)
+        if not isinstance(transformable, TensorTable):
+            transformable = TensorTable.from_df(transformable)
+
+        col_type = TensorflowColumn
+
+        tf_columns = {
+            col_name: convert_col(column, col_type) for col_name, column in transformable.items()
+        }
+        model_inputs = TensorTable(tf_columns)
+
+        outputs = self.model(model_inputs.to_dict())
+
         dict_outputs = {}
         for col in self.output_schema.column_names:
-            dict_outputs[col] = outputs.numpy()
+            dict_outputs[col] = (
+                outputs[col].numpy() if isinstance(outputs, dict) else outputs.numpy()
+            )
+
         # TODO: map output schema names to outputs produced by prediction
         return type(transformable)(dict_outputs)
 
-    @property
-    def export_name(self):
-        """
-        Provides a clear common english identifier for this operator.
-
-        Returns
-        -------
-        String
-            Name of the current class as spelled in module.
-        """
-        return self.__class__.__name__.lower()
-
     @classmethod
     def from_path(cls, path, **kwargs):
         return cls.__init__(path, **kwargs)
 
     def compute_input_schema(
         self,
         root_schema: Schema,
@@ -127,56 +127,59 @@
         self, input_schema: Schema, col_selector: ColumnSelector, prev_output_schema: Schema = None
     ) -> Schema:
         """
         Use the output schema supplied during object creation.
         """
         return self.output_schema
 
-    def _construct_schemas_from_model(self, model):
-        signatures = getattr(model, "signatures", {}) or {}
-        default_signature = signatures.get("serving_default")
-
-        if not default_signature:
-            # roundtrip saved model to disk to generate signature if it doesn't exist
-            self._ensure_input_spec_includes_names(model)
-
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                tf_model_path = pathlib.Path(tmp_dir) / "model.savedmodel"
-                model.save(tf_model_path, include_optimizer=False)
-                reloaded = tf.keras.models.load_model(tf_model_path)
-                default_signature = reloaded.signatures["serving_default"]
-
-        input_schema = Schema()
-        for col_name, col in default_signature.structured_input_signature[1].items():
-            col_schema = ColumnSchema(col_name, dtype=col.dtype.as_numpy_dtype)
-            if col.shape[1] and col.shape[1] > 1:
-                col_schema = self._set_list_length(col_schema, col.shape[1])
-            input_schema.column_schemas[col_name] = col_schema
-
-        output_schema = Schema()
-        for col_name, col in default_signature.structured_outputs.items():
-            col_schema = ColumnSchema(col_name, dtype=col.dtype.as_numpy_dtype)
-            if col.shape[1] and col.shape[1] > 1:
-                col_schema = self._set_list_length(col_schema, col.shape[1])
-            output_schema.column_schemas[col_name] = col_schema
-
-        return input_schema, output_schema
-
-    def _ensure_input_spec_includes_names(self, model):
-        if isinstance(model._saved_model_inputs_spec, dict):
-            for key, spec in model._saved_model_inputs_spec.items():
-                if isinstance(spec, tuple):
-                    model._saved_model_inputs_spec[key] = (
-                        tf.TensorSpec(shape=spec[0].shape, dtype=spec[0].dtype, name=key),
-                        tf.TensorSpec(shape=spec[1].shape, dtype=spec[1].dtype, name=key),
-                    )
-                else:
-                    model._saved_model_inputs_spec[key] = tf.TensorSpec(
-                        shape=spec.shape, dtype=spec.dtype, name=key
-                    )
-
-        return model
-
-    def _set_list_length(self, col_schema, list_length):
-        return col_schema.with_dtype(
-            col_schema.dtype, is_list=True, is_ragged=False
-        ).with_properties({"value_count": {"min": list_length, "max": list_length}})
+
+def _construct_schemas_from_model(model):
+    signatures = getattr(model, "signatures", {}) or {}
+    default_signature = signatures.get("serving_default")
+
+    if not default_signature:
+        # roundtrip saved model to disk to generate signature if it doesn't exist
+        model = _ensure_input_spec_includes_names(model)
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            tf_model_path = pathlib.Path(tmp_dir) / "model.savedmodel"
+            model.save(tf_model_path, include_optimizer=False)
+            reloaded = tf.keras.models.load_model(tf_model_path)
+            default_signature = reloaded.signatures["serving_default"]
+
+    input_schema = _build_schema_from_signature(default_signature.structured_input_signature[1])
+    output_schema = _build_schema_from_signature(default_signature.structured_outputs)
+
+    return input_schema, output_schema
+
+
+def _ensure_input_spec_includes_names(model):
+    if isinstance(model._saved_model_inputs_spec, dict):
+        for key, spec in model._saved_model_inputs_spec.items():
+            if isinstance(spec, tuple):
+                model._saved_model_inputs_spec[key] = (
+                    tf.TensorSpec(shape=spec[0].shape, dtype=spec[0].dtype, name=key),
+                    tf.TensorSpec(shape=spec[1].shape, dtype=spec[1].dtype, name=key),
+                )
+            else:
+                model._saved_model_inputs_spec[key] = tf.TensorSpec(
+                    shape=spec.shape, dtype=spec.dtype, name=key
+                )
+
+    return model
+
+
+def _build_schema_from_signature(signature):
+    schema = Schema()
+    for col_name, col in signature.items():
+        if "__offsets" in col_name or "__values" in col_name:
+            col_name = col_name.replace("__offsets", "").replace("__values", "")
+            col_values_sig = signature[f"{col_name}__values"]
+            col_offsets_sig = signature[f"{col_name}__offsets"]
+            col_dtype = col_values_sig.dtype.as_numpy_dtype
+            col_dims = (col_offsets_sig.shape[0], None)
+        else:
+            col_dtype = col.dtype.as_numpy_dtype
+            col_dims = col.shape
+        col_schema = ColumnSchema(col_name, dtype=col_dtype, dims=col_dims)
+        schema.column_schemas[col_name] = col_schema
+    return schema
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/unroll_features.py` & `merlin-systems-23.4.0/merlin/systems/dag/ops/workflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,96 +9,105 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import json
-
-import numpy as np
+from typing import List
 
 from merlin.core.protocols import Transformable
-from merlin.dag import Node
-from merlin.dag.selector import ColumnSelector
+from merlin.dag import ColumnSelector
 from merlin.schema import Schema
 from merlin.systems.dag.ops.operator import InferenceOperator
+from merlin.table import TensorTable
 
 
-class UnrollFeatures(InferenceOperator):
+class TransformWorkflow(InferenceOperator):
     """
-    This operator takes a target column and joins the "unroll" columns to the target. This helps
-    when broadcasting a series of user features to a set of items.
+    This operator takes a workflow and turns it into a ensemble operator so that we can
+    execute feature engineering during ensemble on tritonserver.
     """
 
-    def __init__(self, item_id_col, unroll_cols, unrolled_prefix=""):
-        self.item_id_col = item_id_col
-        self.unroll_cols = Node.construct_from(unroll_cols)
-        self.unrolled_prefix = unrolled_prefix
-        super().__init__()
-
-    @classmethod
-    def from_config(cls, config, **kwargs) -> "UnrollFeatures":
-        """Load operator and properties from Triton config"""
-        parameters = json.loads(config.get("params", ""))
-        candidate_col = parameters["item_id_col"]
-        unroll_cols = parameters["unroll_cols"]
-        unrolled_prefix = parameters["unrolled_prefix"]
-        return UnrollFeatures(candidate_col, unroll_cols, unrolled_prefix)
-
-    def export(
+    def __init__(
         self,
-        path: str,
-        input_schema: Schema,
-        output_schema: Schema,
-        params: dict = None,
-        node_id: int = None,
-        version: int = 1,
-        backend: str = "ensemble",
+        workflow=None,
+        sparse_max: dict = None,
+        max_batch_size: int = None,
+        label_columns: List[str] = None,
+        cats: List[str] = None,
+        conts: List[str] = None,
     ):
-        """Write out a Triton model config directory"""
-        params = params or {}
-        self_params = {
-            "item_id_col": self.item_id_col,
-            "unroll_cols": self._unroll_col_names,
-            "unrolled_prefix": self.unrolled_prefix,
-        }
-        self_params.update(params)
-        return super().export(path, input_schema, output_schema, self_params, node_id, version)
+        """
+        Creates a Transform Workflow operator for a target workflow.
+
+        Parameters
+        ----------
+        workflow : Nvtabular.Workflow
+            The workflow to transform data in ensemble.
+        sparse_max : dict, optional
+            Dictionary representing key(name)/val(max value) pairs of max sparsity, by default None
+        max_batch_size : int, optional
+            Maximum batch size, by default None
+        label_columns : List[str], optional
+            List of strings identifying the label columns, by default None
+        cats : List[str], optional
+            List of strings identifying categorical columns, by default None
+        conts : List[str], optional
+            List of string identifying continuous columns, by default None
+        """
+        super().__init__()
+
+        self.workflow = workflow
+        if label_columns:
+            self.workflow = workflow.remove_inputs(label_columns)
+        self._nvt_model_name = None
+        self.sparse_max = sparse_max or {}
+        self.max_batch_size = max_batch_size
+        self.label_columns = label_columns or []
+        self.cats = cats or []
+        self.conts = conts or []
+
+        if self.workflow is not None:
+            self.input_schema = self.workflow.input_schema
+            self.output_schema = self.workflow.output_schema
 
     @property
-    def dependencies(self):
-        return self.unroll_cols
+    def nvt_model_name(self):
+        return self._nvt_model_name
+
+    def set_nvt_model_name(self, nvt_model_name):
+        self._nvt_model_name = nvt_model_name
 
     def compute_output_schema(
         self, input_schema: Schema, col_selector: ColumnSelector, prev_output_schema: Schema = None
     ) -> Schema:
-        schema = super().compute_output_schema(input_schema, col_selector, prev_output_schema)
-
-        for col_name, col_schema in self.unroll_cols.output_schema.column_schemas.items():
-            schema.column_schemas.pop(col_name, None)
-            col_name = f"{self.unrolled_prefix}_{col_name}" if self.unrolled_prefix else col_name
-            schema[col_name] = col_schema.with_name(col_name)
-
-        return schema
+        """Returns output schema of operator"""
+        return self.workflow.output_schema
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
-        num_items = transformable[self.item_id_col].shape[0]
-        outputs = {}
-        for col_name, col_value in transformable.items():
-            outputs[col_name] = col_value
-
-        for col in self._unroll_col_names:
-            target = outputs.pop(col)
-            col_name = f"{self.unrolled_prefix}_{col}" if self.unrolled_prefix else col
-            outputs[col_name] = np.repeat(target, num_items, axis=0)
+        """Run nvtabular workflow transformations.
 
-        return type(transformable)(outputs)
+        Parameters
+        ----------
+        col_selector : ColumnSelector
+            Unused ColumunSelector input
+        transformable : Transformable
+            Input features to model
+
+        Returns
+        -------
+        Transformable
+            workflow transform
+        """
+        output_type = type(transformable)
+        if isinstance(transformable, TensorTable):
+            transformable = transformable.to_df()
 
-    @property
-    def _unroll_col_names(self):
-        if self.unroll_cols.selector:
-            return self.unroll_cols.selector.names
-        else:
-            return self.unroll_cols.output_columns.names
+        output = self.workflow._transform_df(transformable)
+
+        if not isinstance(output, output_type):
+            output = TensorTable.from_df(output)
+
+        return output
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/ops/workflow.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/operator.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,124 +9,114 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import List
+from abc import ABCMeta, abstractmethod
+
+import tritonclient.grpc.model_config_pb2 as model_config
 
 from merlin.core.protocols import Transformable
-from merlin.dag import ColumnSelector
+from merlin.dag.selector import ColumnSelector
 from merlin.schema import Schema
-from merlin.systems.dag.dictarray import DictArray
 from merlin.systems.dag.ops.operator import InferenceOperator
+from merlin.systems.triton.export import _convert_dtype
 
 
-class TransformWorkflow(InferenceOperator):
-    """
-    This operator takes a workflow and turns it into a ensemble operator so that we can
-    execute feature engineering during ensemble on tritonserver.
-    """
+class TritonOperator(InferenceOperator, metaclass=ABCMeta):
+    """Base class for Triton operators."""
 
-    def __init__(
-        self,
-        workflow=None,
-        sparse_max: dict = None,
-        max_batch_size: int = None,
-        label_columns: List[str] = None,
-        model_framework: str = None,
-        cats: List[str] = None,
-        conts: List[str] = None,
-        backend: str = "workflow",
-    ):
-        """
-        Creates a Transform Workflow operator for a target workflow.
+    def __init__(self, base_op: InferenceOperator):
+        """Construct TritonOperator from a base operator.
 
         Parameters
         ----------
-        workflow : Nvtabular.Workflow
-            The workflow to transform data in ensemble.
-        sparse_max : dict, optional
-            Dictionary representing key(name)/val(max value) pairs of max sparsity, by default None
-        max_batch_size : int, optional
-            Maximum batch size, by default None
-        label_columns : List[str], optional
-            List of strings identifying the label columns, by default None
-        model_framework : str, optional
-            String representing the target framework
-            (supported: hugectr, tensorflow, pytorch, python), by default None
-        cats : List[str], optional
-            List of strings identifying categorical columns, by default None
-        conts : List[str], optional
-            List of string identifying continuous columns, by default None
+        base_op : merlin.systems.dag.ops.operator.InfereneOperator
+            Base operator used to construct this Triton op.
         """
         super().__init__()
-
-        self.workflow = workflow
-        if label_columns:
-            self.workflow = workflow.remove_inputs(label_columns)
-        self._nvt_model_name = None
-        self.sparse_max = sparse_max or {}
-        self.max_batch_size = max_batch_size
-        self.label_columns = label_columns or []
-        self.model_framework = model_framework or ""
-        self.cats = cats or []
-        self.conts = conts or []
-
-        if self.workflow is not None:
-            self.input_schema = self.workflow.input_schema
-            self.output_schema = self.workflow.output_schema
+        self.op = base_op
 
     @property
-    def nvt_model_name(self):
-        return self._nvt_model_name
-
-    def set_nvt_model_name(self, nvt_model_name):
-        self._nvt_model_name = nvt_model_name
+    def export_name(self):
+        """
+        Provides a clear common english identifier for this operator.
 
-    def compute_output_schema(
-        self, input_schema: Schema, col_selector: ColumnSelector, prev_output_schema: Schema = None
-    ) -> Schema:
-        """Returns output schema of operator"""
-        return self.workflow.output_schema
+        Returns
+        -------
+        String
+            Name of the current class as spelled in module.
+        """
+        return self.__class__.__name__.lower()
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
-        """Run nvtabular workflow transformations.
+        """Transform the dataframe by applying this operator to the set of input columns
 
         Parameters
-        ----------
-        col_selector : ColumnSelector
-            Unused ColumunSelector input
-        transformable : Transformable
-            Input features to model
+        -----------
+        df: Dataframe
+            A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
-        Transformable
-            workflow transform
+        DataFrame
+            Returns a transformed dataframe for this operator
         """
-        output_type = type(transformable)
-        if isinstance(transformable, DictArray):
-            transformable = transformable.to_df()
-
-        output = self.workflow._transform_df(transformable)
-
-        if not isinstance(output, output_type):
-            output = DictArray().from_df(output)
-
-        return output
+        return transformable
 
+    @abstractmethod
     def export(
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
-        """Create a directory inside supplied path based on our export name"""
-        raise NotImplementedError
+        """
+        Export the Operator to as a Triton Model at the path corresponding to the model repository.
+
+        Parameters
+        ----------
+        path : str
+            Artifact export path
+        input_schema : Schema
+            A schema with information about the inputs to this operator.
+        output_schema : Schema
+            A schema with information about the outputs of this operator.
+        params : dict, optional
+            Parameters dictionary of key, value pairs stored in exported config, by default None.
+        node_id : int, optional
+            The placement of the node in the graph (starts at 1), by default None.
+        version : int, optional
+            The version of the model, by default 1.
+
+        Returns
+        -------
+        model_config: ModelConfig
+            The config for the operator (model) if defined.
+        """
+
+
+def add_model_param(params, paramclass, col_schema, dims=None):
+    if col_schema.is_list and col_schema.is_ragged:
+        params.append(
+            paramclass(
+                name=col_schema.name + "__values",
+                data_type=_convert_dtype(col_schema.dtype),
+                dims=dims[1:],
+            )
+        )
+        params.append(
+            paramclass(
+                name=col_schema.name + "__offsets", data_type=model_config.TYPE_INT32, dims=[-1]
+            )
+        )
+    else:
+        params.append(
+            paramclass(name=col_schema.name, data_type=_convert_dtype(col_schema.dtype), dims=dims)
+        )
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/__init__.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/base_runtime.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/base_runtime.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/__init__.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/__init__.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/fil.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/fil.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import json
 import pathlib
 
 import numpy as np
 import tritonclient.grpc.model_config_pb2 as model_config  # noqa
 from google.protobuf import text_format  # noqa
 
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector  # noqa
-from merlin.schema import ColumnSchema, Schema  # noqa
-from merlin.systems.dag import DictArray
+from merlin.schema import Schema  # noqa
 from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator  # noqa
 from merlin.systems.triton.conversions import (
-    dict_array_to_triton_request,
-    triton_response_to_dict_array,
+    tensor_table_to_triton_request,
+    triton_response_to_tensor_table,
 )
+from merlin.table import TensorTable
 
 
 class PredictForestTriton(TritonOperator):
     """Operator for running inference on Forest models.
 
     This works for gradient-boosted decision trees (GBDTs) and Random forests (RF).
     While RF and GBDT algorithms differ in the way they train the models,
@@ -91,15 +90,14 @@
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
         """Export the class and related files to the path specified."""
         fil_model_config = self.fil_op.export(
             path,
             input_schema,
             output_schema,
             params=params,
@@ -112,74 +110,51 @@
         return super().export(
             path,
             input_schema,
             output_schema,
             params=params,
             node_id=node_id,
             version=version,
-            backend=self.backend,
         )
 
-    @classmethod
-    def from_config(cls, config: dict, **kwargs) -> "PredictForestTriton":
-        """Instantiate the class from a dictionary representation.
-
-        Expected structure:
-        {
-            "input_dict": str  # JSON dict with input names and schemas
-            "params": str  # JSON dict with params saved at export
-        }
-
-        """
-        column_schemas = [
-            ColumnSchema(name, **schema_properties)
-            for name, schema_properties in json.loads(config["input_dict"]).items()
-        ]
-        input_schema = Schema(column_schemas)
-        cls_instance = cls(None, input_schema)
-        params = json.loads(config["params"])
-        model_name = params["fil_model_name"]
-        cls_instance.set_fil_model_name(model_name)
-        return cls_instance
-
     @property
     def fil_model_name(self):
         return self._fil_model_name
 
     def set_fil_model_name(self, fil_model_name):
         self._fil_model_name = fil_model_name
 
     def transform(
         self, col_selector: ColumnSelector, transformable: Transformable
     ) -> Transformable:
         """Transform the dataframe by applying this FIL operator to the set of input columns.
 
         Parameters
         -----------
-        df: DictArray
+        df: TensorTable
             A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
-        DictArray
+        TensorTable
             Returns a transformed dataframe for this operator"""
 
         input0 = (
             np.array([column.values.ravel() for column in transformable.values()])
             .astype(np.float32)
             .T
         )
 
-        inputs = DictArray({"input__0": input0})
+        inputs = TensorTable({"input__0": input0})
 
-        inference_request = dict_array_to_triton_request(
+        inference_request = tensor_table_to_triton_request(
             self.fil_model_name, inputs, ["input__0"], ["output__0"]
         )
         inference_response = inference_request.exec()
-        return triton_response_to_dict_array(inference_response, type(inputs), ["output__0"])
+        return triton_response_to_tensor_table(inference_response, type(inputs), ["output__0"])
 
 
 class FILTriton(TritonOperator):
     """Operator for Forest Inference Library (FIL) models.
 
     Packages up XGBoost models to run on Triton inference server using the fil backend.
     """
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/implicit.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/pytorch.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,177 +9,190 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import importlib
-import json
+import os
 import pathlib
+from shutil import copyfile
 
-import numpy as np
+import tritonclient.grpc.model_config_pb2 as model_config  # noqa
+from google.protobuf import text_format  # noqa
 
-from merlin.core.protocols import Transformable
-from merlin.dag import ColumnSelector
-from merlin.schema import ColumnSchema, Schema
+from merlin.core.protocols import Transformable  # noqa
+from merlin.dag import ColumnSelector  # noqa
+from merlin.schema import Schema  # noqa
+from merlin.systems.dag.ops import compute_dims  # noqa
+from merlin.systems.dag.runtimes.triton.ops.operator import add_model_param  # noqa
 from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator
-
-try:
-    import implicit
-    from packaging.version import Version
-
-    if Version(implicit.__version__) < Version("0.6.0"):
-        raise RuntimeError(
-            "Implicit version 0.6.0 or higher required. (for model save/load methods)."
-        )
-except ImportError:
-    implicit = None
+from merlin.systems.triton.conversions import (  # noqa
+    tensor_table_to_triton_request,
+    triton_response_to_tensor_table,
+)
 
 
-class PredictImplicitTriton(TritonOperator):
-    """Operator for running inference on Implicit models.."""
+class PredictPyTorchTriton(TritonOperator):
+    """
+    This operator takes a pytorch model and packages it correctly for tritonserver
+    to run, on the pytorch backend.
+    """
 
     def __init__(self, op):
-        """Instantiate an Implicit prediction operator.
+        """
+        Instantiate a PredictPyTorch inference operator.
 
         Parameters
         ----------
-        model : An Implicit Model instance
-        num_to_recommend : int
-           the number of items to return
+        model_or_path : PyTorch model or string
+            This can be a pytorch model or a path to a pytorch model.
+        input_schema : Schema
+            Input schema for the pytorch model. This could be the output schema of the NVTabular
+            workflow that produced your training data.
+        output_schema : Schema
+            Output schema for the pytorch model.
         """
+
         super().__init__(op)
-        if op:
-            self.model = op.model
-            self.model_module_name: str = self.model.__module__
-            self.model_class_name: str = self.model.__class__.__name__
-            self.num_to_recommend = op.num_to_recommend
-
-    def __getstate__(self):
-        return {k: v for k, v in self.__dict__.items() if k != "model"}
-
-    def load_artifacts(self, artifact_path: str):
-        model_file = pathlib.Path(artifact_path) / "model.npz"
-
-        model_module_name = self.model_module_name
-        model_class_name = self.model_class_name
-        model_module = importlib.import_module(model_module_name)
-        model_cls = getattr(model_module, model_class_name)
+        self._torch_model_name = None
+        self.input_schema = op.input_schema
+        self.output_schema = op.output_schema
+
+    @property
+    def torch_model_name(self):
+        return self._torch_model_name
+
+    def set_torch_model_name(self, torch_model_name):
+        """
+        Set the name of the Triton model to use
+
+        Parameters
+        ----------
+        torch_model_name : str
+            Triton model directory name
+        """
+        self._torch_model_name = torch_model_name
+
+    def transform(self, col_selector: ColumnSelector, transformable: Transformable):
+        inference_request = tensor_table_to_triton_request(
+            self.torch_model_name,
+            transformable,
+            self.input_schema.column_names,
+            self.output_schema.column_names,
+        )
 
-        self.model = model_cls.load(str(model_file))
+        inference_response = inference_request.exec()
+
+        return triton_response_to_tensor_table(
+            inference_response, type(transformable), self.output_schema.column_names
+        )
 
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
         deps_schema: Schema,
         selector: ColumnSelector,
     ) -> Schema:
-        """Return the input schema representing the input columns this operator expects to use."""
-        return Schema([ColumnSchema("user_id", dtype="int64")])
+        """
+        Use the input schema supplied during object creation.
+        """
+        return self.input_schema
 
     def compute_output_schema(
-        self,
-        input_schema: Schema,
-        col_selector: ColumnSelector,
-        prev_output_schema: Schema = None,
+        self, input_schema: Schema, col_selector: ColumnSelector, prev_output_schema: Schema = None
     ) -> Schema:
-        """Return the output schema representing the columns this operator returns."""
-        return Schema([ColumnSchema("ids", dtype="int64"), ColumnSchema("scores", dtype="float64")])
-
-    @property
-    def exportable_backends(self):
-        return ["ensemble", "executor"]
+        """
+        Use the output schema supplied during object creation.
+        """
+        return self.output_schema
 
     def export(
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
-        """Export the class and related files to the path specified."""
-        node_name = f"{node_id}_{self.export_name}" if node_id is not None else self.export_name
-
-        if backend == "ensemble":
-            artifact_path = pathlib.Path(path) / node_name / str(version)
-        else:
-            artifact_path = pathlib.Path(path) / "executor_model" / str(version) / "ensemble"
-
-        artifact_path.mkdir(parents=True, exist_ok=True)
-        model_path = artifact_path / "model.npz"
-        self.model.save(str(model_path))
-
-        if backend == "ensemble":
-            params = params or {}
-            params["model_module_name"] = self.model.__module__
-            params["model_class_name"] = self.model.__class__.__name__
-            params["num_to_recommend"] = self.num_to_recommend
-            return super().export(
-                path,
-                input_schema,
-                output_schema,
-                params=params,
-                node_id=node_id,
-                version=version,
+        """Create a directory inside supplied path based on our export name"""
+        export_name = self.__class__.__name__.lower()
+        node_name = f"{node_id}_{export_name}" if node_id is not None else export_name
+
+        node_export_path = pathlib.Path(path) / node_name
+        node_export_path.mkdir(exist_ok=True)
+
+        export_model_path = pathlib.Path(node_export_path) / str(version)
+        export_model_path.mkdir(exist_ok=True)
+
+        if self.op.path:
+            copyfile(
+                str(self.op.path),
+                export_model_path / "model.pt",
             )
         else:
-            return ({}, [])
+            self.op.model.save(export_model_path / "model.pt")
+
+        self.set_torch_model_name(node_name)
+        backend_model_config = self._export_model_config(node_name, node_export_path)
+        return backend_model_config
 
-    @classmethod
-    def from_config(cls, config: dict, **kwargs) -> "PredictImplicitTriton":
-        """Instantiate the class from a dictionary representation.
-
-        Expected config structure:
-        {
-            "input_dict": str  # JSON dict with input names and schemas
-            "params": str  # JSON dict with params saved at export
-        }
-
-        """
-        params = json.loads(config["params"])
-
-        model_repository = kwargs["model_repository"]
-        model_name = kwargs["model_name"]
-        model_version = kwargs["model_version"]
-
-        # load implicit model
-        cls_instance = cls(None)
-        model_module_name = params["model_module_name"]
-        model_class_name = params["model_class_name"]
-        model_module = importlib.import_module(model_module_name)
-        model_cls = getattr(model_module, model_class_name)
-        model_file = pathlib.Path(model_repository) / model_name / str(model_version) / "model.npz"
-        cls_instance.model_module_name = model_module_name
-        cls_instance.model_class_name = model_class_name
-        cls_instance.model = model_cls.load(str(model_file))
-
-        cls_instance.num_to_recommend = params["num_to_recommend"]
-
-        return cls_instance
-
-    def transform(
-        self, col_selector: ColumnSelector, transformable: Transformable
-    ) -> Transformable:
-        """Transform the dataframe by applying this operator to the set of input columns.
+    def _export_model_config(self, name, output_path):
+        """Exports a PyTorch model for serving with Triton
 
         Parameters
-        -----------
-        df: DictArray
-            A pandas or cudf dataframe that this operator will work on
-
-        Returns
-        -------
-        DictArray
-            Returns a transformed dataframe for this operator"""
-        user_id = transformable["user_id"].values.ravel()
-        user_items = None
-        ids, scores = self.model.recommend(
-            user_id, user_items, N=self.num_to_recommend, filter_already_liked_items=False
-        )
-        return type(transformable)(
-            {"ids": ids.astype(np.int64), "scores": scores.astype(np.float64)}
+        ----------
+        name:
+            The name of the triton model to export
+        output_path:
+            The path to write the exported model to
+        """
+        config = self._export_torchscript_config(name, output_path)
+
+        return config
+
+    def _export_torchscript_config(self, name, output_path):
+        """Exports a PyTorch model for serving with Triton
+
+        Parameters
+        ----------
+        name:
+            The name of the triton model to export
+        output_path:
+            The path to write the exported model to
+        """
+        config = model_config.ModelConfig(
+            name=name,
+            instance_group=[
+                model_config.ModelInstanceGroup(kind=model_config.ModelInstanceGroup.Kind.KIND_AUTO)
+            ],
         )
+
+        config.backend = "pytorch"
+        config.platform = "pytorch_libtorch"
+        config.parameters["INFERENCE_MODE"].string_value = "true"
+
+        for _, col_schema in self.input_schema.column_schemas.items():
+            add_model_param(
+                config.input,
+                model_config.ModelInput,
+                col_schema,
+                compute_dims(col_schema),
+            )
+
+        for _, col_schema in self.output_schema.column_schemas.items():
+            add_model_param(
+                config.output,
+                model_config.ModelOutput,
+                col_schema,
+                compute_dims(col_schema),
+            )
+
+        with open(os.path.join(output_path, "config.pbtxt"), "w", encoding="utf-8") as o:
+            text_format.PrintMessage(config, o)
+        return config
+
+    @property
+    def scalar_shape(self):
+        return []
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/operator.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/runtime.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,212 +10,220 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import importlib.resources
-import json
 import os
 import pathlib
-from abc import abstractmethod
 from shutil import copyfile
-from typing import List
+from typing import List, Tuple
 
 import tritonclient.grpc.model_config_pb2 as model_config
 from google.protobuf import text_format
 
-from merlin.core.protocols import Transformable
-from merlin.dag.selector import ColumnSelector
-from merlin.schema import Schema
+from merlin.dag import postorder_iter_nodes
 from merlin.systems.dag.ops import compute_dims
-from merlin.systems.dag.ops.operator import InferenceOperator
-from merlin.systems.triton.export import _convert_dtype
+from merlin.systems.dag.ops.compat import (
+    cuml_ensemble,
+    lightgbm,
+    sklearn_ensemble,
+    treelite_sklearn,
+    xgboost,
+)
+from merlin.systems.dag.ops.workflow import TransformWorkflow
+from merlin.systems.dag.runtimes import Runtime
+from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator, add_model_param
+from merlin.systems.dag.runtimes.triton.ops.workflow import TransformWorkflowTriton
+
+tensorflow = None
+try:
+    from nvtabular.loader.tf_utils import configure_tensorflow
+
+    # everything tensorflow related must be imported after this.
+    configure_tensorflow()
+    import tensorflow
+except ImportError:
+    ...
+
+torch = None
+try:
+    import torch
+except ImportError:
+    ...
+
+
+TRITON_OP_TABLE = {}
+TRITON_OP_TABLE[TransformWorkflow] = TransformWorkflowTriton
+
+if cuml_ensemble or lightgbm or sklearn_ensemble or treelite_sklearn or xgboost:
+    from merlin.systems.dag.ops.fil import PredictForest
+    from merlin.systems.dag.runtimes.triton.ops.fil import PredictForestTriton
+
+    TRITON_OP_TABLE[PredictForest] = PredictForestTriton
+
+if tensorflow:
+    from merlin.systems.dag.ops.tensorflow import PredictTensorflow
+    from merlin.systems.dag.runtimes.triton.ops.tensorflow import PredictTensorflowTriton
+
+    TRITON_OP_TABLE[PredictTensorflow] = PredictTensorflowTriton
+
+if torch:
+    from merlin.systems.dag.ops.pytorch import PredictPyTorch
+    from merlin.systems.dag.runtimes.triton.ops.pytorch import PredictPyTorchTriton
+
+    TRITON_OP_TABLE[PredictPyTorch] = PredictPyTorchTriton
+
+
+class TritonExecutorRuntime(Runtime):
+    """Runtime for Triton.
+    This will run the DAG in a single Triton model and call out to other
+    Triton models for nodes that use any non-python backends.
+    """
 
+    def __init__(self):
+        super().__init__()
+        self.op_table = TRITON_OP_TABLE
+
+    def export(
+        self, ensemble, path: str, version: int = 1, name: str = None
+    ) -> Tuple[model_config.ModelConfig, List[model_config.ModelConfig]]:
+        """Exports an 'Ensemble' as a Triton model repository.
 
-class TritonOperator(InferenceOperator):
-    """Base class for Triton operators."""
+        All operators in the ensemble will run in a single python backend model except
+        those that have a non-python Triton backend.
 
-    def __init__(self, base_op: InferenceOperator):
-        """Construct TritonOperator from a base operator.
+        The entrypoint is the model with name `name`, by default "executor_model"
 
         Parameters
         ----------
-        base_op : merlin.systems.dag.ops.operator.InfereneOperator
-            Base operator used to construct this Triton op.
-        """
-        super().__init__()
-        self.op = base_op
-
-    @property
-    def export_name(self):
-        """
-        Provides a clear common english identifier for this operator.
+        ensemble : merlin.systems.dag.Ensemble
+            Systems ensemble to export
+        path : str
+            Path to directory where Triton model repository will be created.
+        version : int, optional
+            Version for Triton models created, by default 1
+        name : str, optional
+            The name of the ensemble triton model, by default "executor_model"
 
         Returns
         -------
-        String
-            Name of the current class as spelled in module.
+        Tuple[model_config.ModelConfig, List[model_config.ModelConfig]]
+            Tuple of ensemble config and list of non-python backend model configs
         """
-        return self.__class__.__name__.lower()
+        triton_model_name = name or "executor_model"
 
-    @property
-    def exportable_backends(self) -> List[str]:
-        """Returns list of supported backends.
+        nodes = list(postorder_iter_nodes(ensemble.graph.output_node))
 
-        Returns
-        -------
-        List[str]
-            List of supported backends
-        """
-        return ["ensemble", "executor"]
+        for node in nodes:
+            if type(node.op) in self.op_table:
+                node.op = self.op_table[type(node.op)](node.op)
 
-    @classmethod
-    @abstractmethod
-    def from_config(cls, config: dict, **kwargs):
-        """
-        Instantiate a class object given a config.
+        node_id_table, _ = _create_node_table(nodes)
 
-        Parameters
-        ----------
-        config : dict
-        **kwargs
-          contains the following:
-            * model_repository: Model repository path
-            * model_version: Model version
-            * model_name: Model name
+        # Path were extra files can be optionally saved by operators
+        # that don't save all state in operator when pickled
+        artifact_path = pathlib.Path(path) / triton_model_name / str(version) / "ensemble"
+        artifact_path.mkdir(parents=True, exist_ok=True)
 
-        Returns
-        -------
-            Class object instantiated with config values
-        """
+        node_configs = []
+        for node in nodes:
+            node_id = node_id_table.get(node, None)
+            if node_id is not None:
+                node_config = node.export(path, node_id=node_id, version=version)
+                if node_config is not None:
+                    node_configs.append(node_config)
 
-    @abstractmethod
-    def transform(
-        self, col_selector: ColumnSelector, transformable: Transformable
-    ) -> Transformable:
-        """Transform the dataframe by applying this operator to the set of input columns
+            if hasattr(node.op, "save_artifacts"):
+                node.op.save_artifacts(str(artifact_path))
 
-        Parameters
-        -----------
-        df: Dataframe
-            A pandas or cudf dataframe that this operator will work on
+        executor_config = self._executor_model_export(path, triton_model_name, ensemble)
 
-        Returns
-        -------
-        DataFrame
-            Returns a transformed dataframe for this operator
-        """
-        return transformable
+        return (executor_config, node_configs)
 
-    def export(
+    def _executor_model_export(
         self,
         path: str,
-        input_schema: Schema,
-        output_schema: Schema,
+        export_name: str,
+        ensemble,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "python",
-    ):
-        """
-        Export the class object as a config and all related files to the user-defined path.
+    ) -> model_config.ModelConfig:
+        """Export the ensemble and all related files to the  path.
 
         Parameters
         ----------
         path : str
             Artifact export path
-        input_schema : Schema
-            A schema with information about the inputs to this operator.
-        output_schema : Schema
-            A schema with information about the outputs of this operator.
+        export_name : str
+            The name for the Triton model to export to.
+        ensemble : merlin.systems.dag.Ensemble
+            The ensemble to export.
         params : dict, optional
             Parameters dictionary of key, value pairs stored in exported config, by default None.
         node_id : int, optional
             The placement of the node in the graph (starts at 1), by default None.
         version : int, optional
             The version of the model, by default 1.
 
         Returns
         -------
-        Ensemble_config: dict
-            The config for the entire ensemble.
-        Node_configs: list
-            A list of individual configs for each step (operator) in graph.
+        model_config.ModelConfig
+            The config for the ensemble.
         """
 
         params = params or {}
 
-        node_name = f"{node_id}_{self.export_name}" if node_id is not None else self.export_name
+        node_name = f"{node_id}_{export_name}" if node_id is not None else export_name
 
         node_export_path = pathlib.Path(path) / node_name
         node_export_path.mkdir(parents=True, exist_ok=True)
 
-        config = model_config.ModelConfig(name=node_name, backend=backend, platform="op_runner")
-
-        config.parameters["operator_names"].string_value = json.dumps([node_name])
-
-        config.parameters[node_name].string_value = json.dumps(
-            {
-                "module_name": self.__class__.__module__,
-                "class_name": self.__class__.__name__,
-                "input_dict": json.dumps(_schema_to_dict(input_schema)),
-                "output_dict": json.dumps(_schema_to_dict(output_schema)),
-                "params": json.dumps(params),
-            }
+        config = model_config.ModelConfig(
+            name=node_name,
+            backend="python",
+            platform="merlin_executor",
+            instance_group=[
+                model_config.ModelInstanceGroup(kind=model_config.ModelInstanceGroup.Kind.KIND_AUTO)
+            ],
         )
 
+        input_schema = ensemble.input_schema
+        output_schema = ensemble.output_schema
+
         for col_schema in input_schema.column_schemas.values():
             col_dims = compute_dims(col_schema)
             add_model_param(config.input, model_config.ModelInput, col_schema, col_dims)
 
         for col_schema in output_schema.column_schemas.values():
             col_dims = compute_dims(col_schema)
             add_model_param(config.output, model_config.ModelOutput, col_schema, col_dims)
 
         with open(os.path.join(node_export_path, "config.pbtxt"), "w", encoding="utf-8") as o:
             text_format.PrintMessage(config, o)
 
         os.makedirs(node_export_path, exist_ok=True)
         os.makedirs(os.path.join(node_export_path, str(version)), exist_ok=True)
         with importlib.resources.path(
-            "merlin.systems.triton.models", "oprunner_model.py"
-        ) as oprunner_model:
+            "merlin.systems.triton.models", "executor_model.py"
+        ) as executor_model:
             copyfile(
-                oprunner_model,
+                executor_model,
                 os.path.join(node_export_path, str(version), "model.py"),
             )
 
+        ensemble.save(os.path.join(node_export_path, str(version), "ensemble"))
+
         return config
 
 
-def _schema_to_dict(schema: Schema) -> dict:
-    # TODO: Write the conversion
-    schema_dict = {}
-    for col_name, col_schema in schema.column_schemas.items():
-        schema_dict[col_name] = {
-            "dtype": col_schema.dtype.name,
-            "is_list": col_schema.is_list,
-            "is_ragged": col_schema.is_ragged,
-        }
-
-    return schema_dict
-
-
-def add_model_param(params, paramclass, col_schema, dims=None):
-    if col_schema.is_list and col_schema.is_ragged:
-        params.append(
-            paramclass(
-                name=col_schema.name + "__values",
-                data_type=_convert_dtype(col_schema.dtype),
-                dims=dims,
-            )
-        )
-        params.append(
-            paramclass(
-                name=col_schema.name + "__lengths", data_type=model_config.TYPE_INT32, dims=dims
-            )
-        )
-    else:
-        params.append(
-            paramclass(name=col_schema.name, data_type=_convert_dtype(col_schema.dtype), dims=dims)
-        )
+def _create_node_table(nodes):
+    exportable_node_idx = 0
+    node_id_lookup = {}
+    for node in nodes:
+        if isinstance(node.op, TritonOperator):
+            node_id_lookup[node] = exportable_node_idx
+            exportable_node_idx += 1
+
+    return node_id_lookup, exportable_node_idx
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/tensorflow.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from merlin.core.protocols import Transformable  # noqa
 from merlin.dag import ColumnSelector  # noqa
 from merlin.schema import Schema  # noqa
 from merlin.systems.dag.ops import compute_dims  # noqa
 from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator  # noqa
 from merlin.systems.dag.runtimes.triton.ops.operator import add_model_param  # noqa
 from merlin.systems.triton.conversions import (  # noqa
-    dict_array_to_triton_request,
-    triton_response_to_dict_array,
+    tensor_table_to_triton_request,
+    triton_response_to_tensor_table,
 )
 
 
 class PredictTensorflowTriton(TritonOperator):
     """TensorFlow Model Prediction Operator for running inside Triton."""
 
     def __init__(self, op):
@@ -64,36 +64,35 @@
         Returns
         -------
         Transformable
             TensorFlow Model Outputs
         """
         # TODO: Validate that the inputs match the schema
         # TODO: Should we coerce the dtypes to match the schema here?
-        inference_request = dict_array_to_triton_request(
+        inference_request = tensor_table_to_triton_request(
             self.tf_model_name,
             transformable,
             self.input_schema.column_names,
             self.output_schema.column_names,
         )
         inference_response = inference_request.exec()
 
         # TODO: Validate that the outputs match the schema
-        return triton_response_to_dict_array(
+        return triton_response_to_tensor_table(
             inference_response, type(transformable), self.output_schema.column_names
         )
 
     def export(
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
         """Create a directory inside supplied path based on our export name"""
         # Export Triton TF back-end directory and config etc
         export_name = self.__class__.__name__.lower()
         node_name = f"{node_id}_{export_name}" if node_id is not None else export_name
 
         node_export_path = pathlib.Path(path) / node_name
@@ -123,34 +122,39 @@
             The tensorflow model that should be served
         name:
             The name of the triton model to export
         output_path:
             The path to write the exported model to
         """
         config = model_config.ModelConfig(
-            name=name, backend="tensorflow", platform="tensorflow_savedmodel"
+            name=name,
+            backend="tensorflow",
+            platform="tensorflow_savedmodel",
+            instance_group=[
+                model_config.ModelInstanceGroup(kind=model_config.ModelInstanceGroup.Kind.KIND_AUTO)
+            ],
         )
 
         config.parameters["TF_GRAPH_TAG"].string_value = "serve"
         config.parameters["TF_SIGNATURE_DEF"].string_value = "serving_default"
 
         for _, col_schema in self.input_schema.column_schemas.items():
             add_model_param(
                 config.input,
                 model_config.ModelInput,
                 col_schema,
-                compute_dims(col_schema, self.scalar_shape),
+                compute_dims(col_schema),
             )
 
         for _, col_schema in self.output_schema.column_schemas.items():
             add_model_param(
                 config.output,
                 model_config.ModelOutput,
                 col_schema,
-                compute_dims(col_schema, self.scalar_shape),
+                compute_dims(col_schema),
             )
 
         with open(os.path.join(output_path, "config.pbtxt"), "w", encoding="utf-8") as o:
             text_format.PrintMessage(config, o)
         return config
 
     @property
```

### Comparing `merlin-systems-23.2.0/merlin/systems/dag/runtimes/triton/ops/workflow.py` & `merlin-systems-23.4.0/merlin/systems/dag/runtimes/triton/ops/workflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 from google.protobuf import text_format
 
 from merlin.core.protocols import Transformable
 from merlin.dag import ColumnSelector
 from merlin.schema import ColumnSchema, Schema
 from merlin.systems.dag.runtimes.triton.ops.operator import TritonOperator
 from merlin.systems.triton.conversions import (
-    dict_array_to_triton_request,
-    triton_response_to_dict_array,
+    tensor_table_to_triton_request,
+    triton_response_to_tensor_table,
 )
-from merlin.systems.triton.export import _add_model_param, _convert_dtype
+from merlin.systems.triton.export import _add_model_param
 
 
 class TransformWorkflowTriton(TritonOperator):
     """
     This operator takes a workflow and turns it into a ensemble operator so that we can
     execute feature engineering during ensemble on tritonserver.
     """
@@ -50,17 +50,14 @@
             The workflow to transform data in ensemble.
         sparse_max : dict, optional
             Dictionary representing key(name)/val(max value) pairs of max sparsity, by default None
         max_batch_size : int, optional
             Maximum batch size, by default None
         label_columns : List[str], optional
             List of strings identifying the label columns, by default None
-        model_framework : str, optional
-            String representing the target framework
-            (supported: hugectr, tensorflow, pytorch, python), by default None
         cats : List[str], optional
             List of strings identifying categorical columns, by default None
         conts : List[str], optional
             List of string identifying continuous columns, by default None
         """
         super().__init__(op)
 
@@ -71,41 +68,52 @@
             self.output_schema = op.workflow.output_schema
 
     def transform(self, col_selector: ColumnSelector, transformable: Transformable):
         """Transform the dataframe by applying this FIL operator to the set of input columns.
 
         Parameters
         -----------
-        df: DictArray
+        df: TensorTable
             A pandas or cudf dataframe that this operator will work on
 
         Returns
         -------
-        DictArray
+        TensorTable
             Returns a transformed dataframe for this operator"""
-        inference_request = dict_array_to_triton_request(
+
+        output_names = []
+        for col in self.output_schema:
+            if col.is_ragged:
+                output_names.append(f"{col.name}__values")
+                output_names.append(f"{col.name}__offsets")
+            else:
+                output_names.append(col.name)
+
+        inference_request = tensor_table_to_triton_request(
             self._nvt_model_name,
             transformable,
             self.input_schema.column_names,
-            self.output_schema.column_names,
+            output_names,
         )
 
         inference_response = inference_request.exec()
 
         # check inference response for errors:
         if inference_response.has_error():
             # Cannot raise inference response error because it is not derived from BaseException
             raise tritonclient.utils.InferenceServerException(
                 str(inference_response.error().message())
             )
 
-        return triton_response_to_dict_array(
-            inference_response, type(transformable), self.output_schema.column_names
+        response_table = triton_response_to_tensor_table(
+            inference_response, type(transformable), output_names
         )
 
+        return response_table
+
     @classmethod
     def from_config(cls, config: dict, **kwargs) -> "TransformWorkflowTriton":
         """Instantiate the class from a dictionary representation.
 
         Expected structure:
         {
             "input_dict": str  # JSON dict with input names and schemas
@@ -154,15 +162,14 @@
         self,
         path: str,
         input_schema: Schema,
         output_schema: Schema,
         params: dict = None,
         node_id: int = None,
         version: int = 1,
-        backend: str = "ensemble",
     ):
         """Create a directory inside supplied path based on our export name"""
         modified_workflow = self.op.workflow.remove_inputs(self.op.label_columns)
         export_name = self.__class__.__name__.lower()
         node_name = f"{node_id}_{export_name}" if node_id is not None else export_name
         self.set_nvt_model_name(node_name)
         node_export_path = pathlib.Path(path) / node_name
@@ -182,15 +189,14 @@
 
 
 def _generate_nvtabular_model(
     workflow,
     name,
     output_path,
     version=1,
-    output_model=None,
     max_batch_size=None,
     sparse_max=None,
     backend="python",
     cats=None,
     conts=None,
 ):
     """converts a workflow to a triton mode
@@ -204,15 +210,14 @@
         Names of the continuous columns
     """
     workflow.save(os.path.join(output_path, str(version), "workflow"))
     config = _generate_nvtabular_config(
         workflow,
         name,
         output_path,
-        output_model,
         max_batch_size,
         sparse_max=sparse_max,
         backend=backend,
         cats=cats,
         conts=conts,
     )
 
@@ -229,74 +234,47 @@
     return config
 
 
 def _generate_nvtabular_config(
     workflow,
     name,
     output_path,
-    output_model=None,
     max_batch_size=None,
     sparse_max=None,
     backend="python",
     cats=None,
     conts=None,
 ):
     """given a workflow generates the trton modelconfig proto object describing the inputs
     and outputs to that workflow"""
-    config = model_config.ModelConfig(name=name, backend=backend, max_batch_size=max_batch_size)
+    config = model_config.ModelConfig(
+        name=name,
+        backend=backend,
+        max_batch_size=max_batch_size,
+        instance_group=[
+            model_config.ModelInstanceGroup(kind=model_config.ModelInstanceGroup.Kind.KIND_AUTO)
+        ],
+    )
 
     config.parameters["python_module"].string_value = "merlin.systems.triton.models.workflow_model"
-    config.parameters["output_model"].string_value = output_model if output_model else ""
 
     config.parameters["cats"].string_value = json.dumps(cats) if cats else ""
     config.parameters["conts"].string_value = json.dumps(conts) if conts else ""
 
     if sparse_max:
         # this assumes seq_length is same for each list column
         config.parameters["sparse_max"].string_value = json.dumps(sparse_max)
 
-    if output_model == "hugectr":
-        config.instance_group.append(model_config.ModelInstanceGroup(kind=2))
-
-        for column in workflow.output_node.input_columns.names:
-            dtype = workflow.input_dtypes[column]
-            config.input.append(
-                model_config.ModelInput(name=column, data_type=_convert_dtype(dtype), dims=[-1])
-            )
+    for col_name, col_schema in workflow.input_schema.column_schemas.items():
+        _add_model_param(col_schema, model_config.ModelInput, config.input)
 
-        config.output.append(
-            model_config.ModelOutput(name="DES", data_type=model_config.TYPE_FP32, dims=[-1])
-        )
-
-        config.output.append(
-            model_config.ModelOutput(name="CATCOLUMN", data_type=model_config.TYPE_INT64, dims=[-1])
-        )
-
-        config.output.append(
-            model_config.ModelOutput(name="ROWINDEX", data_type=model_config.TYPE_INT32, dims=[-1])
-        )
-    elif output_model == "pytorch":
-        for col_name, col_schema in workflow.input_schema.column_schemas.items():
-            _add_model_param(col_schema, model_config.ModelInput, config.input)
-
-        for col_name, col_schema in workflow.output_schema.column_schemas.items():
-            _add_model_param(
-                col_schema,
-                model_config.ModelOutput,
-                config.output,
-                [-1, 1],
-            )
-    else:
-        for col_name, col_schema in workflow.input_schema.column_schemas.items():
-            _add_model_param(col_schema, model_config.ModelInput, config.input)
-
-        for col_name, col_schema in workflow.output_schema.column_schemas.items():
-            if sparse_max and col_name in sparse_max.keys():
-                # this assumes max_sequence_length is equal for all output columns
-                dim = sparse_max[col_name]
-                _add_model_param(col_schema, model_config.ModelOutput, config.output, [-1, dim])
-            else:
-                _add_model_param(col_schema, model_config.ModelOutput, config.output)
+    for col_name, col_schema in workflow.output_schema.column_schemas.items():
+        if sparse_max and col_name in sparse_max.keys():
+            # this assumes max_sequence_length is equal for all output columns
+            dim = sparse_max[col_name]
+            _add_model_param(col_schema, model_config.ModelOutput, config.output, [-1, dim])
+        else:
+            _add_model_param(col_schema, model_config.ModelOutput, config.output)
 
     with open(os.path.join(output_path, "config.pbtxt"), "w", encoding="utf-8") as o:
         text_format.PrintMessage(config, o)
     return config
```

### Comparing `merlin-systems-23.2.0/merlin/systems/model_registry.py` & `merlin-systems-23.4.0/merlin/systems/model_registry.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/__init__.py` & `merlin-systems-23.4.0/merlin/systems/triton/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,62 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import json
 import os
 
-import numpy as np
 import pandas as pd
 
 # this needs to be before any modules that import protobuf
 os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"
 
 import tritonclient.grpc as grpcclient  # noqa
 from tritonclient.utils import np_to_triton_dtype  # noqa
 
+import merlin.dtypes as md  # noqa
 from merlin.core.dispatch import is_string_dtype, make_df  # noqa
 from merlin.systems.dag.ops import compute_dims  # noqa
+from merlin.table import NumpyColumn, TensorTable  # noqa
+
+
+def convert_table_to_triton_input(schema, batch, input_class=grpcclient.InferInput, dtype="int32"):
+    """
+    Convert a dataframe to a set of Triton inputs
+
+    Parameters
+    ----------
+    schema : Schema
+        Schema of the input data
+    batch : TensorTable
+        The input data itself
+    input_class : Triton input class, optional
+        The Triton input class to use, by default grpcclient.InferInput
+    dtype : str, optional
+        The dtype for lengths/offsets values, by default "int32"
+
+    Returns
+    -------
+    List[input_class]
+        A list of Triton inputs of the requested input class
+    """
+    cpu_table = batch.cpu()
+
+    numpy_cols = {}
+    for col_name, col_values in cpu_table.items():
+        np_col = NumpyColumn(col_values) if not isinstance(col_values, NumpyColumn) else col_values
+        numpy_cols[col_name] = np_col
+    numpy_table = TensorTable(numpy_cols)
+
+    inputs = []
+    for col_name, col_values in numpy_table.to_dict().items():
+        triton_input = _convert_array_to_triton_input(col_name, col_values, input_class)
+        inputs.append(triton_input)
+
+    return inputs
 
 
 def convert_df_to_triton_input(schema, batch, input_class=grpcclient.InferInput, dtype="int32"):
     """
     Convert a dataframe to a set of Triton inputs
 
     Parameters
@@ -46,57 +83,24 @@
     Returns
     -------
     List[input_class]
         A list of Triton inputs of the requested input class
     """
     df_dict = _convert_df_to_dict(schema, batch, dtype)
     inputs = [
-        _convert_column_to_triton_input(col_name, col_values, input_class)
+        _convert_array_to_triton_input(col_name, col_values, input_class)
         for col_name, col_values in df_dict.items()
     ]
     return inputs
 
 
-def _convert_df_to_dict(schema, batch, dtype="int32"):
-    df_dict = {}
-    for col_name, col_schema in schema.column_schemas.items():
-        col = batch[col_name]
-        shape = compute_dims(col_schema)
-        shape[0] = len(col)
-
-        if col_schema.is_list:
-            if isinstance(col, pd.Series):
-                raise ValueError("this function doesn't support CPU list values yet")
-
-            if col_schema.is_ragged:
-                df_dict[col_name + "__values"] = col.list.leaves.values_host.astype(
-                    col_schema.dtype.to_numpy
-                )
-                offsets = col._column.offsets.values_host.astype(dtype)
-                row_lengths = offsets[1:] - offsets[:-1]
-                df_dict[col_name + "__lengths"] = row_lengths
-            else:
-                values = col.list.leaves.values_host
-                values = values.reshape(*shape).astype(col_schema.dtype.to_numpy)
-                df_dict[col_name] = values
-
-        else:
-            values = col.values if isinstance(col, pd.Series) else col.values_host
-            values = values.reshape(*shape).astype(col_schema.dtype.to_numpy)
-            df_dict[col_name] = values
-    return df_dict
-
-
-def _convert_column_to_triton_input(col_name, col_values, input_class=grpcclient.InferInput):
+def _convert_array_to_triton_input(col_name, col_values, input_class=grpcclient.InferInput):
     # Triton's mapping of numpy types to Triton types doesn't know how to handle string types,
     # so we need to map them to object ourselves before we call np_to_triton_dtype
-    col_dtype = col_values.dtype
-    if isinstance(col_dtype, type(np.dtype("str"))):
-        col_dtype = np.dtype("O")
-
+    col_dtype = md.dtype(col_values.dtype).to_numpy
     dtype = np_to_triton_dtype(col_dtype)
     input_tensor = input_class(col_name, col_values.shape, dtype)
 
     # set_data_from_numpy checks the type against what was supplied when we created the tensor
     # using np_to_triton_dtype, so the workaround above isn't enough to make them match here.
     # Do one last `astype` cast to make absolutely sure the dtypes match.
     col_values = col_values.astype(col_dtype)
@@ -146,7 +150,36 @@
     out = t.as_numpy()
     if len(out.shape) == 2:
         out = out[:, 0]
     # cudf doesn't seem to handle dtypes like |S15 or object that well
     if is_string_dtype(out.dtype):
         out = out.astype("str")
     return out
+
+
+def _convert_df_to_dict(schema, batch, dtype="int32"):
+    df_dict = {}
+    for col_name, col_schema in schema.column_schemas.items():
+        col = batch[col_name]
+        shape = compute_dims(col_schema)
+        shape[0] = len(col)
+
+        if col_schema.is_list:
+            if isinstance(col, pd.Series):
+                raise ValueError("this function doesn't support CPU list values yet")
+
+            if col_schema.is_ragged:
+                df_dict[col_name + "__values"] = col.list.leaves.values_host.astype(
+                    col_schema.dtype.to_numpy
+                )
+                offsets = col._column.offsets.values_host.astype(dtype)
+                df_dict[col_name + "__offsets"] = offsets
+            else:
+                values = col.list.leaves.values_host
+                values = values.reshape(*shape).astype(col_schema.dtype.to_numpy)
+                df_dict[col_name] = values
+
+        else:
+            values = col.values if isinstance(col, pd.Series) else col.values_host
+            values = values.reshape(*shape).astype(col_schema.dtype.to_numpy)
+            df_dict[col_name] = values
+    return df_dict
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/conversions.py` & `merlin-systems-23.4.0/merlin/systems/triton/conversions.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,143 +22,151 @@
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 # OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import itertools
 
-try:
-    import cudf
-    import cupy as cp
-except ImportError:
-    cudf = cp = None
-
 import numpy as np
 import pandas as pd
 
+from merlin.core.compat import cudf
+from merlin.core.compat import cupy as cp
 from merlin.core.dispatch import build_cudf_list_column, is_list_dtype
 from merlin.dag import Supports
-from merlin.systems.dag import DictArray
 from merlin.systems.dag.ops.compat import pb_utils
+from merlin.table import TensorTable
 
 
-def triton_request_to_dict_array(request, column_names):
+def triton_request_to_tensor_table(request, column_names):
     """
-    Turns a Triton request into a DictArray by extracting individual tensors
+    Turns a Triton request into a TensorTable by extracting individual tensors
     from the request using pb_utils.
 
     Parameters
     ----------
     request : TritonInferenceRequest
         The incoming request for predictions
     column_names : List[str]
         List of the input columns to extract from the request
 
     Returns
     -------
-    DictArray
+    TensorTable
         Dictionary-like representation of the input columns
     """
     dict_inputs = {}
     for name in column_names:
         try:
             values = _array_from_triton_tensor(request, f"{name}__values")
-            lengths = _array_from_triton_tensor(request, f"{name}__lengths")
+            lengths = _array_from_triton_tensor(request, f"{name}__offsets")
             dict_inputs[name] = (values, lengths)
         except (AttributeError, ValueError):
             dict_inputs[name] = _array_from_triton_tensor(request, name)
 
-    return DictArray(dict_inputs)
+    return TensorTable(dict_inputs)
 
 
-def dict_array_to_triton_response(dictarray):
+def tensor_table_to_triton_response(tensor_table):
     """
-    Turns a DictArray into a Triton response that can be returned
+    Turns a TensorTable into a Triton response that can be returned
     to resolve an incoming request.
 
     Parameters
     ----------
-    dictarray : DictArray
+    tensor_table : TensorTable
         Dictionary-like representation of the output columns
 
     Returns
     -------
     response : TritonInferenceResponse
         The output response for predictions
     """
     output_tensors = []
-    for name, column in dictarray.items():
-        if column.is_ragged:
+    for name, column in tensor_table.items():
+        if column.offsets is not None:
             values = _triton_tensor_from_array(f"{name}__values", column.values)
-            lengths = _triton_tensor_from_array(f"{name}__lengths", column.row_lengths)
-            output_tensors.extend([values, lengths])
+            offsets = _triton_tensor_from_array(f"{name}__offsets", column.offsets)
+            output_tensors.extend([values, offsets])
         else:
             col_tensor = _triton_tensor_from_array(name, column.values)
             output_tensors.append(col_tensor)
 
     return pb_utils.InferenceResponse(output_tensors)
 
 
-def dict_array_to_triton_request(model_name, dictarray, input_col_names, output_col_names):
+def tensor_table_to_triton_request(model_name, tensor_table, input_col_names, output_col_names):
     """
-    Turns a DictArray into a Triton request that can, for example, be used to make a
+    Turns a TensorTable into a Triton request that can, for example, be used to make a
     Business Logic Scripting call to a Triton model on the same Triton instance.
 
     Parameters
     ----------
     model_name : String
         Name of model registered in triton
-    dictarray : DictArray
+    tensor_table : TensorTable
         Dictionary-like representation of the output columns
     input_col_names : List[str]
         List of the input columns to create triton request
     output_col_names : List[str]
         List of the output columns to extract from the response
 
     Returns
     -------
     TritonInferenceRequest
-        The DictArray reformatted as a Triton request
+        The TensorTable reformatted as a Triton request
     """
     input_tensors = []
 
-    for name, column in dictarray.items():
+    for name, column in tensor_table.items():
         if name in input_col_names:
-            col_tensor = _triton_tensor_from_array(name, column.values)
-            input_tensors.append(col_tensor)
+            if column.offsets is not None:
+                values = _triton_tensor_from_array(f"{name}__values", column.values)
+                offsets = _triton_tensor_from_array(f"{name}__offsets", column.offsets)
+                input_tensors.extend([values, offsets])
+            else:
+                col_tensor = _triton_tensor_from_array(name, column.values)
+                input_tensors.append(col_tensor)
 
     return pb_utils.InferenceRequest(
         model_name=model_name,
         requested_output_names=output_col_names,
         inputs=input_tensors,
     )
 
 
-def triton_response_to_dict_array(response, transformable_type, output_column_names):
+def triton_response_to_tensor_table(response, transformable_type, output_column_names):
     """
-    Turns a Triton response into a DictArray by extracting individual tensors
+    Turns a Triton response into a TensorTable by extracting individual tensors
     from the request using pb_utils.
 
     Parameters
     ----------
     response : pb_utils.InferenceResponse
         Response received from triton containing prediction
-    transformable_type : Union[pd.DataFrame, cudf.DataFrame, DictArray]
+    transformable_type : Union[pd.DataFrame, cudf.DataFrame, TensorTable]
         The specific type of object matching the Transformable protocol to create
     output_col_names : List[str]
         List of the output columns to extract from the response
 
     Returns
     -------
     Transformable
-        A DictArray or DataFrame representing the response columns from a Triton request
+        A TensorTable or DataFrame representing the response columns from a Triton request
     """
     outputs_dict = {}
 
     for out_col_name in output_column_names:
+        try:
+            values = _array_from_triton_tensor(response, f"{out_col_name}__values")
+            lengths = _array_from_triton_tensor(response, f"{out_col_name}__offsets")
+            outputs_dict[out_col_name] = (values, lengths)
+        except (AttributeError, ValueError):
+            outputs_dict[out_col_name] = _array_from_triton_tensor(response, out_col_name)
+
         output_val = _array_from_triton_tensor(response, out_col_name)
         outputs_dict[out_col_name] = output_val
 
     return transformable_type(outputs_dict)
 
 
 def _triton_tensor_from_array(name, array):
@@ -228,15 +236,15 @@
         if kind == Supports.GPU_DICT_ARRAY:
             return _convert_array(tensors, cp.asnumpy), Supports.CPU_DICT_ARRAY
         elif kind == Supports.CPU_DATAFRAME:
             return _pandas_to_array(tensors, True), Supports.CPU_DICT_ARRAY
         elif kind == Supports.GPU_DATAFRAME:
             return _cudf_to_array(tensors, True), Supports.CPU_DICT_ARRAY
 
-    elif target_kind & Supports.GPU_DATAFRAME:
+    elif cudf and target_kind & Supports.GPU_DATAFRAME:
         if kind == Supports.CPU_DATAFRAME:
             return cudf.DataFrame(tensors), Supports.GPU_DATAFRAME
         return _array_to_cudf(tensors), Supports.GPU_DATAFRAME
 
     elif target_kind & Supports.CPU_DATAFRAME:
         if kind == Supports.GPU_DATAFRAME:
             return tensors.to_pandas(), Supports.CPU_DATAFRAME
@@ -282,33 +290,42 @@
 def _pandas_to_array(df, cpu=True):
     array_type = np.array if cpu else cp.array
 
     output = {}
     for name in df.columns:
         col = df[name]
         if pd.api.types.is_list_like(col.values[0]):
-            offsets = pd.Series([0]).append(col.map(len).cumsum()).values
-            if not cpu:
-                offsets = cp.array(offsets)
             values = array_type(list(itertools.chain(*col)))
-            output[name] = (values, offsets)
+            row_lengths = col.map(len)
+            if all(row_lengths == row_lengths[0]):
+                output[name] = values.reshape((-1, row_lengths[0]))
+            else:
+                offsets = pd.Series([0]).append(row_lengths.cumsum()).values
+                if not cpu:
+                    offsets = cp.array(offsets)
+                output[name] = (values, offsets)
         else:
             values = col.values
             if not cpu:
                 values = cp.array(values)
             output[name] = values
 
     return output
 
 
 def _cudf_to_array(df, cpu=True):
     output = {}
     for name in df.columns:
         col = df[name]
         if is_list_dtype(col.dtype):
-            offsets = col._column.offsets.values_host if cpu else col._column.offsets.values
             values = col.list.leaves.values_host if cpu else col.list.leaves.values
-            output[name] = (values, offsets)
+            offsets = col._column.offsets.values_host if cpu else col._column.offsets.values
+
+            row_lengths = offsets[1:] - offsets[:-1]
+            if all(row_lengths == row_lengths[0]):
+                output[name] = values.reshape((-1, row_lengths[0]))
+            else:
+                output[name] = (values, offsets)
         else:
             output[name] = col.values_host if cpu else col.values
 
     return output
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/export.py` & `merlin-systems-23.4.0/merlin/systems/triton/export.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,30 @@
 # this needs to be before any modules that import protobuf
 os.environ["PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION"] = "python"
 
 import tritonclient.grpc.model_config_pb2 as model_config  # noqa
 
 import merlin.dtypes as md  # noqa
 from merlin.core.dispatch import is_string_dtype  # noqa
+from merlin.systems.dag.ops import compute_dims  # noqa
 
 
 def _add_model_param(col_schema, paramclass, params, dims=None):
-    dims = dims if dims is not None else [-1, 1]
+    dims = dims if dims is not None else compute_dims(col_schema)
     if col_schema.is_list and col_schema.is_ragged:
         params.append(
             paramclass(
                 name=col_schema.name + "__values",
                 data_type=_convert_dtype(col_schema.dtype),
-                dims=dims,
+                dims=[-1],
             )
         )
         params.append(
             paramclass(
-                name=col_schema.name + "__lengths", data_type=model_config.TYPE_INT32, dims=dims
+                name=col_schema.name + "__offsets", data_type=model_config.TYPE_INT32, dims=[-1]
             )
         )
     else:
         params.append(
             paramclass(name=col_schema.name, data_type=_convert_dtype(col_schema.dtype), dims=dims)
         )
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/models/__init__.py` & `merlin-systems-23.4.0/merlin/systems/triton/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/models/executor_model.py` & `merlin-systems-23.4.0/merlin/systems/triton/models/executor_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 import pathlib
 from pathlib import Path
 
 from merlin.dag import postorder_iter_nodes
 from merlin.systems.dag import Ensemble
 from merlin.systems.dag.runtimes.triton import TritonExecutorRuntime
 from merlin.systems.triton.conversions import (
-    dict_array_to_triton_response,
-    triton_request_to_dict_array,
+    tensor_table_to_triton_response,
+    triton_request_to_tensor_table,
 )
 from merlin.systems.triton.utils import triton_error_handling, triton_multi_request
 
 
 class TritonPythonModel:
     """Model for Triton Python Backend.
 
@@ -88,17 +88,17 @@
 
         Returns
         -------
         list
           A list of pb_utils.InferenceResponse. The length of this list must
           be the same as `requests`
         """
-        inputs = triton_request_to_dict_array(request, self.ensemble.input_schema.column_names)
+        inputs = triton_request_to_tensor_table(request, self.ensemble.input_schema.column_names)
         outputs = self.ensemble.transform(inputs, runtime=TritonExecutorRuntime())
-        return dict_array_to_triton_response(outputs)
+        return tensor_table_to_triton_response(outputs)
 
 
 def _parse_model_repository(model_repository: str) -> str:
     """
     Extract the model repository path from the model_repository value
     passed to the TritonPythonModel initialize method.
     """
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/models/pytorch_model.py` & `merlin-systems-23.4.0/merlin/systems/triton/models/pytorch_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 from merlin.systems.triton.utils import triton_error_handling, triton_multi_request
 from nvtabular.inference.triton import _convert_string2pytorch_dtype, _convert_tensor
 
 LOG = logging.getLogger("nvtabular")
 
 sparse_value_marker = "__values"
-sparse_lengths_marker = "__lengths"
+sparse_offsets_marker = "__offsets"
 
 
 class TritonPythonModel:
     """The Python back-end for PyTorch serving"""
 
     def initialize(self, args):
         # Arg parsing
@@ -77,32 +77,32 @@
                 self.model_info = json.load(json_file)
 
         # Get the name of the dense and sparse inputs, and the outputs
         self.inputs = {}
         self.sparse_inputs = {}
         self.outputs = {}
         len_svm = len(sparse_value_marker)
-        len_snm = len(sparse_lengths_marker)
+        len_snm = len(sparse_offsets_marker)
 
         for val in self.model_config["input"]:
             name = val["name"]
 
             # NVTabular adds this specific marker "__values" into the name of the sparse inputs
-            # The ones that has the marker "__lengths" are for the sparse values
+            # The ones that has the marker "__offsets" are for the sparse values
             # Hence, dense and sparse inputs are identified based on these markers
             if len(name) > len_svm:
                 if name[-len_svm:] == sparse_value_marker:
                     self.sparse_inputs[
                         name[0 : (len(name) - len_svm)]
                     ] = _convert_string2pytorch_dtype(val["data_type"])
-                elif name[-len_snm:] != sparse_lengths_marker:
+                elif name[-len_snm:] != sparse_offsets_marker:
                     self.inputs[name] = _convert_string2pytorch_dtype(val["data_type"])
             else:
                 if len(name) > len_snm:
-                    if name[-len_snm:] != sparse_lengths_marker:
+                    if name[-len_snm:] != sparse_offsets_marker:
                         self.inputs[name] = _convert_string2pytorch_dtype(val["data_type"])
                 else:
                     self.inputs[name] = _convert_string2pytorch_dtype(val["data_type"])
 
         for val in self.model_config["output"]:
             self.outputs[val["name"]] = _convert_string2pytorch_dtype(val["data_type"])
 
@@ -125,20 +125,20 @@
                     _convert_tensor(pb_utils.get_input_tensor_by_name(request, name)),
                     dtype=dtype,
                 ).cuda()
 
             # Sparse inputs have a special format
             for name, dtype in self.sparse_inputs.items():
 
-                # Get __values and __lengths
+                # Get __values and __offsets
                 input_val = _convert_tensor(
                     pb_utils.get_input_tensor_by_name(request, name + sparse_value_marker)
                 )
                 input_lengths = _convert_tensor(
-                    pb_utils.get_input_tensor_by_name(request, name + sparse_lengths_marker)
+                    pb_utils.get_input_tensor_by_name(request, name + sparse_offsets_marker)
                 )
                 input_lengths = torch.tensor(input_lengths, dtype=torch.int64)
                 input_values = torch.tensor(input_val, dtype=dtype)
 
                 # Get the PyTorch sparse_coo_tensor
                 sparse_to_dense = False
                 seq_limit = 0
@@ -194,15 +194,15 @@
     )
     if sparse_as_dense:
         sparse_tensor = sparse_tensor.to_dense()
     return sparse_tensor
 
 
 def _build_sparse_tensor(values, lengths, seq_limit, sparse_as_dense, device="cuda"):
-    """Builds PyTorch sparse_coo_tensor by converting the __values and __lengths inputs"""
+    """Builds PyTorch sparse_coo_tensor by converting the __values and __offsets inputs"""
     indices = _get_indices(lengths, device)
     num_rows = len(lengths)
     return _get_sparse_tensor(values, indices, num_rows, seq_limit, sparse_as_dense, device)
 
 
 def _convert_dtype(dtype):
     """Transformer4Rec uses these fixed dtypes and this function converts the original dtype
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/models/workflow_model.py` & `merlin-systems-23.4.0/merlin/systems/triton/models/workflow_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,17 @@
 
 import json
 import pathlib
 
 import triton_python_backend_utils as pb_utils
 
 import nvtabular
-from merlin.core.dispatch import is_list_dtype
 from merlin.systems.triton import _convert_tensor
 from merlin.systems.triton.utils import triton_error_handling, triton_multi_request
-from merlin.systems.workflow.hugectr import HugeCTRWorkflowRunner
-from merlin.systems.workflow.pytorch import PyTorchWorkflowRunner
-from merlin.systems.workflow.tensorflow import TensorflowWorkflowRunner
+from merlin.systems.workflow.base import WorkflowRunner
 
 
 class TritonPythonModel:
     """
     Triton model used for running NVT Workflows
     """
 
@@ -69,36 +66,28 @@
         model_device = args["model_instance_kind"]
 
         # Workflow instantiation
         self.workflow = nvtabular.Workflow.load(str(workflow_path))
 
         # Config loading and parsing
         self.model_config = json.loads(args["model_config"])
-        model_framework = self.model_config["parameters"]["output_model"]["string_value"]
 
         # Dtype parsing
         input_dtypes = self.workflow.input_dtypes.items()
-        self.input_dtypes, self.input_multihots = _parse_input_dtypes(input_dtypes)
+        self.input_dtypes, self.input_multihots = self._parse_input_dtypes(input_dtypes)
 
         self.output_dtypes = {}
         for col_name, col_schema in self.workflow.output_schema.column_schemas.items():
             if col_schema.is_list and col_schema.is_ragged:
-                self._set_output_dtype(col_name + "__lengths")
+                self._set_output_dtype(col_name + "__offsets")
                 self._set_output_dtype(col_name + "__values")
             else:
                 self._set_output_dtype(col_name)
 
-        if model_framework == "hugectr":
-            runner_class = HugeCTRWorkflowRunner
-        elif model_framework == "pytorch":
-            runner_class = PyTorchWorkflowRunner
-        else:
-            runner_class = TensorflowWorkflowRunner
-
-        self.runner = runner_class(
+        self.runner = WorkflowRunner(
             self.workflow, self.output_dtypes, self.model_config, model_device
         )
 
     def _set_output_dtype(self, name):
         conf = pb_utils.get_output_config_by_name(self.model_config, name)
         self.output_dtypes[name] = pb_utils.triton_string_to_numpy(conf["data_type"])
 
@@ -114,24 +103,28 @@
             for name in self.input_dtypes
         }
 
         # multihots are represented as a tuple of (values, offsets)
         for name, dtype in self.input_multihots.items():
             values = _convert_tensor(pb_utils.get_input_tensor_by_name(request, name + "__values"))
             offsets = _convert_tensor(
-                pb_utils.get_input_tensor_by_name(request, name + "__lengths")
+                pb_utils.get_input_tensor_by_name(request, name + "__offsets")
             )
             input_tensors[name] = (values, offsets)
 
-        # raise pb_utils.TritonModelException("Custom Error To check raised!")
-        raw_tensor_tuples = self.runner.run_workflow(input_tensors)
-
-        result = [pb_utils.Tensor(name, data) for name, data in raw_tensor_tuples]
+        transformed = self.runner.run_workflow(input_tensors)
+        result = [pb_utils.Tensor(name, data) for name, data in transformed.items()]
 
         return pb_utils.InferenceResponse(result)
 
+    def _is_list_dtype(self, column: str) -> bool:
+        """Check if a column of a Workflow contains list elements"""
+        col_schema = self.workflow.input_schema.get(column)
+        if col_schema is None:
+            return False
+        return col_schema.is_list and col_schema.is_ragged
+
+    def _parse_input_dtypes(self, dtypes):
+        input_dtypes = {col: dtype for col, dtype in dtypes if not self._is_list_dtype(col)}
+        input_multihots = {col: dtype for col, dtype in dtypes if self._is_list_dtype(col)}
 
-def _parse_input_dtypes(dtypes):
-    input_dtypes = {col: dtype for col, dtype in dtypes if not is_list_dtype(dtype)}
-    input_multihots = {col: dtype for col, dtype in dtypes if is_list_dtype(dtype)}
-
-    return input_dtypes, input_multihots
+        return input_dtypes, input_multihots
```

### Comparing `merlin-systems-23.2.0/merlin/systems/triton/utils.py` & `merlin-systems-23.4.0/merlin/systems/triton/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,30 +171,30 @@
         )
 
     return response
 
 
 def send_triton_request(
     schema,
-    df,
+    inputs,
     outputs_list,
     client=None,
     endpoint="localhost:8001",
     request_id="1",
     triton_model="executor_model",
 ):
     """This function checks if the triton server is available and sends a request to the Triton
     server that has already been started.
 
     Parameters
     ----------
     schema : Schema
         The schema of the inputs in the dataframe
-    df : dataframe
-        The dataframe with the inputs to predict on.
+    inputs : Union[dataframe, TensorTable]
+        The table or dataframe with the inputs to predict on.
     outputs_list : [string]
         A list of the output columns from the prediction.
     endpoint : str, optional
         The connection endpoint of the tritonserver instance, by default "localhost:8001"
     request_id : str, optional
         The id of the inference request, by default "1"
     triton_model : str, optional
@@ -202,27 +202,38 @@
 
     Returns
     -------
     results : dict
         A dictionary of parsed output column results from the prediction.
 
     """
+    from merlin.table import TensorTable
+
+    close_client = False
+
     if not client:
         try:
             client = grpcclient.InferenceServerClient(url=endpoint)
+            close_client = True
         except Exception as e:
             raise e
 
     if not client.is_server_live():
         raise ValueError("Client could not establish commuincation with Triton Inference Server.")
 
-    inputs = triton.convert_df_to_triton_input(schema, df, grpcclient.InferInput)
+    if isinstance(inputs, TensorTable):
+        triton_inputs = triton.convert_table_to_triton_input(schema, inputs, grpcclient.InferInput)
+    else:
+        triton_inputs = triton.convert_df_to_triton_input(schema, inputs, grpcclient.InferInput)
 
     outputs = [grpcclient.InferRequestedOutput(col) for col in outputs_list]
-    with client:
-        response = client.infer(triton_model, inputs, request_id=request_id, outputs=outputs)
+
+    response = client.infer(triton_model, triton_inputs, request_id=request_id, outputs=outputs)
 
     results = {}
     for col in outputs_list:
         results[col] = response.as_numpy(col)
 
+    if close_client:
+        client.close()
+
     return results
```

### Comparing `merlin-systems-23.2.0/merlin/systems/workflow/__init__.py` & `merlin-systems-23.4.0/merlin/systems/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/merlin/systems/workflow/base.py` & `merlin-systems-23.4.0/merlin/systems/workflow/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,29 +21,31 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 # OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import functools
+import itertools
 import json
 import logging
-from abc import ABC, abstractmethod
 
 import numpy as np
 
+from merlin.core.compat import cupy
 from merlin.core.dispatch import concat_columns
 from merlin.dag import ColumnSelector, Supports
 from merlin.schema import Tags
 from merlin.systems.triton.conversions import convert_format
+from merlin.table import TensorColumn, TensorTable
 
 LOG = logging.getLogger("merlin-systems")
 
 
-class WorkflowRunner(ABC):
+class WorkflowRunner:
     def __init__(self, workflow, output_dtypes, model_config, model_device):
         self.workflow = workflow
         self.output_dtypes = output_dtypes
         self.model_config = model_config
         self.device = model_device
 
         output_schema = self.workflow.output_schema
@@ -52,28 +54,24 @@
         schema_conts = output_schema.apply(ColumnSelector(tags=[Tags.CONTINUOUS])).column_names
 
         mc_cats = json.loads(self._get_param(model_config, "cats", "string_value", default="[]"))
         mc_conts = json.loads(self._get_param(model_config, "conts", "string_value", default="[]"))
 
         self.cats = mc_cats or schema_cats
         self.conts = mc_conts or schema_conts
+        self.offsets = None
 
         workflow_outputs = set(workflow.output_schema.column_names)
         requested_cols = set(self.cats + self.conts)
         missing_cols = requested_cols - workflow_outputs
-        extra_cols = workflow_outputs - requested_cols
 
         if missing_cols:
             raise ValueError(
                 f"The following columns were not found in the workflow's output: {missing_cols}"
             )
-        if extra_cols:
-            raise ValueError(
-                f"The following extra columns were found in the workflow's output: {extra_cols}"
-            )
 
         # recurse over all column groups, initializing operators for inference pipeline
         self._initialize_ops(self.workflow.output_node)
 
     def _initialize_ops(self, workflow_node, visited=None):
         if visited is None:
             visited = set()
@@ -107,27 +105,27 @@
         transformed, kind = self._transform_tensors(input_tensors, self.workflow.output_node)
 
         # if we don't have tensors in numpy format, convert back so that the we can return
         # to triton
         if kind != Supports.CPU_DICT_ARRAY:
             transformed, kind = convert_format(transformed, kind, Supports.CPU_DICT_ARRAY)
 
-        # convert to the format expected by the DL models
-        return self._transform_outputs(transformed)
+        output_table = TensorTable(transformed)
+
+        for col in self.workflow.output_schema:
+            if col.is_ragged and output_table[col.name].offsets is None:
+                values, offsets = _to_ragged(output_table[col.name].values)
+                output_table[col.name] = TensorColumn(values, offsets=offsets)
+
+        output_dict = output_table.to_dict()
 
-    @abstractmethod
-    def _transform_outputs(self, tensors):
-        pass
-
-    def _convert_to_np(self, columns, tensors, dtype, rows):
-        """converts outputs to a numpy input compatible with pytorch"""
-        d = np.empty((rows, len(columns)), dtype=dtype)
-        for i, name in enumerate(columns):
-            d[:, i] = tensors[name].astype(dtype)
-        return d
+        for key, value in output_dict.items():
+            output_dict[key] = value.astype(self.output_dtypes[key])
+
+        return output_dict
 
     def _transform_tensors(self, input_tensors, workflow_node):
         upstream_inputs = []
 
         # Gather inputs from the parents and dependency nodes
         if workflow_node.parents_with_dependencies:
             for parent in workflow_node.parents_with_dependencies:
@@ -203,7 +201,29 @@
             return output
 
     def _get_param(self, config, *args, default=None):
         config_element = config["parameters"]
         for key in args:
             config_element = config_element.get(key, {})
         return config_element or default
+
+
+def _to_ragged(array):
+    """Convert Array to Ragged representation
+
+    Parameters
+    ----------
+    array : numpy.ndarray or cupy.ndarray
+        Array to convert
+
+    Returns
+    -------
+    values, offsets
+        Tuple of values and offsets
+    """
+    num_rows = array.shape[0]
+    row_lengths = [array.shape[1]] * num_rows
+    offsets = [0] + list(itertools.accumulate(row_lengths))
+    array_lib = cupy if cupy and isinstance(array, cupy.ndarray) else np
+    offsets = array_lib.array(offsets, dtype="int32")
+    values = array.reshape(-1, *array.shape[2:])
+    return values, offsets
```

### Comparing `merlin-systems-23.2.0/merlin_systems.egg-info/PKG-INFO` & `merlin-systems-23.4.0/merlin_systems.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-systems
-Version: 23.2.0
+Version: 23.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/systems
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-systems-23.2.0/merlin_systems.egg-info/SOURCES.txt` & `merlin-systems-23.4.0/merlin_systems.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 setup.cfg
 setup.py
 versioneer.py
 merlin/systems/__init__.py
 merlin/systems/_version.py
 merlin/systems/model_registry.py
 merlin/systems/dag/__init__.py
-merlin/systems/dag/dictarray.py
 merlin/systems/dag/ensemble.py
 merlin/systems/dag/node.py
-merlin/systems/dag/op_runner.py
 merlin/systems/dag/ops/__init__.py
 merlin/systems/dag/ops/compat.py
 merlin/systems/dag/ops/faiss.py
 merlin/systems/dag/ops/feast.py
 merlin/systems/dag/ops/fil.py
 merlin/systems/dag/ops/implicit.py
 merlin/systems/dag/ops/operator.py
@@ -28,33 +26,28 @@
 merlin/systems/dag/ops/workflow.py
 merlin/systems/dag/runtimes/__init__.py
 merlin/systems/dag/runtimes/base_runtime.py
 merlin/systems/dag/runtimes/triton/__init__.py
 merlin/systems/dag/runtimes/triton/runtime.py
 merlin/systems/dag/runtimes/triton/ops/__init__.py
 merlin/systems/dag/runtimes/triton/ops/fil.py
-merlin/systems/dag/runtimes/triton/ops/implicit.py
 merlin/systems/dag/runtimes/triton/ops/operator.py
 merlin/systems/dag/runtimes/triton/ops/pytorch.py
 merlin/systems/dag/runtimes/triton/ops/tensorflow.py
 merlin/systems/dag/runtimes/triton/ops/workflow.py
 merlin/systems/triton/__init__.py
 merlin/systems/triton/conversions.py
 merlin/systems/triton/export.py
 merlin/systems/triton/utils.py
 merlin/systems/triton/models/__init__.py
 merlin/systems/triton/models/executor_model.py
-merlin/systems/triton/models/oprunner_model.py
 merlin/systems/triton/models/pytorch_model.py
 merlin/systems/triton/models/workflow_model.py
 merlin/systems/workflow/__init__.py
 merlin/systems/workflow/base.py
-merlin/systems/workflow/hugectr.py
-merlin/systems/workflow/pytorch.py
-merlin/systems/workflow/tensorflow.py
 merlin_systems.egg-info/PKG-INFO
 merlin_systems.egg-info/SOURCES.txt
 merlin_systems.egg-info/dependency_links.txt
 merlin_systems.egg-info/not-zip-safe
 merlin_systems.egg-info/requires.txt
 merlin_systems.egg-info/top_level.txt
 requirements/base.txt
```

### Comparing `merlin-systems-23.2.0/merlin_systems.egg-info/requires.txt` & `merlin-systems-23.4.0/merlin_systems.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
+tritonclient[all]
 
 [cpu]
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
+tritonclient[all]
 
 [dev]
 tritonclient[all]
 
 [docs]
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
 tritonclient[all]
 tensorflow<=2.9.0
 Sphinx==3.5.4
@@ -40,66 +42,66 @@
 faiss-gpu
 pytest
 pytest-cov
 dask>=2022.3.0
 distributed>=2022.3.0
 
 [test]
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
+tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-tritonclient
-feast==0.19.4
+feast==0.18.1
 xgboost==1.6.2
 implicit==0.6.0
 
 [test-cpu]
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
+tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-tritonclient
-feast==0.19.4
+feast==0.18.1
 xgboost==1.6.2
 implicit==0.6.0
-merlin-models>=0.6.0
+merlin-models>=23.4.0
 faiss-cpu==1.7.2
 tensorflow<=2.9.0
 treelite==2.4.0
 treelite_runtime==2.4.0
 torch~=1.12
 lightgbm==3.3.2
 ipykernel
 
 [test-gpu]
-merlin-core>=0.2.0
-nvtabular>=1.0.0
+merlin-core>=23.4.0
+nvtabular>=23.4.0
 requests<3,>=2.10
 treelite==2.4.0
 treelite_runtime==2.4.0
 tritonclient[all]
+tritonclient[all]
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@ git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
-tritonclient
-feast==0.19.4
+feast==0.18.1
 xgboost==1.6.2
 implicit==0.6.0
 tensorflow-gpu<=2.9.0
 faiss-gpu==1.7.2
```

### Comparing `merlin-systems-23.2.0/pyproject.toml` & `merlin-systems-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/requirements/test.txt` & `merlin-systems-23.4.0/requirements/test.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,13 @@
 pytest>=5
 pytest-cov>=2
 scikit-learn<1.2
 asvdb@git+https://github.com/rapidsai/asvdb.git
 testbook==0.4.2
 
 # packages necessary to run tests and push PRs
-tritonclient
-feast==0.19.4
+feast==0.18.1
 xgboost==1.6.2
 implicit==0.6.0
 
 # TODO: do we need more of these?
 # https://github.com/NVIDIA-Merlin/Merlin/blob/a1cc48fe23c4dfc627423168436f26ef7e028204/ci/dockerfile.ci#L13-L18
```

### Comparing `merlin-systems-23.2.0/setup.cfg` & `merlin-systems-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-systems-23.2.0/setup.py` & `merlin-systems-23.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 }
 
 with open("README.md", encoding="utf8") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="merlin-systems",
-    version=versioneer.get_version(),
+    version="23.04.00",
     packages=find_namespace_packages(include=["merlin*"]),
     url="https://github.com/NVIDIA-Merlin/systems",
     author="NVIDIA Corporation",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `merlin-systems-23.2.0/versioneer.py` & `merlin-systems-23.4.0/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1700,14 +1700,17 @@
 
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
+    return {
+        "version": "23.04.00"
+    }
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
```

