# Comparing `tmp/hpccm-23.3.0.tar.gz` & `tmp/hpccm-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hpccm-23.3.0.tar", last modified: Thu Mar 16 19:23:49 2023, max compression
+gzip compressed data, was "dist/hpccm-23.5.0.tar", last modified: Tue May  2 15:36:02 2023, max compression
```

## Comparing `hpccm-23.3.0.tar` & `hpccm-23.5.0.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/docs/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3181 2020-04-28 20:06:10.000000 hpccm-23.3.0/docs/README.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)   153466 2023-02-02 21:29:48.000000 hpccm-23.3.0/docs/building_blocks.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      399 2018-12-18 16:07:47.000000 hpccm-23.3.0/docs/citation.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3252 2019-10-29 18:54:25.000000 hpccm-23.3.0/docs/getting_started.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5619 2022-05-20 18:47:16.000000 hpccm-23.3.0/docs/misc_api.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10438 2023-02-02 21:29:48.000000 hpccm-23.3.0/docs/primitives.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13267 2019-05-28 19:27:13.000000 hpccm-23.3.0/docs/recipes.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    24213 2021-03-23 16:46:35.000000 hpccm-23.3.0/docs/tutorial.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3595 2019-05-28 19:27:13.000000 hpccm-23.3.0/docs/workflows.md
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm/
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm/building_blocks/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4546 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/__init__.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5713 2020-07-31 18:46:09.000000 hpccm-23.3.0/hpccm/building_blocks/amgx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9036 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/apt_get.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15988 2022-04-29 21:06:35.000000 hpccm-23.3.0/hpccm/building_blocks/arm_allinea_studio.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2171 2020-07-31 18:46:09.000000 hpccm-23.3.0/hpccm/building_blocks/base.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8810 2021-06-30 22:07:43.000000 hpccm-23.3.0/hpccm/building_blocks/boost.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11225 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/catalyst.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7122 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/cgns.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9408 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/charm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8221 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/cmake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8769 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/conda.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7929 2021-09-30 21:58:46.000000 hpccm-23.3.0/hpccm/building_blocks/fftw.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5794 2021-04-30 19:29:17.000000 hpccm-23.3.0/hpccm/building_blocks/gdrcopy.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14416 2021-01-29 22:43:41.000000 hpccm-23.3.0/hpccm/building_blocks/generic_autotools.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10687 2021-01-29 22:43:41.000000 hpccm-23.3.0/hpccm/building_blocks/generic_build.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14323 2021-01-29 22:43:41.000000 hpccm-23.3.0/hpccm/building_blocks/generic_cmake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    20653 2022-10-12 21:08:01.000000 hpccm-23.3.0/hpccm/building_blocks/gnu.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9479 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/hdf5.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17680 2022-08-11 21:55:16.000000 hpccm-23.3.0/hpccm/building_blocks/hpcx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8404 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/building_blocks/intel_mpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    18189 2021-06-02 19:31:54.000000 hpccm-23.3.0/hpccm/building_blocks/intel_psxe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14815 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/intel_psxe_runtime.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9327 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/julia.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3751 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/knem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8703 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/kokkos.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11500 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/libsim.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17818 2023-03-16 19:22:01.000000 hpccm-23.3.0/hpccm/building_blocks/llvm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4881 2020-07-31 18:46:09.000000 hpccm-23.3.0/hpccm/building_blocks/magma.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7204 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/building_blocks/mkl.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11095 2022-05-20 18:47:16.000000 hpccm-23.3.0/hpccm/building_blocks/mlnx_ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8511 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/mpich.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6822 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/multi_ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13788 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/mvapich2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13762 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/mvapich2_gdr.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10691 2022-04-29 21:06:35.000000 hpccm-23.3.0/hpccm/building_blocks/nccl.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10571 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/netcdf.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9381 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/nsight_compute.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5498 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/nsight_systems.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    26706 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/nvhpc.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9202 2021-08-31 22:19:51.000000 hpccm-23.3.0/hpccm/building_blocks/nvshmem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10416 2022-05-20 18:47:16.000000 hpccm-23.3.0/hpccm/building_blocks/ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5926 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/building_blocks/openblas.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15723 2022-04-29 21:06:35.000000 hpccm-23.3.0/hpccm/building_blocks/openmpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7953 2022-10-12 21:08:01.000000 hpccm-23.3.0/hpccm/building_blocks/packages.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    19043 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/pgi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6551 2021-01-29 22:43:41.000000 hpccm-23.3.0/hpccm/building_blocks/pip.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7160 2022-04-29 21:06:35.000000 hpccm-23.3.0/hpccm/building_blocks/pmix.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8400 2021-02-26 19:22:07.000000 hpccm-23.3.0/hpccm/building_blocks/pnetcdf.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3739 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/building_blocks/python.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9309 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/building_blocks/rdma_core.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9165 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/building_blocks/scif.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6256 2020-07-31 18:46:09.000000 hpccm-23.3.0/hpccm/building_blocks/sensei.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5711 2022-05-20 18:47:16.000000 hpccm-23.3.0/hpccm/building_blocks/slurm_pmi2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    16816 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/building_blocks/ucx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5966 2021-10-29 20:37:56.000000 hpccm-23.3.0/hpccm/building_blocks/xpmem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10120 2021-04-30 19:29:17.000000 hpccm-23.3.0/hpccm/building_blocks/yum.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm/primitives/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1263 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/primitives/__init__.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8209 2023-02-02 21:29:48.000000 hpccm-23.3.0/hpccm/primitives/baseimage.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2853 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/primitives/blob.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3393 2019-03-29 14:45:09.000000 hpccm-23.3.0/hpccm/primitives/comment.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11118 2021-03-31 20:07:58.000000 hpccm-23.3.0/hpccm/primitives/copy.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5641 2019-05-01 03:09:48.000000 hpccm-23.3.0/hpccm/primitives/environment.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4064 2019-05-01 03:09:48.000000 hpccm-23.3.0/hpccm/primitives/label.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2359 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/primitives/raw.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5098 2019-05-01 03:09:48.000000 hpccm-23.3.0/hpccm/primitives/runscript.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6983 2021-03-31 20:07:58.000000 hpccm-23.3.0/hpccm/primitives/shell.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1908 2019-05-01 03:09:48.000000 hpccm-23.3.0/hpccm/primitives/user.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2267 2019-05-01 03:09:48.000000 hpccm-23.3.0/hpccm/primitives/workdir.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm/templates/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5461 2020-04-28 20:06:10.000000 hpccm-23.3.0/hpccm/templates/CMakeBuild.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6616 2020-04-28 20:06:10.000000 hpccm-23.3.0/hpccm/templates/ConfigureMake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1167 2020-06-10 19:13:37.000000 hpccm-23.3.0/hpccm/templates/__init__.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1736 2020-04-28 20:06:10.000000 hpccm-23.3.0/hpccm/templates/annotate.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5728 2021-03-31 20:07:58.000000 hpccm-23.3.0/hpccm/templates/downloader.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1962 2020-02-19 15:04:04.000000 hpccm-23.3.0/hpccm/templates/envvars.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4658 2020-09-30 21:37:04.000000 hpccm-23.3.0/hpccm/templates/git.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1512 2019-06-27 16:08:46.000000 hpccm-23.3.0/hpccm/templates/ldconfig.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1310 2019-03-08 22:45:08.000000 hpccm-23.3.0/hpccm/templates/rm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1921 2019-03-08 22:45:08.000000 hpccm-23.3.0/hpccm/templates/sed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2217 2020-06-10 19:13:37.000000 hpccm-23.3.0/hpccm/templates/tar.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2077 2020-04-28 20:06:10.000000 hpccm-23.3.0/hpccm/templates/wget.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1495 2020-06-10 19:13:37.000000 hpccm-23.3.0/hpccm/templates/zipfile.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4590 2020-01-23 16:41:20.000000 hpccm-23.3.0/hpccm/Stage.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1377 2020-03-26 20:56:16.000000 hpccm-23.3.0/hpccm/__init__.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1474 2019-03-08 22:45:08.000000 hpccm-23.3.0/hpccm/base_object.py
--rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3730 2021-06-02 19:31:54.000000 hpccm-23.3.0/hpccm/cli.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1125 2021-06-30 22:07:43.000000 hpccm-23.3.0/hpccm/common.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8411 2022-05-20 18:47:16.000000 hpccm-23.3.0/hpccm/config.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6654 2022-03-01 20:21:56.000000 hpccm-23.3.0/hpccm/recipe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2779 2020-12-18 20:51:16.000000 hpccm-23.3.0/hpccm/toolchain.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      674 2023-03-16 19:22:01.000000 hpccm-23.3.0/hpccm/version.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4250 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/PKG-INFO
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5876 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/SOURCES.txt
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        1 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/dependency_links.txt
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/entry_points.txt
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       47 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/requires.txt
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        6 2023-03-16 19:23:49.000000 hpccm-23.3.0/hpccm.egg-info/top_level.txt
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/examples/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      343 2021-03-23 16:46:35.000000 hpccm-23.3.0/recipes/examples/basic.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      397 2020-03-26 20:56:16.000000 hpccm-23.3.0/recipes/examples/cloverleaf.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      400 2020-03-26 20:56:16.000000 hpccm-23.3.0/recipes/examples/gnu-devel.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      721 2021-03-23 16:46:35.000000 hpccm-23.3.0/recipes/examples/multistage.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1504 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/examples/scif.py
--rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     2320 2020-10-30 18:46:31.000000 hpccm-23.3.0/recipes/examples/script.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      722 2021-03-23 16:46:35.000000 hpccm-23.3.0/recipes/examples/userargs.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/gromacs/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1651 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/gromacs/gromacs.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/hpccm/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      402 2019-03-08 22:44:59.000000 hpccm-23.3.0/recipes/hpccm/Dockerfile
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      785 2019-03-08 22:44:59.000000 hpccm-23.3.0/recipes/hpccm/README.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      420 2019-03-08 22:44:59.000000 hpccm-23.3.0/recipes/hpccm/Singularity.def
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      858 2019-03-08 22:44:59.000000 hpccm-23.3.0/recipes/hpccm/bootstrap.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/jupyter/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       27 2019-11-14 20:32:35.000000 hpccm-23.3.0/recipes/jupyter/.gitignore
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1386 2020-03-26 20:56:16.000000 hpccm-23.3.0/recipes/jupyter/README.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       63 2019-11-14 20:32:35.000000 hpccm-23.3.0/recipes/jupyter/environment.yml
--rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3203 2020-06-10 19:13:37.000000 hpccm-23.3.0/recipes/jupyter/jupyter.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      733 2019-11-14 20:32:35.000000 hpccm-23.3.0/recipes/jupyter/notebook.ipynb
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        6 2019-11-14 20:32:35.000000 hpccm-23.3.0/recipes/jupyter/requirements.txt
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/lammps/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4878 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/lammps/lammps.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/milc/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3809 2022-03-01 20:21:56.000000 hpccm-23.3.0/recipes/milc/milc.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/recipes/osu_benchmarks/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1091 2021-03-31 20:07:58.000000 hpccm-23.3.0/recipes/osu_benchmarks/README.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2735 2022-05-20 18:47:16.000000 hpccm-23.3.0/recipes/osu_benchmarks/common.py
--rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3511 2021-03-31 20:07:58.000000 hpccm-23.3.0/recipes/osu_benchmarks/entrypoint.sh
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      783 2021-03-31 20:07:58.000000 hpccm-23.3.0/recipes/osu_benchmarks/osu_benchmarks.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1967 2022-03-01 20:21:56.000000 hpccm-23.3.0/recipes/easybuild.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1302 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/hpcbase-gnu-mvapich2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1300 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/hpcbase-gnu-openmpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2146 2022-03-01 20:21:56.000000 hpccm-23.3.0/recipes/hpcbase-nvhpc-mvapich2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2208 2022-03-01 20:21:56.000000 hpccm-23.3.0/recipes/hpcbase-nvhpc-openmpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1787 2021-03-23 16:46:35.000000 hpccm-23.3.0/recipes/mpi_bandwidth.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2749 2021-08-31 22:19:51.000000 hpccm-23.3.0/recipes/nvhpc.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1731 2020-12-18 20:51:16.000000 hpccm-23.3.0/recipes/spack.py
-drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-03-16 19:23:49.000000 hpccm-23.3.0/test/
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      126 2018-03-24 23:12:02.000000 hpccm-23.3.0/test/bad_recipe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       21 2018-03-24 23:12:02.000000 hpccm-23.3.0/test/docker.blob
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      162 2018-10-30 13:57:27.000000 hpccm-23.3.0/test/global_vars_recipe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6893 2022-05-20 18:47:16.000000 hpccm-23.3.0/test/helpers.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2020-03-26 20:56:16.000000 hpccm-23.3.0/test/include1.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       48 2020-03-26 20:56:16.000000 hpccm-23.3.0/test/include2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2020-03-26 20:56:16.000000 hpccm-23.3.0/test/include3.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       34 2018-03-24 23:12:02.000000 hpccm-23.3.0/test/singularity.blob
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4958 2019-03-08 22:45:08.000000 hpccm-23.3.0/test/test_CMakeBuild.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4858 2020-02-19 15:04:04.000000 hpccm-23.3.0/test/test_ConfigureMake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5515 2020-01-23 16:41:20.000000 hpccm-23.3.0/test/test_Stage.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4695 2020-06-10 19:13:37.000000 hpccm-23.3.0/test/test_amgx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2368 2020-04-28 20:06:10.000000 hpccm-23.3.0/test/test_annotate.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4187 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_apt_get.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7881 2022-04-29 21:06:35.000000 hpccm-23.3.0/test/test_arm_allinea_studio.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12797 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_baseimage.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3036 2020-07-31 18:46:09.000000 hpccm-23.3.0/test/test_bb_base.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3628 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_blob.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7879 2021-06-30 22:07:43.000000 hpccm-23.3.0/test/test_boost.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9286 2019-07-25 15:00:43.000000 hpccm-23.3.0/test/test_catalyst.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3177 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_cgns.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6433 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_charm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1415 2018-05-22 15:48:34.000000 hpccm-23.3.0/test/test_cli.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8378 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_cmake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2864 2019-03-29 14:45:09.000000 hpccm-23.3.0/test/test_comment.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8077 2020-10-07 22:36:15.000000 hpccm-23.3.0/test/test_conda.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9796 2021-06-30 22:07:43.000000 hpccm-23.3.0/test/test_config.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8581 2021-03-31 20:07:58.000000 hpccm-23.3.0/test/test_copy.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5207 2020-07-31 18:46:09.000000 hpccm-23.3.0/test/test_downloader.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5526 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_environment.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2280 2019-07-25 15:00:43.000000 hpccm-23.3.0/test/test_envvars.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7811 2021-09-30 21:58:46.000000 hpccm-23.3.0/test/test_fftw.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8199 2021-04-30 19:29:17.000000 hpccm-23.3.0/test/test_gdrcopy.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10171 2021-01-29 22:43:41.000000 hpccm-23.3.0/test/test_generic_autotools.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8030 2021-01-29 22:43:41.000000 hpccm-23.3.0/test/test_generic_build.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15782 2021-01-29 22:43:41.000000 hpccm-23.3.0/test/test_generic_cmake.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8455 2020-06-10 19:13:37.000000 hpccm-23.3.0/test/test_git.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      616 2018-10-30 13:57:06.000000 hpccm-23.3.0/test/test_global_vars.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12004 2022-10-12 21:08:01.000000 hpccm-23.3.0/test/test_gnu.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4936 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_hdf5.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17443 2022-08-11 21:55:16.000000 hpccm-23.3.0/test/test_hpcx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6331 2020-02-19 15:04:04.000000 hpccm-23.3.0/test/test_intel_mpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10313 2021-06-02 19:31:54.000000 hpccm-23.3.0/test/test_intel_psxe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5683 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_intel_psxe_runtime.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5414 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_julia.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2689 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_knem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5925 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_kokkos.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3957 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_label.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1444 2019-01-24 22:39:40.000000 hpccm-23.3.0/test/test_ldconfig.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6402 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_libsim.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15008 2023-03-16 19:22:01.000000 hpccm-23.3.0/test/test_llvm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3703 2020-04-28 20:06:10.000000 hpccm-23.3.0/test/test_magma.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5612 2020-02-19 15:04:04.000000 hpccm-23.3.0/test/test_mkl.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12043 2021-06-30 22:07:43.000000 hpccm-23.3.0/test/test_mlnx_ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4723 2020-04-28 20:06:10.000000 hpccm-23.3.0/test/test_mpich.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11005 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_multi_ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11767 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_mvapich2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9403 2021-04-30 19:29:17.000000 hpccm-23.3.0/test/test_mvapich2_gdr.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8824 2022-04-29 21:06:35.000000 hpccm-23.3.0/test/test_nccl.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7773 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_netcdf.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9130 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_nsight_compute.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6999 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_nsight_systems.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    18719 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_nvhpc.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7177 2021-08-31 22:19:51.000000 hpccm-23.3.0/test/test_nvshmem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8343 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_ofed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5417 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_openblas.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11425 2022-04-29 21:06:35.000000 hpccm-23.3.0/test/test_openmpi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1997 2019-05-28 19:27:13.000000 hpccm-23.3.0/test/test_packages.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9987 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_pgi.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5026 2021-01-29 22:43:41.000000 hpccm-23.3.0/test/test_pip.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3606 2022-04-29 21:06:35.000000 hpccm-23.3.0/test/test_pmix.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4270 2021-02-26 19:22:07.000000 hpccm-23.3.0/test/test_pnetcdf.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2787 2019-10-25 13:52:27.000000 hpccm-23.3.0/test/test_python.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2843 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_raw.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7171 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_rdma_core.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9487 2023-02-02 21:29:48.000000 hpccm-23.3.0/test/test_recipe.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1331 2018-08-22 16:55:49.000000 hpccm-23.3.0/test/test_rm.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3836 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_runscript.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6076 2021-06-30 22:07:43.000000 hpccm-23.3.0/test/test_scif.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1626 2018-07-17 14:54:11.000000 hpccm-23.3.0/test/test_sed.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3413 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_sensei.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5423 2019-08-30 03:36:17.000000 hpccm-23.3.0/test/test_shell.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3245 2022-05-20 18:47:16.000000 hpccm-23.3.0/test/test_slurm_pmi2.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2495 2020-06-10 19:13:37.000000 hpccm-23.3.0/test/test_tar.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2357 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_toolchain.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13833 2020-09-30 21:37:04.000000 hpccm-23.3.0/test/test_ucx.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1856 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_user.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2807 2018-07-17 14:54:11.000000 hpccm-23.3.0/test/test_wget.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1982 2019-05-01 03:09:48.000000 hpccm-23.3.0/test/test_workdir.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4340 2021-10-29 20:37:56.000000 hpccm-23.3.0/test/test_xpmem.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5349 2020-12-18 20:51:16.000000 hpccm-23.3.0/test/test_yum.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1507 2020-06-10 19:13:37.000000 hpccm-23.3.0/test/test_zipfile.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    16848 2023-03-16 19:22:01.000000 hpccm-23.3.0/CHANGELOG.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11357 2018-03-24 23:12:02.000000 hpccm-23.3.0/LICENSE
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      296 2020-03-26 20:56:16.000000 hpccm-23.3.0/MANIFEST.in
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3181 2020-04-28 20:06:10.000000 hpccm-23.3.0/README.md
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1480 2021-06-02 19:38:54.000000 hpccm-23.3.0/setup.py
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4250 2023-03-16 19:23:49.000000 hpccm-23.3.0/PKG-INFO
--rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       38 2023-03-16 19:23:49.000000 hpccm-23.3.0/setup.cfg
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/docs/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3181 2020-04-28 20:06:10.000000 hpccm-23.5.0/docs/README.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)   153694 2023-05-02 15:35:31.000000 hpccm-23.5.0/docs/building_blocks.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      399 2018-12-18 16:07:47.000000 hpccm-23.5.0/docs/citation.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3252 2019-10-29 18:54:25.000000 hpccm-23.5.0/docs/getting_started.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5619 2022-05-20 18:47:16.000000 hpccm-23.5.0/docs/misc_api.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10438 2023-02-02 21:29:48.000000 hpccm-23.5.0/docs/primitives.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13267 2019-05-28 19:27:13.000000 hpccm-23.5.0/docs/recipes.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    24213 2021-03-23 16:46:35.000000 hpccm-23.5.0/docs/tutorial.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3595 2019-05-28 19:27:13.000000 hpccm-23.5.0/docs/workflows.md
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm/
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm/building_blocks/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4546 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/__init__.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5713 2020-07-31 18:46:09.000000 hpccm-23.5.0/hpccm/building_blocks/amgx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9036 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/apt_get.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15988 2022-04-29 21:06:35.000000 hpccm-23.5.0/hpccm/building_blocks/arm_allinea_studio.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2171 2020-07-31 18:46:09.000000 hpccm-23.5.0/hpccm/building_blocks/base.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8810 2021-06-30 22:07:43.000000 hpccm-23.5.0/hpccm/building_blocks/boost.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11225 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/catalyst.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7122 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/cgns.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9408 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/charm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8221 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/cmake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8854 2023-05-02 15:35:31.000000 hpccm-23.5.0/hpccm/building_blocks/conda.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7929 2021-09-30 21:58:46.000000 hpccm-23.5.0/hpccm/building_blocks/fftw.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5794 2021-04-30 19:29:17.000000 hpccm-23.5.0/hpccm/building_blocks/gdrcopy.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14749 2023-05-02 15:35:31.000000 hpccm-23.5.0/hpccm/building_blocks/generic_autotools.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10687 2021-01-29 22:43:41.000000 hpccm-23.5.0/hpccm/building_blocks/generic_build.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14323 2021-01-29 22:43:41.000000 hpccm-23.5.0/hpccm/building_blocks/generic_cmake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    20653 2022-10-12 21:08:01.000000 hpccm-23.5.0/hpccm/building_blocks/gnu.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9479 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/hdf5.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17680 2022-08-11 21:55:16.000000 hpccm-23.5.0/hpccm/building_blocks/hpcx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8404 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/building_blocks/intel_mpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    18189 2021-06-02 19:31:54.000000 hpccm-23.5.0/hpccm/building_blocks/intel_psxe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    14815 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/intel_psxe_runtime.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9327 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/julia.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3751 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/knem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8703 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/kokkos.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11500 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/libsim.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17818 2023-03-16 19:22:01.000000 hpccm-23.5.0/hpccm/building_blocks/llvm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4881 2020-07-31 18:46:09.000000 hpccm-23.5.0/hpccm/building_blocks/magma.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7204 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/building_blocks/mkl.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11095 2022-05-20 18:47:16.000000 hpccm-23.5.0/hpccm/building_blocks/mlnx_ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8511 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/mpich.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6822 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/multi_ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13788 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/mvapich2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13762 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/mvapich2_gdr.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10691 2022-04-29 21:06:35.000000 hpccm-23.5.0/hpccm/building_blocks/nccl.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10571 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/netcdf.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9381 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/nsight_compute.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5498 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/nsight_systems.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    26706 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/nvhpc.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9202 2021-08-31 22:19:51.000000 hpccm-23.5.0/hpccm/building_blocks/nvshmem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10416 2022-05-20 18:47:16.000000 hpccm-23.5.0/hpccm/building_blocks/ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5926 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/building_blocks/openblas.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15723 2022-04-29 21:06:35.000000 hpccm-23.5.0/hpccm/building_blocks/openmpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7953 2022-10-12 21:08:01.000000 hpccm-23.5.0/hpccm/building_blocks/packages.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    19043 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/pgi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6551 2021-01-29 22:43:41.000000 hpccm-23.5.0/hpccm/building_blocks/pip.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7160 2022-04-29 21:06:35.000000 hpccm-23.5.0/hpccm/building_blocks/pmix.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8400 2021-02-26 19:22:07.000000 hpccm-23.5.0/hpccm/building_blocks/pnetcdf.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4285 2023-05-02 15:35:31.000000 hpccm-23.5.0/hpccm/building_blocks/python.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9309 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/building_blocks/rdma_core.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9165 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/building_blocks/scif.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6256 2020-07-31 18:46:09.000000 hpccm-23.5.0/hpccm/building_blocks/sensei.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5711 2022-05-20 18:47:16.000000 hpccm-23.5.0/hpccm/building_blocks/slurm_pmi2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    16816 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/building_blocks/ucx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5966 2021-10-29 20:37:56.000000 hpccm-23.5.0/hpccm/building_blocks/xpmem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10120 2021-04-30 19:29:17.000000 hpccm-23.5.0/hpccm/building_blocks/yum.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm/primitives/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1263 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/primitives/__init__.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8209 2023-02-02 21:29:48.000000 hpccm-23.5.0/hpccm/primitives/baseimage.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2853 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/primitives/blob.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3393 2019-03-29 14:45:09.000000 hpccm-23.5.0/hpccm/primitives/comment.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11118 2021-03-31 20:07:58.000000 hpccm-23.5.0/hpccm/primitives/copy.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5641 2019-05-01 03:09:48.000000 hpccm-23.5.0/hpccm/primitives/environment.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4064 2019-05-01 03:09:48.000000 hpccm-23.5.0/hpccm/primitives/label.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2359 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/primitives/raw.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5098 2019-05-01 03:09:48.000000 hpccm-23.5.0/hpccm/primitives/runscript.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6983 2021-03-31 20:07:58.000000 hpccm-23.5.0/hpccm/primitives/shell.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1908 2019-05-01 03:09:48.000000 hpccm-23.5.0/hpccm/primitives/user.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2267 2019-05-01 03:09:48.000000 hpccm-23.5.0/hpccm/primitives/workdir.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm/templates/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5461 2020-04-28 20:06:10.000000 hpccm-23.5.0/hpccm/templates/CMakeBuild.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6777 2023-05-02 15:35:31.000000 hpccm-23.5.0/hpccm/templates/ConfigureMake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1167 2020-06-10 19:13:37.000000 hpccm-23.5.0/hpccm/templates/__init__.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1736 2020-04-28 20:06:10.000000 hpccm-23.5.0/hpccm/templates/annotate.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5728 2021-03-31 20:07:58.000000 hpccm-23.5.0/hpccm/templates/downloader.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1962 2020-02-19 15:04:04.000000 hpccm-23.5.0/hpccm/templates/envvars.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4658 2020-09-30 21:37:04.000000 hpccm-23.5.0/hpccm/templates/git.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1512 2019-06-27 16:08:46.000000 hpccm-23.5.0/hpccm/templates/ldconfig.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1310 2019-03-08 22:45:08.000000 hpccm-23.5.0/hpccm/templates/rm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1921 2019-03-08 22:45:08.000000 hpccm-23.5.0/hpccm/templates/sed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2217 2020-06-10 19:13:37.000000 hpccm-23.5.0/hpccm/templates/tar.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2077 2020-04-28 20:06:10.000000 hpccm-23.5.0/hpccm/templates/wget.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1495 2020-06-10 19:13:37.000000 hpccm-23.5.0/hpccm/templates/zipfile.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4590 2020-01-23 16:41:20.000000 hpccm-23.5.0/hpccm/Stage.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1377 2020-03-26 20:56:16.000000 hpccm-23.5.0/hpccm/__init__.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1474 2019-03-08 22:45:08.000000 hpccm-23.5.0/hpccm/base_object.py
+-rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3730 2021-06-02 19:31:54.000000 hpccm-23.5.0/hpccm/cli.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1125 2021-06-30 22:07:43.000000 hpccm-23.5.0/hpccm/common.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8411 2022-05-20 18:47:16.000000 hpccm-23.5.0/hpccm/config.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6654 2022-03-01 20:21:56.000000 hpccm-23.5.0/hpccm/recipe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2779 2020-12-18 20:51:16.000000 hpccm-23.5.0/hpccm/toolchain.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      674 2023-05-02 15:35:31.000000 hpccm-23.5.0/hpccm/version.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4250 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/PKG-INFO
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5876 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/SOURCES.txt
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        1 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/dependency_links.txt
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/entry_points.txt
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       47 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/requires.txt
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        6 2023-05-02 15:36:02.000000 hpccm-23.5.0/hpccm.egg-info/top_level.txt
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/examples/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      343 2021-03-23 16:46:35.000000 hpccm-23.5.0/recipes/examples/basic.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      397 2020-03-26 20:56:16.000000 hpccm-23.5.0/recipes/examples/cloverleaf.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      400 2020-03-26 20:56:16.000000 hpccm-23.5.0/recipes/examples/gnu-devel.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      721 2021-03-23 16:46:35.000000 hpccm-23.5.0/recipes/examples/multistage.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1504 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/examples/scif.py
+-rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     2320 2020-10-30 18:46:31.000000 hpccm-23.5.0/recipes/examples/script.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      722 2021-03-23 16:46:35.000000 hpccm-23.5.0/recipes/examples/userargs.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/gromacs/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1651 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/gromacs/gromacs.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/hpccm/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      402 2019-03-08 22:44:59.000000 hpccm-23.5.0/recipes/hpccm/Dockerfile
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      785 2019-03-08 22:44:59.000000 hpccm-23.5.0/recipes/hpccm/README.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      420 2019-03-08 22:44:59.000000 hpccm-23.5.0/recipes/hpccm/Singularity.def
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      858 2019-03-08 22:44:59.000000 hpccm-23.5.0/recipes/hpccm/bootstrap.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/jupyter/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       27 2019-11-14 20:32:35.000000 hpccm-23.5.0/recipes/jupyter/.gitignore
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1386 2020-03-26 20:56:16.000000 hpccm-23.5.0/recipes/jupyter/README.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       63 2019-11-14 20:32:35.000000 hpccm-23.5.0/recipes/jupyter/environment.yml
+-rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3203 2020-06-10 19:13:37.000000 hpccm-23.5.0/recipes/jupyter/jupyter.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      733 2019-11-14 20:32:35.000000 hpccm-23.5.0/recipes/jupyter/notebook.ipynb
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)        6 2019-11-14 20:32:35.000000 hpccm-23.5.0/recipes/jupyter/requirements.txt
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/lammps/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4878 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/lammps/lammps.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/milc/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3809 2022-03-01 20:21:56.000000 hpccm-23.5.0/recipes/milc/milc.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/recipes/osu_benchmarks/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1091 2021-03-31 20:07:58.000000 hpccm-23.5.0/recipes/osu_benchmarks/README.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2735 2022-05-20 18:47:16.000000 hpccm-23.5.0/recipes/osu_benchmarks/common.py
+-rwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)     3511 2021-03-31 20:07:58.000000 hpccm-23.5.0/recipes/osu_benchmarks/entrypoint.sh
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      783 2021-03-31 20:07:58.000000 hpccm-23.5.0/recipes/osu_benchmarks/osu_benchmarks.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1967 2022-03-01 20:21:56.000000 hpccm-23.5.0/recipes/easybuild.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1302 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/hpcbase-gnu-mvapich2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1300 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/hpcbase-gnu-openmpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2146 2022-03-01 20:21:56.000000 hpccm-23.5.0/recipes/hpcbase-nvhpc-mvapich2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2208 2022-03-01 20:21:56.000000 hpccm-23.5.0/recipes/hpcbase-nvhpc-openmpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1787 2021-03-23 16:46:35.000000 hpccm-23.5.0/recipes/mpi_bandwidth.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2749 2021-08-31 22:19:51.000000 hpccm-23.5.0/recipes/nvhpc.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1731 2020-12-18 20:51:16.000000 hpccm-23.5.0/recipes/spack.py
+drwxr-xr-x   0 smcmillan  (1000) smcmillan  (1000)        0 2023-05-02 15:36:02.000000 hpccm-23.5.0/test/
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      126 2018-03-24 23:12:02.000000 hpccm-23.5.0/test/bad_recipe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       21 2018-03-24 23:12:02.000000 hpccm-23.5.0/test/docker.blob
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      162 2018-10-30 13:57:27.000000 hpccm-23.5.0/test/global_vars_recipe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6893 2022-05-20 18:47:16.000000 hpccm-23.5.0/test/helpers.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2020-03-26 20:56:16.000000 hpccm-23.5.0/test/include1.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       48 2020-03-26 20:56:16.000000 hpccm-23.5.0/test/include2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       42 2020-03-26 20:56:16.000000 hpccm-23.5.0/test/include3.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       34 2018-03-24 23:12:02.000000 hpccm-23.5.0/test/singularity.blob
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4958 2019-03-08 22:45:08.000000 hpccm-23.5.0/test/test_CMakeBuild.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5591 2023-05-02 15:35:31.000000 hpccm-23.5.0/test/test_ConfigureMake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5515 2020-01-23 16:41:20.000000 hpccm-23.5.0/test/test_Stage.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4695 2020-06-10 19:13:37.000000 hpccm-23.5.0/test/test_amgx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2368 2020-04-28 20:06:10.000000 hpccm-23.5.0/test/test_annotate.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4187 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_apt_get.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7881 2022-04-29 21:06:35.000000 hpccm-23.5.0/test/test_arm_allinea_studio.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12797 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_baseimage.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3036 2020-07-31 18:46:09.000000 hpccm-23.5.0/test/test_bb_base.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3628 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_blob.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7879 2021-06-30 22:07:43.000000 hpccm-23.5.0/test/test_boost.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9286 2019-07-25 15:00:43.000000 hpccm-23.5.0/test/test_catalyst.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3177 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_cgns.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6433 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_charm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1415 2018-05-22 15:48:34.000000 hpccm-23.5.0/test/test_cli.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8378 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_cmake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2864 2019-03-29 14:45:09.000000 hpccm-23.5.0/test/test_comment.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8101 2023-05-02 15:35:31.000000 hpccm-23.5.0/test/test_conda.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9796 2021-06-30 22:07:43.000000 hpccm-23.5.0/test/test_config.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8581 2021-03-31 20:07:58.000000 hpccm-23.5.0/test/test_copy.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5207 2020-07-31 18:46:09.000000 hpccm-23.5.0/test/test_downloader.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5526 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_environment.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2280 2019-07-25 15:00:43.000000 hpccm-23.5.0/test/test_envvars.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7811 2021-09-30 21:58:46.000000 hpccm-23.5.0/test/test_fftw.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8199 2021-04-30 19:29:17.000000 hpccm-23.5.0/test/test_gdrcopy.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10171 2021-01-29 22:43:41.000000 hpccm-23.5.0/test/test_generic_autotools.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8030 2021-01-29 22:43:41.000000 hpccm-23.5.0/test/test_generic_build.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15782 2021-01-29 22:43:41.000000 hpccm-23.5.0/test/test_generic_cmake.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8455 2020-06-10 19:13:37.000000 hpccm-23.5.0/test/test_git.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      616 2018-10-30 13:57:06.000000 hpccm-23.5.0/test/test_global_vars.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12004 2022-10-12 21:08:01.000000 hpccm-23.5.0/test/test_gnu.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4936 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_hdf5.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17443 2022-08-11 21:55:16.000000 hpccm-23.5.0/test/test_hpcx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6331 2020-02-19 15:04:04.000000 hpccm-23.5.0/test/test_intel_mpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    10313 2021-06-02 19:31:54.000000 hpccm-23.5.0/test/test_intel_psxe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5683 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_intel_psxe_runtime.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5414 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_julia.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2689 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_knem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5925 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_kokkos.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3957 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_label.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1444 2019-01-24 22:39:40.000000 hpccm-23.5.0/test/test_ldconfig.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6402 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_libsim.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    15008 2023-03-16 19:22:01.000000 hpccm-23.5.0/test/test_llvm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3703 2020-04-28 20:06:10.000000 hpccm-23.5.0/test/test_magma.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5612 2020-02-19 15:04:04.000000 hpccm-23.5.0/test/test_mkl.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    12043 2021-06-30 22:07:43.000000 hpccm-23.5.0/test/test_mlnx_ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4723 2020-04-28 20:06:10.000000 hpccm-23.5.0/test/test_mpich.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11005 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_multi_ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11767 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_mvapich2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9403 2021-04-30 19:29:17.000000 hpccm-23.5.0/test/test_mvapich2_gdr.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8824 2022-04-29 21:06:35.000000 hpccm-23.5.0/test/test_nccl.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7773 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_netcdf.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9130 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_nsight_compute.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6999 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_nsight_systems.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    18719 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_nvhpc.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7177 2021-08-31 22:19:51.000000 hpccm-23.5.0/test/test_nvshmem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     8343 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_ofed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5417 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_openblas.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11425 2022-04-29 21:06:35.000000 hpccm-23.5.0/test/test_openmpi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1997 2019-05-28 19:27:13.000000 hpccm-23.5.0/test/test_packages.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9987 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_pgi.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5026 2021-01-29 22:43:41.000000 hpccm-23.5.0/test/test_pip.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3606 2022-04-29 21:06:35.000000 hpccm-23.5.0/test/test_pmix.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4270 2021-02-26 19:22:07.000000 hpccm-23.5.0/test/test_pnetcdf.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3155 2023-05-02 15:35:31.000000 hpccm-23.5.0/test/test_python.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2843 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_raw.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     7171 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_rdma_core.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     9487 2023-02-02 21:29:48.000000 hpccm-23.5.0/test/test_recipe.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1331 2018-08-22 16:55:49.000000 hpccm-23.5.0/test/test_rm.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3836 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_runscript.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     6076 2021-06-30 22:07:43.000000 hpccm-23.5.0/test/test_scif.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1626 2018-07-17 14:54:11.000000 hpccm-23.5.0/test/test_sed.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3413 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_sensei.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5423 2019-08-30 03:36:17.000000 hpccm-23.5.0/test/test_shell.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3245 2022-05-20 18:47:16.000000 hpccm-23.5.0/test/test_slurm_pmi2.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2495 2020-06-10 19:13:37.000000 hpccm-23.5.0/test/test_tar.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2357 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_toolchain.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    13833 2020-09-30 21:37:04.000000 hpccm-23.5.0/test/test_ucx.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1856 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_user.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     2807 2018-07-17 14:54:11.000000 hpccm-23.5.0/test/test_wget.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1982 2019-05-01 03:09:48.000000 hpccm-23.5.0/test/test_workdir.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4340 2021-10-29 20:37:56.000000 hpccm-23.5.0/test/test_xpmem.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     5349 2020-12-18 20:51:16.000000 hpccm-23.5.0/test/test_yum.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1507 2020-06-10 19:13:37.000000 hpccm-23.5.0/test/test_zipfile.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    17210 2023-05-02 15:35:31.000000 hpccm-23.5.0/CHANGELOG.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)    11357 2018-03-24 23:12:02.000000 hpccm-23.5.0/LICENSE
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)      296 2020-03-26 20:56:16.000000 hpccm-23.5.0/MANIFEST.in
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     3181 2020-04-28 20:06:10.000000 hpccm-23.5.0/README.md
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     1480 2021-06-02 19:38:54.000000 hpccm-23.5.0/setup.py
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)     4250 2023-05-02 15:36:02.000000 hpccm-23.5.0/PKG-INFO
+-rw-r--r--   0 smcmillan  (1000) smcmillan  (1000)       38 2023-05-02 15:36:02.000000 hpccm-23.5.0/setup.cfg
```

### Comparing `hpccm-23.3.0/docs/README.md` & `hpccm-23.5.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/building_blocks.md` & `hpccm-23.5.0/docs/building_blocks.md`

 * *Files 0% similar despite different names*

```diff
@@ -594,18 +594,18 @@
 `/usr/local/anaconda`.
 
 - __python2__: Boolean flag to specify that the Python 2 version of
 Anaconda should be installed.  The default is False.
 
 - __python_subversion__: The Python version to install.  This value is
 ignored if the Conda version is less than 4.8.  The default is
-`py38` if using Python 3, and `py27` if using Python 2.
+`py310` if using Python 3, and `py27` if using Python 2.
 
 - __version__: The version of Anaconda to download.  The default value
-is `4.8.3`.
+is `23.1.0-1` if using Python 3, and `4.8.3` if using Python 2.
 
 __Examples__
 
 
 ```python
 conda(packages=['numpy'])
 ```
@@ -865,14 +865,18 @@
 `--enable-foo` and `enable_foo='yes'` maps to `--enable-foo=yes`.
 Underscores in the parameter name are converted to dashes.
 
 - __environment__: Boolean flag to specify whether the environment
 should be modified (see `devel_environment` and
 `runtime_environment`).  The default is True.
 
+- __export_build_environment__: Boolean flag to specify whether the
+build environment should be exported, or merely set on the
+configure command line.  The default is False.
+
 - __install__: Boolean flag to specify whether the `make install` step
 should be performed.  The default is True.
 
 - __ldconfig__: Boolean flag to specify whether the library directory
 should be added dynamic linker cache.  The default value is False.
 
 - __libdir__: The path relative to the install prefix to use when
```

### Comparing `hpccm-23.3.0/docs/getting_started.md` & `hpccm-23.5.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/misc_api.md` & `hpccm-23.5.0/docs/misc_api.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/primitives.md` & `hpccm-23.5.0/docs/primitives.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/recipes.md` & `hpccm-23.5.0/docs/recipes.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/tutorial.md` & `hpccm-23.5.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/docs/workflows.md` & `hpccm-23.5.0/docs/workflows.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/__init__.py` & `hpccm-23.5.0/hpccm/building_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/amgx.py` & `hpccm-23.5.0/hpccm/building_blocks/amgx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/apt_get.py` & `hpccm-23.5.0/hpccm/building_blocks/apt_get.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/arm_allinea_studio.py` & `hpccm-23.5.0/hpccm/building_blocks/arm_allinea_studio.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/base.py` & `hpccm-23.5.0/hpccm/building_blocks/base.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/boost.py` & `hpccm-23.5.0/hpccm/building_blocks/boost.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/catalyst.py` & `hpccm-23.5.0/hpccm/building_blocks/catalyst.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/cgns.py` & `hpccm-23.5.0/hpccm/building_blocks/cgns.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/charm.py` & `hpccm-23.5.0/hpccm/building_blocks/charm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/cmake.py` & `hpccm-23.5.0/hpccm/building_blocks/cmake.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/conda.py` & `hpccm-23.5.0/hpccm/building_blocks/conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """conda building block"""
 
 from __future__ import absolute_import
 from __future__ import unicode_literals
 from __future__ import print_function
 
-from distutils.version import StrictVersion
+from distutils.version import LooseVersion
 import logging
 import posixpath
 
 import hpccm.config
 import hpccm.templates.rm
 import hpccm.templates.wget
 
@@ -62,18 +62,18 @@
     `/usr/local/anaconda`.
 
     python2: Boolean flag to specify that the Python 2 version of
     Anaconda should be installed.  The default is False.
 
     python_subversion: The Python version to install.  This value is
     ignored if the Conda version is less than 4.8.  The default is
-    `py38` if using Python 3, and `py27` if using Python 2.
+    `py310` if using Python 3, and `py27` if using Python 2.
 
     version: The version of Anaconda to download.  The default value
-    is `4.8.3`.
+    is `23.1.0-1` if using Python 3, and `4.8.3` if using Python 2.
 
     # Examples
 
     ```python
     conda(packages=['numpy'])
     ```
 
@@ -105,16 +105,16 @@
         self.__ospackages = kwargs.get('ospackages',
                                        ['ca-certificates', 'wget'])
         self.__packages = kwargs.get('packages', [])
         self.__prefix = kwargs.get('prefix', '/usr/local/anaconda')
         self.__python2 = kwargs.get('python2', False)
         self.__python_version = '2' if self.__python2 else '3'
         self.__python_subversion = kwargs.get(
-            'python_subversion', 'py27' if self.__python2 else 'py38')
-        self.__version = kwargs.get('version', '4.8.3')
+            'python_subversion', 'py27' if self.__python2 else 'py310')
+        self.__version = kwargs.get('version', '4.8.3' if self.__python2 else '23.1.0-1')
 
         self.__commands = [] # Filled in by __setup()
         self.__wd = kwargs.get('wd', hpccm.config.g_wd) # working directory
 
         if not self.__eula:
             logging.warning('Anaconda EULA was not accepted.  To accept, see the documentation for this building block')
 
@@ -148,15 +148,15 @@
         else: # pragma: no cover
             raise RuntimeError('Unknown CPU architecture')
 
     def __setup(self):
         """Construct the series of shell commands, i.e., fill in
            self.__commands"""
 
-        if StrictVersion(self.__version) >= StrictVersion('4.8'):
+        if LooseVersion(self.__version) >= LooseVersion('4.8'):
             miniconda = 'Miniconda{0}-{1}_{2}-Linux-{3}.sh'.format(
                 self.__python_version, self.__python_subversion,
                 self.__version, self.__arch_pkg)
         else:
             miniconda = 'Miniconda{0}-{1}-Linux-{2}.sh'.format(
                 self.__python_version, self.__version, self.__arch_pkg)
         url = '{0}/{1}'.format(self.__baseurl, miniconda)
```

### Comparing `hpccm-23.3.0/hpccm/building_blocks/fftw.py` & `hpccm-23.5.0/hpccm/building_blocks/fftw.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/gdrcopy.py` & `hpccm-23.5.0/hpccm/building_blocks/gdrcopy.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/generic_autotools.py` & `hpccm-23.5.0/hpccm/building_blocks/generic_autotools.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
     `--enable-foo` and `enable_foo='yes'` maps to `--enable-foo=yes`.
     Underscores in the parameter name are converted to dashes.
 
     environment: Boolean flag to specify whether the environment
     should be modified (see `devel_environment` and
     `runtime_environment`).  The default is True.
 
+    export_build_environment: Boolean flag to specify whether the
+    build environment should be exported, or merely set on the
+    configure command line.  The default is False.
+
     install: Boolean flag to specify whether the `make install` step
     should be performed.  The default is True.
 
     ldconfig: Boolean flag to specify whether the library directory
     should be added dynamic linker cache.  The default value is False.
 
     libdir: The path relative to the install prefix to use when
@@ -187,14 +191,15 @@
         self.__build_directory = kwargs.get('build_directory', None)
         self.__build_environment = kwargs.get('build_environment', {})
         self.__check = kwargs.get('check', False)
         self.__comment = kwargs.get('comment', True)
         self.configure_opts = kwargs.get('configure_opts', [])
         self.__directory = kwargs.get('directory', None)
         self.environment_variables = kwargs.get('devel_environment', {})
+        self.__export_build_environment = kwargs.get('export_build_environment', False)
         self.__install = kwargs.get('install', True)
         self.__libdir = kwargs.get('libdir', 'lib')
         self.__make = kwargs.get('make', True)
         self.__postconfigure = kwargs.get('postconfigure', [])
         self.__postinstall = kwargs.get('postinstall', [])
         self.__preconfigure = kwargs.get('preconfigure', [])
         self.__recursive = kwargs.get('recursive', False)
@@ -262,14 +267,15 @@
         build_environment = []
         if self.__build_environment:
             for key, val in sorted(self.__build_environment.items()):
                 build_environment.append('{0}={1}'.format(key, val))
         self.__commands.append(self.configure_step(
             build_directory=self.__build_directory,
             directory=self.src_directory, environment=build_environment,
+            export_environment=self.__export_build_environment,
             toolchain=self.__toolchain))
 
         # Post configure setup
         if self.__postconfigure:
             # Assume the postconfigure commands should be run from the
             # source directory
             self.__commands.append('cd {}'.format(self.src_directory))
```

### Comparing `hpccm-23.3.0/hpccm/building_blocks/generic_build.py` & `hpccm-23.5.0/hpccm/building_blocks/generic_build.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/generic_cmake.py` & `hpccm-23.5.0/hpccm/building_blocks/generic_cmake.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/gnu.py` & `hpccm-23.5.0/hpccm/building_blocks/gnu.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/hdf5.py` & `hpccm-23.5.0/hpccm/building_blocks/hdf5.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/hpcx.py` & `hpccm-23.5.0/hpccm/building_blocks/hpcx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/intel_mpi.py` & `hpccm-23.5.0/hpccm/building_blocks/intel_mpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/intel_psxe.py` & `hpccm-23.5.0/hpccm/building_blocks/intel_psxe.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/intel_psxe_runtime.py` & `hpccm-23.5.0/hpccm/building_blocks/intel_psxe_runtime.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/julia.py` & `hpccm-23.5.0/hpccm/building_blocks/julia.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/knem.py` & `hpccm-23.5.0/hpccm/building_blocks/knem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/kokkos.py` & `hpccm-23.5.0/hpccm/building_blocks/kokkos.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/libsim.py` & `hpccm-23.5.0/hpccm/building_blocks/libsim.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/llvm.py` & `hpccm-23.5.0/hpccm/building_blocks/llvm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/magma.py` & `hpccm-23.5.0/hpccm/building_blocks/magma.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/mkl.py` & `hpccm-23.5.0/hpccm/building_blocks/mkl.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/mlnx_ofed.py` & `hpccm-23.5.0/hpccm/building_blocks/mlnx_ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/mpich.py` & `hpccm-23.5.0/hpccm/building_blocks/mpich.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/multi_ofed.py` & `hpccm-23.5.0/hpccm/building_blocks/multi_ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/mvapich2.py` & `hpccm-23.5.0/hpccm/building_blocks/mvapich2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/mvapich2_gdr.py` & `hpccm-23.5.0/hpccm/building_blocks/mvapich2_gdr.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/nccl.py` & `hpccm-23.5.0/hpccm/building_blocks/nccl.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/netcdf.py` & `hpccm-23.5.0/hpccm/building_blocks/netcdf.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/nsight_compute.py` & `hpccm-23.5.0/hpccm/building_blocks/nsight_compute.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/nsight_systems.py` & `hpccm-23.5.0/hpccm/building_blocks/nsight_systems.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/nvhpc.py` & `hpccm-23.5.0/hpccm/building_blocks/nvhpc.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/nvshmem.py` & `hpccm-23.5.0/hpccm/building_blocks/nvshmem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/ofed.py` & `hpccm-23.5.0/hpccm/building_blocks/ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/openblas.py` & `hpccm-23.5.0/hpccm/building_blocks/openblas.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/openmpi.py` & `hpccm-23.5.0/hpccm/building_blocks/openmpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/packages.py` & `hpccm-23.5.0/hpccm/building_blocks/packages.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/pgi.py` & `hpccm-23.5.0/hpccm/building_blocks/pgi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/pip.py` & `hpccm-23.5.0/hpccm/building_blocks/pip.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/pmix.py` & `hpccm-23.5.0/hpccm/building_blocks/pmix.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/pnetcdf.py` & `hpccm-23.5.0/hpccm/building_blocks/pnetcdf.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/rdma_core.py` & `hpccm-23.5.0/hpccm/building_blocks/rdma_core.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/scif.py` & `hpccm-23.5.0/hpccm/building_blocks/scif.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/sensei.py` & `hpccm-23.5.0/hpccm/building_blocks/sensei.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/slurm_pmi2.py` & `hpccm-23.5.0/hpccm/building_blocks/slurm_pmi2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/ucx.py` & `hpccm-23.5.0/hpccm/building_blocks/ucx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/xpmem.py` & `hpccm-23.5.0/hpccm/building_blocks/xpmem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/building_blocks/yum.py` & `hpccm-23.5.0/hpccm/building_blocks/yum.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/__init__.py` & `hpccm-23.5.0/hpccm/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/baseimage.py` & `hpccm-23.5.0/hpccm/primitives/baseimage.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/blob.py` & `hpccm-23.5.0/hpccm/primitives/blob.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/comment.py` & `hpccm-23.5.0/hpccm/primitives/comment.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/copy.py` & `hpccm-23.5.0/hpccm/primitives/copy.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/environment.py` & `hpccm-23.5.0/hpccm/primitives/environment.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/label.py` & `hpccm-23.5.0/hpccm/primitives/label.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/raw.py` & `hpccm-23.5.0/hpccm/primitives/raw.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/runscript.py` & `hpccm-23.5.0/hpccm/primitives/runscript.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/shell.py` & `hpccm-23.5.0/hpccm/primitives/shell.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/user.py` & `hpccm-23.5.0/hpccm/primitives/user.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/primitives/workdir.py` & `hpccm-23.5.0/hpccm/primitives/workdir.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/CMakeBuild.py` & `hpccm-23.5.0/hpccm/templates/CMakeBuild.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/ConfigureMake.py` & `hpccm-23.5.0/hpccm/templates/ConfigureMake.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,16 @@
     def check_step(self, parallel=None):
         """Generate make check command line string"""
         if not parallel:
             parallel = self.parallel
         return 'make -j{} check'.format(parallel)
 
     def configure_step(self, build_directory=None, directory=None,
-                       environment=[], opts=[], toolchain=None):
+                       environment=[], export_environment=False, opts=[],
+                       toolchain=None):
         """Generate configure command line string"""
 
         change_directory = ''
         src_directory = '.'
         if directory:
             if build_directory:
                 src_directory = directory
@@ -134,15 +135,18 @@
                 e.append('LDFLAGS={}'.format(shlex_quote(
                     toolchain.LDFLAGS)))
 
             if toolchain.LIBS:
                 e.append('LIBS={}'.format(shlex_quote(
                     toolchain.LIBS)))
 
-        configure_env = ' '.join(e)
+        if export_environment:
+            configure_env = 'export {} &&'.format(' '.join(e))
+        else:
+            configure_env = ' '.join(e)
 
         # Build set of configuration command line options
         optlist = []
         if not opts:
             if self.configure_opts:
                 optlist.extend(self.configure_opts)
             if self.__opts:
```

### Comparing `hpccm-23.3.0/hpccm/templates/__init__.py` & `hpccm-23.5.0/hpccm/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/annotate.py` & `hpccm-23.5.0/hpccm/templates/annotate.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/downloader.py` & `hpccm-23.5.0/hpccm/templates/downloader.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/envvars.py` & `hpccm-23.5.0/hpccm/templates/envvars.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/git.py` & `hpccm-23.5.0/hpccm/templates/git.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/ldconfig.py` & `hpccm-23.5.0/hpccm/templates/ldconfig.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/rm.py` & `hpccm-23.5.0/hpccm/templates/rm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/sed.py` & `hpccm-23.5.0/hpccm/templates/sed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/tar.py` & `hpccm-23.5.0/hpccm/templates/tar.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/wget.py` & `hpccm-23.5.0/hpccm/templates/wget.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/templates/zipfile.py` & `hpccm-23.5.0/hpccm/templates/zipfile.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/Stage.py` & `hpccm-23.5.0/hpccm/Stage.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/__init__.py` & `hpccm-23.5.0/hpccm/__init__.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/base_object.py` & `hpccm-23.5.0/hpccm/base_object.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/cli.py` & `hpccm-23.5.0/hpccm/cli.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/common.py` & `hpccm-23.5.0/hpccm/common.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/config.py` & `hpccm-23.5.0/hpccm/config.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/recipe.py` & `hpccm-23.5.0/hpccm/recipe.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/toolchain.py` & `hpccm-23.5.0/hpccm/toolchain.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/hpccm/version.py` & `hpccm-23.5.0/hpccm/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import absolute_import
 
-__version__ = '23.3.0'
+__version__ = '23.5.0'
```

### Comparing `hpccm-23.3.0/hpccm.egg-info/PKG-INFO` & `hpccm-23.5.0/hpccm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpccm
-Version: 23.3.0
+Version: 23.5.0
 Summary: HPC Container Maker
 Home-page: https://github.com/NVIDIA/hpc-container-maker
 Maintainer: Scott McMillan
 Maintainer-email: smcmillan@nvidia.com
 License: Apache License Version 2.0
 Description: [![Python 3](https://github.com/NVIDIA/hpc-container-maker/workflows/Python%203/badge.svg)](https://github.com/NVIDIA/hpc-container-maker/actions?query=workflow%3A%22Python+3%22)
         [![Python 2](https://github.com/NVIDIA/hpc-container-maker/workflows/Python%202/badge.svg)](https://github.com/NVIDIA/hpc-container-maker/actions?query=workflow%3A%22Python+2%22)
```

### Comparing `hpccm-23.3.0/hpccm.egg-info/SOURCES.txt` & `hpccm-23.5.0/hpccm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/examples/multistage.py` & `hpccm-23.5.0/recipes/examples/multistage.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/examples/scif.py` & `hpccm-23.5.0/recipes/examples/scif.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/examples/script.py` & `hpccm-23.5.0/recipes/examples/script.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/examples/userargs.py` & `hpccm-23.5.0/recipes/examples/userargs.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/gromacs/gromacs.py` & `hpccm-23.5.0/recipes/gromacs/gromacs.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpccm/README.md` & `hpccm-23.5.0/recipes/hpccm/README.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpccm/bootstrap.py` & `hpccm-23.5.0/recipes/hpccm/bootstrap.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/jupyter/README.md` & `hpccm-23.5.0/recipes/jupyter/README.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/jupyter/jupyter.py` & `hpccm-23.5.0/recipes/jupyter/jupyter.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/jupyter/notebook.ipynb` & `hpccm-23.5.0/recipes/jupyter/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/lammps/lammps.py` & `hpccm-23.5.0/recipes/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/milc/milc.py` & `hpccm-23.5.0/recipes/milc/milc.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/osu_benchmarks/README.md` & `hpccm-23.5.0/recipes/osu_benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/osu_benchmarks/common.py` & `hpccm-23.5.0/recipes/osu_benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/osu_benchmarks/entrypoint.sh` & `hpccm-23.5.0/recipes/osu_benchmarks/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/osu_benchmarks/osu_benchmarks.py` & `hpccm-23.5.0/recipes/osu_benchmarks/osu_benchmarks.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/easybuild.py` & `hpccm-23.5.0/recipes/easybuild.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpcbase-gnu-mvapich2.py` & `hpccm-23.5.0/recipes/hpcbase-gnu-mvapich2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpcbase-gnu-openmpi.py` & `hpccm-23.5.0/recipes/hpcbase-gnu-openmpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpcbase-nvhpc-mvapich2.py` & `hpccm-23.5.0/recipes/hpcbase-nvhpc-mvapich2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/hpcbase-nvhpc-openmpi.py` & `hpccm-23.5.0/recipes/hpcbase-nvhpc-openmpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/mpi_bandwidth.py` & `hpccm-23.5.0/recipes/mpi_bandwidth.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/nvhpc.py` & `hpccm-23.5.0/recipes/nvhpc.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/recipes/spack.py` & `hpccm-23.5.0/recipes/spack.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/helpers.py` & `hpccm-23.5.0/test/helpers.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_CMakeBuild.py` & `hpccm-23.5.0/test/test_CMakeBuild.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_ConfigureMake.py` & `hpccm-23.5.0/test/test_ConfigureMake.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,7 +117,21 @@
     def test_kwargs(self):
         """kwargs"""
         cm = ConfigureMake(disable_long_option=True, enable_foo=True,
                            with_foo=True, with_foo2='/usr',
                            without_bar=True, prefix=None)
         configure = cm.configure_step()
         self.assertEqual(configure, './configure --disable-long-option --enable-foo --with-foo --with-foo2=/usr --without-bar')
+
+    def test_export_environment(self):
+        """export_environment"""
+        cm = ConfigureMake()
+
+        tc = toolchain(CC='mpicc', CXX='mpicxx', FC='mpifc')
+        env = ['OMPI_CC=mycc', 'OMPI_CXX=mycxx', 'OMPI_FC=myfc']
+
+        configure = cm.configure_step(environment=env, toolchain=tc)
+        self.assertEqual(configure, 'OMPI_CC=mycc OMPI_CXX=mycxx OMPI_FC=myfc CC=mpicc CXX=mpicxx FC=mpifc ./configure --prefix=/usr/local')
+
+        ex_configure = cm.configure_step(environment=env,
+                                         export_environment=True, toolchain=tc)
+        self.assertEqual(ex_configure, 'export OMPI_CC=mycc OMPI_CXX=mycxx OMPI_FC=myfc CC=mpicc CXX=mpicxx FC=mpifc && ./configure --prefix=/usr/local')
```

### Comparing `hpccm-23.3.0/test/test_Stage.py` & `hpccm-23.5.0/test/test_Stage.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_amgx.py` & `hpccm-23.5.0/test/test_amgx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_annotate.py` & `hpccm-23.5.0/test/test_annotate.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_apt_get.py` & `hpccm-23.5.0/test/test_apt_get.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_arm_allinea_studio.py` & `hpccm-23.5.0/test/test_arm_allinea_studio.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_baseimage.py` & `hpccm-23.5.0/test/test_baseimage.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_bb_base.py` & `hpccm-23.5.0/test/test_bb_base.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_blob.py` & `hpccm-23.5.0/test/test_blob.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_boost.py` & `hpccm-23.5.0/test/test_boost.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_catalyst.py` & `hpccm-23.5.0/test/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_cgns.py` & `hpccm-23.5.0/test/test_cgns.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_charm.py` & `hpccm-23.5.0/test/test_charm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_cli.py` & `hpccm-23.5.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_cmake.py` & `hpccm-23.5.0/test/test_cmake.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_comment.py` & `hpccm-23.5.0/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_conda.py` & `hpccm-23.5.0/test/test_conda.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,45 +40,45 @@
         self.assertEqual(str(c),
 r'''# Anaconda
 RUN apt-get update -y && \
     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
         ca-certificates \
         wget && \
     rm -rf /var/lib/apt/lists/*
-RUN mkdir -p /var/tmp && wget -q -nc --no-check-certificate -P /var/tmp http://repo.anaconda.com/miniconda/Miniconda3-py38_4.8.3-Linux-x86_64.sh && \
-    bash /var/tmp/Miniconda3-py38_4.8.3-Linux-x86_64.sh -b -p /usr/local/anaconda && \
+RUN mkdir -p /var/tmp && wget -q -nc --no-check-certificate -P /var/tmp http://repo.anaconda.com/miniconda/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh && \
+    bash /var/tmp/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh -b -p /usr/local/anaconda && \
     /usr/local/anaconda/bin/conda init && \
     ln -s /usr/local/anaconda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     . /usr/local/anaconda/etc/profile.d/conda.sh && \
     conda activate base && \
     conda install -y numpy && \
     /usr/local/anaconda/bin/conda clean -afy && \
-    rm -rf /var/tmp/Miniconda3-py38_4.8.3-Linux-x86_64.sh''')
+    rm -rf /var/tmp/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh''')
 
     @x86_64
     @centos
     @docker
     def test_defaults_centos(self):
         """Default conda building block"""
         c = conda(eula=True, packages=['numpy'])
         self.assertEqual(str(c),
 r'''# Anaconda
 RUN yum install -y \
         ca-certificates \
         wget && \
     rm -rf /var/cache/yum/*
-RUN mkdir -p /var/tmp && wget -q -nc --no-check-certificate -P /var/tmp http://repo.anaconda.com/miniconda/Miniconda3-py38_4.8.3-Linux-x86_64.sh && \
-    bash /var/tmp/Miniconda3-py38_4.8.3-Linux-x86_64.sh -b -p /usr/local/anaconda && \
+RUN mkdir -p /var/tmp && wget -q -nc --no-check-certificate -P /var/tmp http://repo.anaconda.com/miniconda/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh && \
+    bash /var/tmp/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh -b -p /usr/local/anaconda && \
     /usr/local/anaconda/bin/conda init && \
     ln -s /usr/local/anaconda/etc/profile.d/conda.sh /etc/profile.d/conda.sh && \
     . /usr/local/anaconda/etc/profile.d/conda.sh && \
     conda activate base && \
     conda install -y numpy && \
     /usr/local/anaconda/bin/conda clean -afy && \
-    rm -rf /var/tmp/Miniconda3-py38_4.8.3-Linux-x86_64.sh''')
+    rm -rf /var/tmp/Miniconda3-py310_23.1.0-1-Linux-x86_64.sh''')
 
     @ppc64le
     @ubuntu
     @docker
     def test_ppc64le(self):
         """ppc64le"""
         c = conda(eula=True, version='4.7.12')
```

### Comparing `hpccm-23.3.0/test/test_config.py` & `hpccm-23.5.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_copy.py` & `hpccm-23.5.0/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_downloader.py` & `hpccm-23.5.0/test/test_downloader.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_environment.py` & `hpccm-23.5.0/test/test_environment.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_envvars.py` & `hpccm-23.5.0/test/test_envvars.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_fftw.py` & `hpccm-23.5.0/test/test_fftw.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_gdrcopy.py` & `hpccm-23.5.0/test/test_gdrcopy.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_generic_autotools.py` & `hpccm-23.5.0/test/test_generic_autotools.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_generic_build.py` & `hpccm-23.5.0/test/test_generic_build.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_generic_cmake.py` & `hpccm-23.5.0/test/test_generic_cmake.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_git.py` & `hpccm-23.5.0/test/test_git.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_global_vars.py` & `hpccm-23.5.0/test/test_global_vars.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_gnu.py` & `hpccm-23.5.0/test/test_gnu.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_hdf5.py` & `hpccm-23.5.0/test/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_hpcx.py` & `hpccm-23.5.0/test/test_hpcx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_intel_mpi.py` & `hpccm-23.5.0/test/test_intel_mpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_intel_psxe.py` & `hpccm-23.5.0/test/test_intel_psxe.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_intel_psxe_runtime.py` & `hpccm-23.5.0/test/test_intel_psxe_runtime.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_julia.py` & `hpccm-23.5.0/test/test_julia.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_knem.py` & `hpccm-23.5.0/test/test_knem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_kokkos.py` & `hpccm-23.5.0/test/test_kokkos.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_label.py` & `hpccm-23.5.0/test/test_label.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_ldconfig.py` & `hpccm-23.5.0/test/test_ldconfig.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_libsim.py` & `hpccm-23.5.0/test/test_libsim.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_llvm.py` & `hpccm-23.5.0/test/test_llvm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_magma.py` & `hpccm-23.5.0/test/test_magma.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_mkl.py` & `hpccm-23.5.0/test/test_mkl.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_mlnx_ofed.py` & `hpccm-23.5.0/test/test_mlnx_ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_mpich.py` & `hpccm-23.5.0/test/test_mpich.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_multi_ofed.py` & `hpccm-23.5.0/test/test_multi_ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_mvapich2.py` & `hpccm-23.5.0/test/test_mvapich2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_mvapich2_gdr.py` & `hpccm-23.5.0/test/test_mvapich2_gdr.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_nccl.py` & `hpccm-23.5.0/test/test_nccl.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_netcdf.py` & `hpccm-23.5.0/test/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_nsight_compute.py` & `hpccm-23.5.0/test/test_nsight_compute.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_nsight_systems.py` & `hpccm-23.5.0/test/test_nsight_systems.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_nvhpc.py` & `hpccm-23.5.0/test/test_nvhpc.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_nvshmem.py` & `hpccm-23.5.0/test/test_nvshmem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_ofed.py` & `hpccm-23.5.0/test/test_ofed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_openblas.py` & `hpccm-23.5.0/test/test_openblas.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_openmpi.py` & `hpccm-23.5.0/test/test_openmpi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_packages.py` & `hpccm-23.5.0/test/test_packages.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_pgi.py` & `hpccm-23.5.0/test/test_pgi.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_pip.py` & `hpccm-23.5.0/test/test_pip.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_pmix.py` & `hpccm-23.5.0/test/test_pmix.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_pnetcdf.py` & `hpccm-23.5.0/test/test_pnetcdf.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_python.py` & `hpccm-23.5.0/test/test_python.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
 import logging # pylint: disable=unused-import
 import unittest
 
-from helpers import centos, centos8, docker, ubuntu
+from helpers import centos, centos8, docker, ubuntu, ubuntu22
 
 from hpccm.building_blocks.python import python
 
 class Test_python(unittest.TestCase):
     def setUp(self):
         """Disable logging output messages"""
         logging.disable(logging.ERROR)
@@ -40,14 +40,27 @@
 r'''# Python
 RUN apt-get update -y && \
     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
         python \
         python3 && \
     rm -rf /var/lib/apt/lists/*''')
 
+    @ubuntu22
+    @docker
+    def test_defaults_ubuntu22(self):
+        """Default python building block"""
+        p = python()
+        self.assertEqual(str(p),
+r'''# Python
+RUN apt-get update -y && \
+    DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
+        python2 \
+        python3 && \
+    rm -rf /var/lib/apt/lists/*''')
+
     @centos
     @docker
     def test_defaults_centos(self):
         """Default python building block"""
         p = python()
         self.assertEqual(str(p),
 r'''# Python
```

### Comparing `hpccm-23.3.0/test/test_raw.py` & `hpccm-23.5.0/test/test_raw.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_rdma_core.py` & `hpccm-23.5.0/test/test_rdma_core.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_recipe.py` & `hpccm-23.5.0/test/test_recipe.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_rm.py` & `hpccm-23.5.0/test/test_rm.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_runscript.py` & `hpccm-23.5.0/test/test_runscript.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_scif.py` & `hpccm-23.5.0/test/test_scif.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_sed.py` & `hpccm-23.5.0/test/test_sed.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_sensei.py` & `hpccm-23.5.0/test/test_sensei.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_shell.py` & `hpccm-23.5.0/test/test_shell.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_slurm_pmi2.py` & `hpccm-23.5.0/test/test_slurm_pmi2.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_tar.py` & `hpccm-23.5.0/test/test_tar.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_toolchain.py` & `hpccm-23.5.0/test/test_toolchain.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_ucx.py` & `hpccm-23.5.0/test/test_ucx.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_user.py` & `hpccm-23.5.0/test/test_user.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_wget.py` & `hpccm-23.5.0/test/test_wget.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_workdir.py` & `hpccm-23.5.0/test/test_workdir.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_xpmem.py` & `hpccm-23.5.0/test/test_xpmem.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_yum.py` & `hpccm-23.5.0/test/test_yum.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/test/test_zipfile.py` & `hpccm-23.5.0/test/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/CHANGELOG.md` & `hpccm-23.5.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# v23.5.0
+- Add the ability to export the build environment to the generic
+  Autotools building block (`generic_autotools`).
+- Update the Anaconda (`conda`) package for the new upstream versioning
+  scheme, and refreshes the default component version.
+- Fix the Python building block (`python`) to use the correct name of the
+  Python 2 package on Ubuntu 22.04
+
 # v23.3.0
 - Refreshes default component version for the LLVM ('llvm') building block.
 
 # v23.2.0
 - Refreshes default component versions for the CMake (`cmake`), OpenBLAS
   (`openblas`), Nsight Compute (`nsight_compute`), Nsight Systems
   (`nsight_systems`), and NVIDIA HPC SDK (`nvhpc`) building blocks.
```

### Comparing `hpccm-23.3.0/LICENSE` & `hpccm-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/README.md` & `hpccm-23.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/setup.py` & `hpccm-23.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `hpccm-23.3.0/PKG-INFO` & `hpccm-23.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpccm
-Version: 23.3.0
+Version: 23.5.0
 Summary: HPC Container Maker
 Home-page: https://github.com/NVIDIA/hpc-container-maker
 Maintainer: Scott McMillan
 Maintainer-email: smcmillan@nvidia.com
 License: Apache License Version 2.0
 Description: [![Python 3](https://github.com/NVIDIA/hpc-container-maker/workflows/Python%203/badge.svg)](https://github.com/NVIDIA/hpc-container-maker/actions?query=workflow%3A%22Python+3%22)
         [![Python 2](https://github.com/NVIDIA/hpc-container-maker/workflows/Python%202/badge.svg)](https://github.com/NVIDIA/hpc-container-maker/actions?query=workflow%3A%22Python+2%22)
```

