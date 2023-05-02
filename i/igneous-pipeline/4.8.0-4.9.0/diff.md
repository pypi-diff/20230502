# Comparing `tmp/igneous-pipeline-4.8.0.tar.gz` & `tmp/igneous-pipeline-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igneous-pipeline-4.8.0.tar", last modified: Thu Sep 29 18:03:48 2022, max compression
+gzip compressed data, was "igneous-pipeline-4.9.0.tar", last modified: Wed Oct 12 01:22:59 2022, max compression
```

## Comparing `igneous-pipeline-4.8.0.tar` & `igneous-pipeline-4.9.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.503594 igneous-pipeline-4.8.0/
--rw-r--r--   0 wms        (501) staff       (20)      153 2022-08-18 23:55:36.000000 igneous-pipeline-4.8.0/.dockerignore
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.486506 igneous-pipeline-4.8.0/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.490444 igneous-pipeline-4.8.0/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)      491 2022-08-19 00:18:27.000000 igneous-pipeline-4.8.0/.github/workflows/docker-image.yml
--rw-r--r--   0 wms        (501) staff       (20)      892 2022-08-02 21:06:14.000000 igneous-pipeline-4.8.0/.github/workflows/test-suite.yml
--rwxr-xr-x   0 wms        (501) staff       (20)      577 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)      932 2022-05-20 18:44:24.000000 igneous-pipeline-4.8.0/CITATION.cff
--rwxr-xr-x   0 wms        (501) staff       (20)    29651 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/ChangeLog
--rwxr-xr-x   0 wms        (501) staff       (20)     1075 2022-09-19 17:18:34.000000 igneous-pipeline-4.8.0/Dockerfile
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-11 02:21:34.000000 igneous-pipeline-4.8.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)    47590 2022-09-29 18:03:48.503913 igneous-pipeline-4.8.0/PKG-INFO
--rwxr-xr-x   0 wms        (501) staff       (20)    41419 2022-08-02 20:26:13.000000 igneous-pipeline-4.8.0/README.md
--rwxr-xr-x   0 wms        (501) staff       (20)     1216 2022-09-20 17:53:19.000000 igneous-pipeline-4.8.0/deployment.yaml
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.492097 igneous-pipeline-4.8.0/igneous/
--rwxr-xr-x   0 wms        (501) staff       (20)      175 2021-01-11 02:21:34.000000 igneous-pipeline-4.8.0/igneous/__init__.py
--rwxr-xr-x   0 wms        (501) staff       (20)    11981 2022-08-10 20:37:28.000000 igneous-pipeline-4.8.0/igneous/downsample_scales.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.492623 igneous-pipeline-4.8.0/igneous/scripts/
--rwxr-xr-x   0 wms        (501) staff       (20)     1318 2021-07-16 21:14:45.000000 igneous-pipeline-4.8.0/igneous/scripts/remap2npy.py
--rwxr-xr-x   0 wms        (501) staff       (20)     1584 2021-01-11 02:21:34.000000 igneous-pipeline-4.8.0/igneous/scripts/validate_provenance.py
--rwxr-xr-x   0 wms        (501) staff       (20)      479 2021-07-16 21:19:15.000000 igneous-pipeline-4.8.0/igneous/secrets.py
--rw-r--r--   0 wms        (501) staff       (20)     1469 2021-10-07 20:04:55.000000 igneous-pipeline-4.8.0/igneous/shards.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.494796 igneous-pipeline-4.8.0/igneous/task_creation/
--rw-r--r--   0 wms        (501) staff       (20)       89 2021-07-16 21:14:45.000000 igneous-pipeline-4.8.0/igneous/task_creation/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     6161 2022-04-13 23:09:49.000000 igneous-pipeline-4.8.0/igneous/task_creation/common.py
--rw-r--r--   0 wms        (501) staff       (20)    47842 2022-08-10 20:37:28.000000 igneous-pipeline-4.8.0/igneous/task_creation/image.py
--rw-r--r--   0 wms        (501) staff       (20)    22359 2022-09-15 22:54:17.000000 igneous-pipeline-4.8.0/igneous/task_creation/mesh.py
--rw-r--r--   0 wms        (501) staff       (20)     6443 2021-07-16 21:14:45.000000 igneous-pipeline-4.8.0/igneous/task_creation/obsolete.py
--rw-r--r--   0 wms        (501) staff       (20)        0 2022-07-19 05:22:12.000000 igneous-pipeline-4.8.0/igneous/task_creation/setup.py
--rw-r--r--   0 wms        (501) staff       (20)    23403 2022-04-13 23:09:49.000000 igneous-pipeline-4.8.0/igneous/task_creation/skeleton.py
--rwxr-xr-x   0 wms        (501) staff       (20)     2368 2021-12-14 00:03:14.000000 igneous-pipeline-4.8.0/igneous/task_execution.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.496222 igneous-pipeline-4.8.0/igneous/tasks/
--rw-r--r--   0 wms        (501) staff       (20)      867 2022-06-25 04:12:24.000000 igneous-pipeline-4.8.0/igneous/tasks/__init__.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.497502 igneous-pipeline-4.8.0/igneous/tasks/image/
--rw-r--r--   0 wms        (501) staff       (20)       39 2022-06-25 04:12:24.000000 igneous-pipeline-4.8.0/igneous/tasks/image/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    12457 2022-08-02 20:14:33.000000 igneous-pipeline-4.8.0/igneous/tasks/image/ccl.py
--rwxr-xr-x   0 wms        (501) staff       (20)    18163 2022-06-25 04:12:24.000000 igneous-pipeline-4.8.0/igneous/tasks/image/image.py
--rw-r--r--   0 wms        (501) staff       (20)    24373 2022-06-25 04:12:24.000000 igneous-pipeline-4.8.0/igneous/tasks/image/obsolete.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.498953 igneous-pipeline-4.8.0/igneous/tasks/mesh/
--rw-r--r--   0 wms        (501) staff       (20)       43 2021-11-12 23:46:32.000000 igneous-pipeline-4.8.0/igneous/tasks/mesh/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     2057 2021-12-14 00:03:14.000000 igneous-pipeline-4.8.0/igneous/tasks/mesh/draco.py
--rw-r--r--   0 wms        (501) staff       (20)    22003 2022-09-13 02:50:09.000000 igneous-pipeline-4.8.0/igneous/tasks/mesh/mesh.py
--rw-r--r--   0 wms        (501) staff       (20)    11056 2021-11-12 23:46:32.000000 igneous-pipeline-4.8.0/igneous/tasks/mesh/mesh_graphene_remap.py
--rw-r--r--   0 wms        (501) staff       (20)    15920 2022-09-21 04:36:39.000000 igneous-pipeline-4.8.0/igneous/tasks/mesh/multires.py
--rw-r--r--   0 wms        (501) staff       (20)    16467 2022-09-17 03:44:08.000000 igneous-pipeline-4.8.0/igneous/tasks/skeleton.py
--rw-r--r--   0 wms        (501) staff       (20)     2165 2022-04-13 23:09:49.000000 igneous-pipeline-4.8.0/igneous/tasks/spatial_index.py
--rwxr-xr-x   0 wms        (501) staff       (20)     3873 2021-01-11 02:21:34.000000 igneous-pipeline-4.8.0/igneous/tasks/watershed.py
--rw-r--r--   0 wms        (501) staff       (20)       86 2021-07-16 21:14:45.000000 igneous-pipeline-4.8.0/igneous/types.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.500571 igneous-pipeline-4.8.0/igneous_cli/
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-05-14 05:03:28.000000 igneous-pipeline-4.8.0/igneous_cli/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       82 2021-05-14 05:03:28.000000 igneous-pipeline-4.8.0/igneous_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    64211 2022-09-29 18:02:36.000000 igneous-pipeline-4.8.0/igneous_cli/cli.py
--rw-r--r--   0 wms        (501) staff       (20)     2339 2021-06-20 21:29:02.000000 igneous-pipeline-4.8.0/igneous_cli/humanbytes.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.501868 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    47590 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     1585 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       46 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-01-03 23:58:12.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)      342 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       20 2022-09-29 18:03:48.000000 igneous-pipeline-4.8.0/igneous_pipeline.egg-info/top_level.txt
--rw-r--r--   0 wms        (501) staff       (20)       68 2022-01-29 00:52:40.000000 igneous-pipeline-4.8.0/pyproject.toml
--rwxr-xr-x   0 wms        (501) staff       (20)      341 2022-09-19 17:50:41.000000 igneous-pipeline-4.8.0/requirements.txt
--rwxr-xr-x   0 wms        (501) staff       (20)     1016 2022-09-29 18:03:48.504449 igneous-pipeline-4.8.0/setup.cfg
--rwxr-xr-x   0 wms        (501) staff       (20)      323 2022-09-19 16:18:14.000000 igneous-pipeline-4.8.0/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-29 18:03:48.503360 igneous-pipeline-4.8.0/test/
--rwxr-xr-x   0 wms        (501) staff       (20)        0 2021-01-11 02:21:34.000000 igneous-pipeline-4.8.0/test/__init__.py
--rwxr-xr-x   0 wms        (501) staff       (20)     3480 2021-06-20 21:29:02.000000 igneous-pipeline-4.8.0/test/downsample_scales_test.py
--rwxr-xr-x   0 wms        (501) staff       (20)     1376 2021-07-16 21:14:45.000000 igneous-pipeline-4.8.0/test/layer_harness.py
--rw-r--r--   0 wms        (501) staff       (20)     6446 2022-08-02 19:47:10.000000 igneous-pipeline-4.8.0/test/test_ccl_tasks.py
--rw-r--r--   0 wms        (501) staff       (20)     4748 2022-04-13 23:09:49.000000 igneous-pipeline-4.8.0/test/test_shards.py
--rwxr-xr-x   0 wms        (501) staff       (20)    15577 2022-07-12 01:11:28.000000 igneous-pipeline-4.8.0/test/test_tasks.py
--rw-r--r--   0 wms        (501) staff       (20)     3990 2022-01-03 23:44:20.000000 igneous-pipeline-4.8.0/test/test_transfer_tasks.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.204538 igneous-pipeline-4.9.0/
+-rw-r--r--   0 wms        (501) staff       (20)      153 2022-08-18 23:55:36.000000 igneous-pipeline-4.9.0/.dockerignore
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.187487 igneous-pipeline-4.9.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.192030 igneous-pipeline-4.9.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)      491 2022-08-19 00:18:27.000000 igneous-pipeline-4.9.0/.github/workflows/docker-image.yml
+-rw-r--r--   0 wms        (501) staff       (20)      892 2022-08-02 21:06:14.000000 igneous-pipeline-4.9.0/.github/workflows/test-suite.yml
+-rwxr-xr-x   0 wms        (501) staff       (20)      577 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)      932 2022-05-20 18:44:24.000000 igneous-pipeline-4.9.0/CITATION.cff
+-rwxr-xr-x   0 wms        (501) staff       (20)    29796 2022-10-12 01:22:58.000000 igneous-pipeline-4.9.0/ChangeLog
+-rwxr-xr-x   0 wms        (501) staff       (20)     1075 2022-09-19 17:18:34.000000 igneous-pipeline-4.9.0/Dockerfile
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-11 02:21:34.000000 igneous-pipeline-4.9.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)    47590 2022-10-12 01:22:59.204862 igneous-pipeline-4.9.0/PKG-INFO
+-rwxr-xr-x   0 wms        (501) staff       (20)    41419 2022-08-02 20:26:13.000000 igneous-pipeline-4.9.0/README.md
+-rwxr-xr-x   0 wms        (501) staff       (20)     1172 2022-10-08 02:46:21.000000 igneous-pipeline-4.9.0/deployment.yaml
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.193603 igneous-pipeline-4.9.0/igneous/
+-rwxr-xr-x   0 wms        (501) staff       (20)      175 2021-01-11 02:21:34.000000 igneous-pipeline-4.9.0/igneous/__init__.py
+-rwxr-xr-x   0 wms        (501) staff       (20)    11981 2022-08-10 20:37:28.000000 igneous-pipeline-4.9.0/igneous/downsample_scales.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.194128 igneous-pipeline-4.9.0/igneous/scripts/
+-rwxr-xr-x   0 wms        (501) staff       (20)     1318 2021-07-16 21:14:45.000000 igneous-pipeline-4.9.0/igneous/scripts/remap2npy.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     1584 2021-01-11 02:21:34.000000 igneous-pipeline-4.9.0/igneous/scripts/validate_provenance.py
+-rwxr-xr-x   0 wms        (501) staff       (20)      479 2021-07-16 21:19:15.000000 igneous-pipeline-4.9.0/igneous/secrets.py
+-rw-r--r--   0 wms        (501) staff       (20)     1469 2021-10-07 20:04:55.000000 igneous-pipeline-4.9.0/igneous/shards.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.195753 igneous-pipeline-4.9.0/igneous/task_creation/
+-rw-r--r--   0 wms        (501) staff       (20)       89 2021-07-16 21:14:45.000000 igneous-pipeline-4.9.0/igneous/task_creation/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     6756 2022-10-12 01:21:57.000000 igneous-pipeline-4.9.0/igneous/task_creation/common.py
+-rw-r--r--   0 wms        (501) staff       (20)    48060 2022-10-12 01:21:57.000000 igneous-pipeline-4.9.0/igneous/task_creation/image.py
+-rw-r--r--   0 wms        (501) staff       (20)    22359 2022-09-15 22:54:17.000000 igneous-pipeline-4.9.0/igneous/task_creation/mesh.py
+-rw-r--r--   0 wms        (501) staff       (20)     6443 2021-07-16 21:14:45.000000 igneous-pipeline-4.9.0/igneous/task_creation/obsolete.py
+-rw-r--r--   0 wms        (501) staff       (20)        0 2022-07-19 05:22:12.000000 igneous-pipeline-4.9.0/igneous/task_creation/setup.py
+-rw-r--r--   0 wms        (501) staff       (20)    23403 2022-04-13 23:09:49.000000 igneous-pipeline-4.9.0/igneous/task_creation/skeleton.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     2368 2021-12-14 00:03:14.000000 igneous-pipeline-4.9.0/igneous/task_execution.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.197185 igneous-pipeline-4.9.0/igneous/tasks/
+-rw-r--r--   0 wms        (501) staff       (20)      867 2022-06-25 04:12:24.000000 igneous-pipeline-4.9.0/igneous/tasks/__init__.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.198687 igneous-pipeline-4.9.0/igneous/tasks/image/
+-rw-r--r--   0 wms        (501) staff       (20)       39 2022-06-25 04:12:24.000000 igneous-pipeline-4.9.0/igneous/tasks/image/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    12457 2022-08-02 20:14:33.000000 igneous-pipeline-4.9.0/igneous/tasks/image/ccl.py
+-rwxr-xr-x   0 wms        (501) staff       (20)    18166 2022-10-12 01:21:57.000000 igneous-pipeline-4.9.0/igneous/tasks/image/image.py
+-rw-r--r--   0 wms        (501) staff       (20)    24373 2022-06-25 04:12:24.000000 igneous-pipeline-4.9.0/igneous/tasks/image/obsolete.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.200354 igneous-pipeline-4.9.0/igneous/tasks/mesh/
+-rw-r--r--   0 wms        (501) staff       (20)       43 2021-11-12 23:46:32.000000 igneous-pipeline-4.9.0/igneous/tasks/mesh/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     2057 2021-12-14 00:03:14.000000 igneous-pipeline-4.9.0/igneous/tasks/mesh/draco.py
+-rw-r--r--   0 wms        (501) staff       (20)    22003 2022-09-13 02:50:09.000000 igneous-pipeline-4.9.0/igneous/tasks/mesh/mesh.py
+-rw-r--r--   0 wms        (501) staff       (20)    11056 2021-11-12 23:46:32.000000 igneous-pipeline-4.9.0/igneous/tasks/mesh/mesh_graphene_remap.py
+-rw-r--r--   0 wms        (501) staff       (20)    15920 2022-09-21 04:36:39.000000 igneous-pipeline-4.9.0/igneous/tasks/mesh/multires.py
+-rw-r--r--   0 wms        (501) staff       (20)    16467 2022-09-17 03:44:08.000000 igneous-pipeline-4.9.0/igneous/tasks/skeleton.py
+-rw-r--r--   0 wms        (501) staff       (20)     2165 2022-04-13 23:09:49.000000 igneous-pipeline-4.9.0/igneous/tasks/spatial_index.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     3873 2021-01-11 02:21:34.000000 igneous-pipeline-4.9.0/igneous/tasks/watershed.py
+-rw-r--r--   0 wms        (501) staff       (20)       86 2021-07-16 21:14:45.000000 igneous-pipeline-4.9.0/igneous/types.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.201457 igneous-pipeline-4.9.0/igneous_cli/
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-05-14 05:03:28.000000 igneous-pipeline-4.9.0/igneous_cli/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       82 2021-05-14 05:03:28.000000 igneous-pipeline-4.9.0/igneous_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    64498 2022-10-12 01:22:13.000000 igneous-pipeline-4.9.0/igneous_cli/cli.py
+-rw-r--r--   0 wms        (501) staff       (20)     2339 2021-06-20 21:29:02.000000 igneous-pipeline-4.9.0/igneous_cli/humanbytes.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.202808 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    47590 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     1585 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       46 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-01-03 23:58:12.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)      342 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       20 2022-10-12 01:22:59.000000 igneous-pipeline-4.9.0/igneous_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 wms        (501) staff       (20)       68 2022-01-29 00:52:40.000000 igneous-pipeline-4.9.0/pyproject.toml
+-rwxr-xr-x   0 wms        (501) staff       (20)      341 2022-09-19 17:50:41.000000 igneous-pipeline-4.9.0/requirements.txt
+-rwxr-xr-x   0 wms        (501) staff       (20)     1016 2022-10-12 01:22:59.205397 igneous-pipeline-4.9.0/setup.cfg
+-rwxr-xr-x   0 wms        (501) staff       (20)      323 2022-09-19 16:18:14.000000 igneous-pipeline-4.9.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-10-12 01:22:59.204317 igneous-pipeline-4.9.0/test/
+-rwxr-xr-x   0 wms        (501) staff       (20)        0 2021-01-11 02:21:34.000000 igneous-pipeline-4.9.0/test/__init__.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     3480 2021-06-20 21:29:02.000000 igneous-pipeline-4.9.0/test/downsample_scales_test.py
+-rwxr-xr-x   0 wms        (501) staff       (20)     1376 2021-07-16 21:14:45.000000 igneous-pipeline-4.9.0/test/layer_harness.py
+-rw-r--r--   0 wms        (501) staff       (20)     6446 2022-08-02 19:47:10.000000 igneous-pipeline-4.9.0/test/test_ccl_tasks.py
+-rw-r--r--   0 wms        (501) staff       (20)     4748 2022-04-13 23:09:49.000000 igneous-pipeline-4.9.0/test/test_shards.py
+-rwxr-xr-x   0 wms        (501) staff       (20)    15577 2022-07-12 01:11:28.000000 igneous-pipeline-4.9.0/test/test_tasks.py
+-rw-r--r--   0 wms        (501) staff       (20)     3990 2022-01-03 23:44:20.000000 igneous-pipeline-4.9.0/test/test_transfer_tasks.py
```

### Comparing `igneous-pipeline-4.8.0/.github/workflows/test-suite.yml` & `igneous-pipeline-4.9.0/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/AUTHORS` & `igneous-pipeline-4.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/CITATION.cff` & `igneous-pipeline-4.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/ChangeLog` & `igneous-pipeline-4.9.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+4.9.0
+-----
+
+* release(4.9.0): adds --encoding-level to image xfer
+* feat: add encoding level to transfer tasks (#140)
+* docs: update ChangeLog
+
 4.8.0
 -----
 
 * release(4.8.0): -x works for SQS, don't encode degenerate meshes
 * feat(cli): add message noting that sqs is waiting
 * refactor(cli): use CloudPath param type instead of extra loc
 * feat(cli): add CloudPath parameter class
```

### Comparing `igneous-pipeline-4.8.0/Dockerfile` & `igneous-pipeline-4.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/LICENSE` & `igneous-pipeline-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/PKG-INFO` & `igneous-pipeline-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igneous-pipeline
-Version: 4.8.0
+Version: 4.9.0
 Summary: Downsample, Mesh, Skeletonize, and Remap Neuroglancer Datasets
 Home-page: https://github.com/seung-lab/igneous/
 Author: Ignacio Tartavull, William Silversmith, and others
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description: [![PyPI version](https://badge.fury.io/py/igneous-pipeline.svg)](https://badge.fury.io/py/igneous-pipeline) [![SfN 2018 Poster](https://img.shields.io/badge/poster-SfN%202018-blue.svg)](https://drive.google.com/open?id=1RKtaAGV2f7F13opnkQfbp6YBqmoD3fZi)
```

### Comparing `igneous-pipeline-4.8.0/README.md` & `igneous-pipeline-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/deployment.yaml` & `igneous-pipeline-4.9.0/deployment.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -34,15 +34,15 @@
               memory: 2.5Gi
             limits:
               memory: 7.0Gi
           env:
             - name: QUEUE_TYPE
               value: aws
             - name: SQS_URL
-              value: 'https://sqs.us-east-1.amazonaws.com/$DIGITS/$QUEUE_NAME'
+              value: 'wms-igneous'
             - name: LEASE_SECONDS
               value: "800"
       volumes:
       - name: secrets
         secret:
           secretName: secrets
       - name: tmp
```

### Comparing `igneous-pipeline-4.8.0/igneous/downsample_scales.py` & `igneous-pipeline-4.9.0/igneous/downsample_scales.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/scripts/remap2npy.py` & `igneous-pipeline-4.9.0/igneous/scripts/remap2npy.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/scripts/validate_provenance.py` & `igneous-pipeline-4.9.0/igneous/scripts/validate_provenance.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/shards.py` & `igneous-pipeline-4.9.0/igneous/shards.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/task_creation/common.py` & `igneous-pipeline-4.9.0/igneous/task_creation/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -207,7 +207,28 @@
   shard_bits += delta
   minishard_bits -= delta
 
   shard_bits = max(shard_bits, min_shard_bits)
   minishard_bits = max(minishard_bits, 0)
 
   return (int(shard_bits), int(minishard_bits), 0)
+
+def set_encoding(cv, mip, encoding, encoding_level):
+  scale = cv.meta.scale(mip)
+  if encoding is not None:
+    scale['encoding'] = encoding
+    if encoding == 'compressed_segmentation' and 'compressed_segmentation_block_size' not in scale:
+      scale['compressed_segmentation_block_size'] = (8,8,8)
+
+  if encoding_level is None:
+    return
+
+  encoding_level = int(encoding_level)
+
+  if encoding == "jpeg":
+    scale["jpeg_quality"] = encoding_level
+  elif encoding == "png":
+    scale["png_level"] = encoding_level
+  elif encoding == "fpzip":
+    scale["fpzip_precision"] = encoding_level
+
+
```

### Comparing `igneous-pipeline-4.8.0/igneous/task_creation/image.py` & `igneous-pipeline-4.9.0/igneous/task_creation/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 )
 
 from igneous.shards import image_shard_shape_from_spec
 from igneous.types import ShapeType
 
 from .common import (
   operator_contact, FinelyDividedTaskIterator, 
-  get_bounds, num_tasks, prod
+  get_bounds, num_tasks, prod, set_encoding
 )
 
 __all__  = [
   "create_blackout_tasks",
   "create_touch_tasks",
   "create_downsampling_tasks", 
   "create_image_shard_downsample_tasks",
@@ -419,15 +419,16 @@
   bounds_mip : int = 0,
   fill_missing: bool = False,
   translate: ShapeType = (0, 0, 0),
   dest_voxel_offset: Optional[ShapeType] = None,
   agglomerate: bool = False, 
   timestamp: int = None,
   memory_target: int = MEMORY_TARGET,
-  clean_info: bool = False
+  clean_info: bool = False,
+  encoding_level: Optional[int] = None,
 ):
   src_vol = CloudVolume(src_layer_path, mip=mip)
 
   if dest_voxel_offset:
     dest_voxel_offset = Vec(*dest_voxel_offset, dtype=int)
   else:
     dest_voxel_offset = src_vol.voxel_offset.clone()
@@ -438,29 +439,32 @@
 
   try:
     dest_vol = CloudVolume(dst_layer_path, mip=mip)
   except cloudvolume.exceptions.InfoUnavailableError:
     info = copy.deepcopy(src_vol.info)
     dest_vol = CloudVolume(dst_layer_path, info=info, mip=mip)
     dest_vol.commit_info()
+  except cloudvolume.exceptions.ScaleUnavailableError:
+    dest_vol = CloudVolume(dst_layer_path)
+    dest_vol.scales.append(src_vol.scale)
+    dest_vol.mip = src_vol.scale["resolution"]
+    dest_vol.commit_info()
 
   if dest_voxel_offset is not None:
     dest_vol.scale["voxel_offset"] = dest_voxel_offset
 
   # If translate is not set, but dest_voxel_offset is then it should naturally be
   # only be the difference between datasets.
   if translate is None:
     translate = dest_vol.voxel_offset - src_vol.voxel_offset # vector pointing from src to dest
   else:
     translate = Vec(*translate) // src_vol.downsample_ratio
 
-  if encoding is not None:
-    dest_vol.info['scales'][mip]['encoding'] = encoding
-    if encoding == 'compressed_segmentation' and 'compressed_segmentation_block_size' not in dest_vol.info['scales'][mip]:
-      dest_vol.info['scales'][mip]['compressed_segmentation_block_size'] = (8,8,8)
+  set_encoding(dest_vol, mip, encoding, encoding_level)
+
   dest_vol.info['scales'] = dest_vol.info['scales'][:mip+1]
   dest_vol.info['scales'][mip]['chunk_sizes'] = [ chunk_size.tolist() ]
 
   spec = create_sharded_image_info(
     dataset_size=dest_vol.scale["size"], 
     chunk_size=dest_vol.scale["chunk_sizes"][0], 
     encoding=dest_vol.scale["encoding"], 
@@ -501,14 +505,15 @@
           "src": src_layer_path,
           "dest": dst_layer_path,
           "shape": list(map(int, shape)),
           "fill_missing": fill_missing,
           "translate": list(map(int, translate)),
           "bounds": [bounds.minpt.tolist(), bounds.maxpt.tolist()],
           "mip": mip,
+          "encoding_level": encoding_level,
         },
         "by": operator_contact(),
         "date": strftime("%Y-%m-%d %H:%M %Z"),
       }
 
       dvol = CloudVolume(dst_layer_path)
       dvol.provenance.sources = [src_layer_path]
@@ -664,14 +669,15 @@
   sparse:bool = False, 
   dest_voxel_offset:ShapeType = None,
   memory_target:int = MEMORY_TARGET, 
   max_mips:int = 5, 
   clean_info:bool = False, 
   no_src_update:bool = False, 
   bounds_mip:int = 0,
+  encoding_level:Optional[int] = None,
 ) -> Iterator:
   """
   Transfer data to a new data layer. You can use this operation
   to make changes to the dataset representation as well. For 
   example, you can change the chunk size, compression, bounds,
   and offset.
 
@@ -699,14 +705,18 @@
     that are all background.
   encoding: "raw", "jpeg", "compressed_segmentation", "compresso", "fpzip", or "kempressed"
     depending on which kind of data you're dealing with. raw works for everything (no compression) 
     but you might get better compression with another encoding. You can think of encoding as the
     image type-specific first stage of compression and the "compress" flag as the data
     agnostic second stage compressor. For example, compressed_segmentation and gzip work
     well together, but not jpeg and gzip.
+  encoding_level: Some encoding schemes (png,jpeg,fpzip) offer a simple scalar knob
+    to control encoding quality. This number corresponds to png level, jpeg quality,
+    and fpzip precision. Other schemes might require more complex inputs and may
+    require info file modifications.
   factor: (overrides axis) can manually specify what each downsampling round is
     supposed to do: e.g. (2,2,1), (2,2,2), etc
   fill_missing: Treat missing image tiles as zeroed for both src and dest.
   max_mips: (pairs with memory_target) maximum number of downsamples to generate even
     if the memory budget is large enough for more.
   memory_target: given a task size in bytes, pick the task shape that will produce the 
     maximum number of downsamples. Only works for (2,2,1) or (2,2,2).
@@ -767,18 +777,15 @@
   # If translate is not set, but dest_voxel_offset is then it should naturally be
   # only be the difference between datasets.
   if translate is None:
     translate = dest_vol.voxel_offset - src_vol.voxel_offset # vector pointing from src to dest
   else:
     translate = Vec(*translate) // src_vol.downsample_ratio
 
-  if encoding is not None:
-    dest_vol.info['scales'][mip]['encoding'] = encoding
-    if encoding == 'compressed_segmentation' and 'compressed_segmentation_block_size' not in dest_vol.info['scales'][mip]:
-      dest_vol.info['scales'][mip]['compressed_segmentation_block_size'] = (8,8,8)
+  set_encoding(dest_vol, mip, encoding, encoding_level)
   dest_vol.info['scales'] = dest_vol.info['scales'][:mip+1]
   dest_vol.info['scales'][mip]['chunk_sizes'] = [ chunk_size.tolist() ]
 
   if clean_info:
     dest_vol.info = clean_xfer_info(dest_vol.info)
 
   dest_vol.commit_info()
@@ -851,14 +858,15 @@
           'agglomerate': bool(agglomerate),
           'timestamp': timestamp,
           'compress': compress,
           'encoding': encoding,
           'memory_target': memory_target,
           'factor': (tuple(factor) if factor else None),
           'sparse': bool(sparse),
+          'encoding_level': encoding_level,
         },
         'by': operator_contact(),
         'date': strftime('%Y-%m-%d %H:%M %Z'),
       }
 
       dest_vol = CloudVolume(dest_layer_path)
       dest_vol.provenance.sources = [ src_layer_path ]
```

### Comparing `igneous-pipeline-4.8.0/igneous/task_creation/mesh.py` & `igneous-pipeline-4.9.0/igneous/task_creation/mesh.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/task_creation/obsolete.py` & `igneous-pipeline-4.9.0/igneous/task_creation/obsolete.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/task_creation/skeleton.py` & `igneous-pipeline-4.9.0/igneous/task_creation/skeleton.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/task_execution.py` & `igneous-pipeline-4.9.0/igneous/task_execution.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/__init__.py` & `igneous-pipeline-4.9.0/igneous/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/image/ccl.py` & `igneous-pipeline-4.9.0/igneous/tasks/image/ccl.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/image/image.py` & `igneous-pipeline-4.9.0/igneous/tasks/image/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
   delete_black_uploads=False,
   background_color=0,
   sparse=False,
   axis='z',
   agglomerate=False,
   timestamp=None,
   compress='gzip',
-  factor=None
+  factor=None,
 ):
   """
   Transfer an image to a new location while enabling
   rechunking, translation, reencoding, recompressing,
   and downsampling. For graphene, we can also generate
   proofread segmentation using the agglomerate flag.
   """
@@ -396,15 +396,15 @@
   src_cv = CloudVolume(
     src_path, fill_missing=fill_missing,
     mip=mip, bounded=False
   )
   dest_cv = CloudVolume(
     dest_path, fill_missing=fill_missing,
     mip=mip, delete_black_uploads=delete_black_uploads,
-    background_color=background_color, compress=compress
+    background_color=background_color, compress=compress,
   )
 
   dst_bbox = Bbox(offset, shape + offset)
   dst_bbox = Bbox.clamp(dst_bbox, dest_cv.bounds)
 
   if (
     skip_downsamples
@@ -500,15 +500,15 @@
     src_path, fill_missing=fill_missing, 
     mip=mip, bounded=False
   )
   dst_vol = CloudVolume(
     dst_path,
     fill_missing=fill_missing,
     mip=mip,
-    compress=None
+    compress=None,
   )
 
   dst_bbox = Bbox(offset, offset + shape)
   dst_bbox = Bbox.clamp(dst_bbox, dst_vol.meta.bounds(mip))
   dst_bbox = dst_bbox.expand_to_chunk_size(
     dst_vol.meta.chunk_size(mip), 
     offset=dst_vol.meta.voxel_offset(mip)
```

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/image/obsolete.py` & `igneous-pipeline-4.9.0/igneous/tasks/image/obsolete.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/mesh/draco.py` & `igneous-pipeline-4.9.0/igneous/tasks/mesh/draco.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/mesh/mesh.py` & `igneous-pipeline-4.9.0/igneous/tasks/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/mesh/mesh_graphene_remap.py` & `igneous-pipeline-4.9.0/igneous/tasks/mesh/mesh_graphene_remap.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/mesh/multires.py` & `igneous-pipeline-4.9.0/igneous/tasks/mesh/multires.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/skeleton.py` & `igneous-pipeline-4.9.0/igneous/tasks/skeleton.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/spatial_index.py` & `igneous-pipeline-4.9.0/igneous/tasks/spatial_index.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous/tasks/watershed.py` & `igneous-pipeline-4.9.0/igneous/tasks/watershed.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous_cli/LICENSE` & `igneous-pipeline-4.9.0/igneous_cli/LICENSE`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous_cli/cli.py` & `igneous-pipeline-4.9.0/igneous_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 class CloudPath(click.ParamType):
   name = "CloudPath"
   def convert(self, value, param, ctx):
     return cloudfiles.paths.normalize(value)
 
 @click.group()
 @click.option("-p", "--parallel", default=1, help="Run with this number of parallel processes. If 0, use number of cores.")
-@click.version_option(version="4.8.0")
+@click.version_option(version="4.9.0")
 @click.pass_context
 def main(ctx, parallel):
   """
   CLI tool for managing igneous jobs.
   https://github.com/seung-lab/igneous
 
   Igneous is a tool for producing neuroglancer
@@ -208,14 +208,15 @@
 @click.option('--mip', default=0, help="Build upward from this level of the image pyramid.", show_default=True)
 @click.option('--translate', type=Tuple3(), default=(0, 0, 0), help="Translate the bounding box by X,Y,Z voxels in the new location.")
 @click.option('--downsample/--skip-downsample', is_flag=True, default=True, help="Whether or not to produce downsamples from transfer tiles.", show_default=True)
 @click.option('--fill-missing', is_flag=True, default=False, help="Interpret missing image files as background instead of failing.")
 @click.option('--memory', default=3.5e9, type=int, help="Task memory limit in bytes. Task shape will be chosen to fit and maximize downsamples.", show_default=True)
 @click.option('--max-mips', default=5, help="Maximum number of additional pyramid levels.", show_default=True)
 @click.option('--encoding', default="raw", help="Which image encoding to use. Options: [all] raw, png; [images] jpeg; [segmentations] cseg, compresso; [floats] fpzip, kempressed", show_default=True)
+@click.option('--encoding-level', default=None, help="For some encodings (png level,jpeg quality,fpzip precision) a simple scalar value can adjust the compression efficiency.", show_default=True)
 @click.option('--sparse', is_flag=True, default=False, help="Don't count black pixels in mode or average calculations. For images, eliminates edge ghosting in 2x2x2 downsample. For segmentation, prevents small objects from disappearing at high mip levels.")
 @click.option('--shape', type=Tuple3(), default=(2048, 2048, 64), help="(overrides --memory) Set the task shape in voxels. This also determines how many downsamples you get. e.g. 2048,2048,64")
 @click.option('--chunk-size', type=Tuple3(), default=None, help="Chunk size of destination layer. e.g. 128,128,64")
 @click.option('--compress', default="gzip", help="Set the image compression scheme. Options: 'none', 'gzip', 'br'", show_default=True)
 @click.option('--volumetric', is_flag=True, default=False, help="Use 2x2x2 downsampling.")
 @click.option('--delete-bg', is_flag=True, default=False, help="Issue a delete instead of uploading a background tile. This is helpful on systems that don't like tiny files.")
 @click.option('--bg-color', default=0, help="Determines which color is regarded as background.", show_default=True)
@@ -224,15 +225,15 @@
 @click.option('--clean-info', is_flag=True, default=False, help="Scrub info file of mesh and skeleton fields.", show_default=True)
 @click.option('--no-src-update', is_flag=True, default=False, help="Don't update the source provenance file with the transfer metadata.", show_default=True)
 @click.pass_context
 def xfer(
 	ctx, src, dest, queue, translate, 
   downsample, mip, fill_missing, 
   memory, max_mips, shape, sparse, 
-  encoding, chunk_size, compress, 
+  encoding, encoding_level, chunk_size, compress,
   volumetric, delete_bg, bg_color, sharded,
   dest_voxel_offset, clean_info, no_src_update
 ):
   """
   Copy, re-encode, or shard an image layer.
 
   It is crucial to choose a good task shape. The task
@@ -261,26 +262,28 @@
     compress = False
 
   if sharded:
     tasks = tc.create_image_shard_transfer_tasks(
       src, dest,
       chunk_size=chunk_size, fill_missing=fill_missing, mip=mip, 
       dest_voxel_offset=dest_voxel_offset, translate=translate, 
-      encoding=encoding, memory_target=memory, clean_info=clean_info
+      encoding=encoding, memory_target=memory, clean_info=clean_info,
+      encoding_level=encoding_level,
     )
   else:
     tasks = tc.create_transfer_tasks(
       src, dest, 
       chunk_size=chunk_size, fill_missing=fill_missing, 
       dest_voxel_offset=dest_voxel_offset, translate=translate, 
       mip=mip, shape=shape, encoding=encoding, skip_downsamples=(not downsample),
       delete_black_uploads=delete_bg, background_color=bg_color,
       compress=compress, factor=factor, sparse=sparse,
       memory_target=memory, max_mips=max_mips, 
-      clean_info=clean_info, no_src_update=no_src_update
+      clean_info=clean_info, no_src_update=no_src_update,
+      encoding_level=encoding_level,
     )
 
   parallel = int(ctx.obj.get("parallel", 1))
   tq = TaskQueue(normalize_path(queue))
   tq.insert(tasks, parallel=parallel)
 
 @imagegroup.group("contrast")
```

### Comparing `igneous-pipeline-4.8.0/igneous_cli/humanbytes.py` & `igneous-pipeline-4.9.0/igneous_cli/humanbytes.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/igneous_pipeline.egg-info/PKG-INFO` & `igneous-pipeline-4.9.0/igneous_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igneous-pipeline
-Version: 4.8.0
+Version: 4.9.0
 Summary: Downsample, Mesh, Skeletonize, and Remap Neuroglancer Datasets
 Home-page: https://github.com/seung-lab/igneous/
 Author: Ignacio Tartavull, William Silversmith, and others
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description: [![PyPI version](https://badge.fury.io/py/igneous-pipeline.svg)](https://badge.fury.io/py/igneous-pipeline) [![SfN 2018 Poster](https://img.shields.io/badge/poster-SfN%202018-blue.svg)](https://drive.google.com/open?id=1RKtaAGV2f7F13opnkQfbp6YBqmoD3fZi)
```

### Comparing `igneous-pipeline-4.8.0/igneous_pipeline.egg-info/SOURCES.txt` & `igneous-pipeline-4.9.0/igneous_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/setup.cfg` & `igneous-pipeline-4.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/downsample_scales_test.py` & `igneous-pipeline-4.9.0/test/downsample_scales_test.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/layer_harness.py` & `igneous-pipeline-4.9.0/test/layer_harness.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/test_ccl_tasks.py` & `igneous-pipeline-4.9.0/test/test_ccl_tasks.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/test_shards.py` & `igneous-pipeline-4.9.0/test/test_shards.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/test_tasks.py` & `igneous-pipeline-4.9.0/test/test_tasks.py`

 * *Files identical despite different names*

### Comparing `igneous-pipeline-4.8.0/test/test_transfer_tasks.py` & `igneous-pipeline-4.9.0/test/test_transfer_tasks.py`

 * *Files identical despite different names*

