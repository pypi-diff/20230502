# Comparing `tmp/pyoptimus-3.0.0b2.tar.gz` & `tmp/pyoptimus-3.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\dev\mood\Optimus\dist\tmp83wjfouf\pyoptimus-3.0.0b2.tar", last modified: Thu Jun 17 04:20:37 2021, max compression
+gzip compressed data, was "dist\pyoptimus-3.0.0b3.tar", last modified: Thu Jun 17 15:28:40 2021, max compression
```

## Comparing `pyoptimus-3.0.0b2.tar` & `pyoptimus-3.0.0b3.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.196537 pyoptimus-3.0.0b2/
--rw-rw-rw-   0        0        0    11357 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/LICENSE
--rw-rw-rw-   0        0        0      118 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/MANIFEST.in
--rw-rw-rw-   0        0        0    22877 2021-06-17 04:20:37.196537 pyoptimus-3.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0    21199 2021-06-17 03:42:50.000000 pyoptimus-3.0.0b2/README.md
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.898468 pyoptimus-3.0.0b2/optimus/
--rw-rw-rw-   0        0        0      354 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.899469 pyoptimus-3.0.0b2/optimus/css/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/css/__init__.py
--rw-rw-rw-   0        0        0      997 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/css/styles.css
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.902469 pyoptimus-3.0.0b2/optimus/engines/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.918473 pyoptimus-3.0.0b2/optimus/engines/base/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/__init__.py
--rw-rw-rw-   0        0        0    30906 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/basedataframe.py
--rw-rw-rw-   0        0        0    94652 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/columns.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.920474 pyoptimus-3.0.0b2/optimus/engines/base/commons/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/commons/__init__.py
--rw-rw-rw-   0        0        0     7459 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/commons/functions.py
--rw-rw-rw-   0        0        0       71 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/contants.py
--rw-rw-rw-   0        0        0      658 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/create.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.922475 pyoptimus-3.0.0b2/optimus/engines/base/cudf/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/cudf/__init__.py
--rw-rw-rw-   0        0        0      148 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/cudf/columns.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.929474 pyoptimus-3.0.0b2/optimus/engines/base/dask/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/__init__.py
--rw-rw-rw-   0        0        0     6899 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/columns.py
--rw-rw-rw-   0        0        0     2144 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/constants.py
--rw-rw-rw-   0        0        0     7830 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/dataframe.py
--rw-rw-rw-   0        0        0     1811 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.930475 pyoptimus-3.0.0b2/optimus/engines/base/dask/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/io/__init__.py
--rw-rw-rw-   0        0        0    16855 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/io/jdbc.py
--rw-rw-rw-   0        0        0     6997 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dask/rows.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.935478 pyoptimus-3.0.0b2/optimus/engines/base/dataframe/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dataframe/__init__.py
--rw-rw-rw-   0        0        0     4863 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dataframe/columns.py
--rw-rw-rw-   0        0        0     6837 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/dataframe/dataframe.py
--rw-rw-rw-   0        0        0      896 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/engine.py
--rw-rw-rw-   0        0        0    14674 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.942479 pyoptimus-3.0.0b2/optimus/engines/base/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/__init__.py
--rw-rw-rw-   0        0        0     9132 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/connect.py
--rw-rw-rw-   0        0        0     1325 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/driver_context.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.955482 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/__init__.py
--rw-rw-rw-   0        0        0     2131 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/abstract_driver.py
--rw-rw-rw-   0        0        0     1269 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/bigquery.py
--rw-rw-rw-   0        0        0      912 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/cassandra.py
--rw-rw-rw-   0        0        0     1659 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/impala.py
--rw-rw-rw-   0        0        0     1656 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/mysql.py
--rw-rw-rw-   0        0        0     1641 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/oracle.py
--rw-rw-rw-   0        0        0     1906 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/postgresql.py
--rw-rw-rw-   0        0        0     1359 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/presto.py
--rw-rw-rw-   0        0        0     1618 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/redshift.py
--rw-rw-rw-   0        0        0     1112 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/sqlite.py
--rw-rw-rw-   0        0        0     1151 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/sqlserver.py
--rw-rw-rw-   0        0        0     2544 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/factory.py
--rw-rw-rw-   0        0        0     5394 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/load.py
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/io/save.py
--rw-rw-rw-   0        0        0     7451 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/mask.py
--rw-rw-rw-   0        0        0     3683 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/meta.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.956482 pyoptimus-3.0.0b2/optimus/engines/base/ml/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/ml/__init__.py
--rw-rw-rw-   0        0        0      360 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/ml/contants.py
--rw-rw-rw-   0        0        0     2808 2021-06-16 19:39:11.000000 pyoptimus-3.0.0b2/optimus/engines/base/profile.py
--rw-rw-rw-   0        0        0     9245 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/remote.py
--rw-rw-rw-   0        0        0    10138 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/rows.py
--rw-rw-rw-   0        0        0     5718 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/base/stringclustering.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.967484 pyoptimus-3.0.0b2/optimus/engines/cudf/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/__init__.py
--rw-rw-rw-   0        0        0     9094 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/columns.py
--rw-rw-rw-   0        0        0     2363 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/constants.py
--rw-rw-rw-   0        0        0      739 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/create.py
--rw-rw-rw-   0        0        0       62 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/cudf.py
--rw-rw-rw-   0        0        0     1941 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/dataframe.py
--rw-rw-rw-   0        0        0     1178 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/engine.py
--rw-rw-rw-   0        0        0     3752 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.971484 pyoptimus-3.0.0b2/optimus/engines/cudf/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/io/__init__.py
--rw-rw-rw-   0        0        0      972 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/io/jdbc.py
--rw-rw-rw-   0        0        0     8025 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/io/load.py
--rw-rw-rw-   0        0        0     3769 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/io/save.py
--rw-rw-rw-   0        0        0      572 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/mask.py
--rw-rw-rw-   0        0        0     3855 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/cudf/rows.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.979487 pyoptimus-3.0.0b2/optimus/engines/dask/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/__init__.py
--rw-rw-rw-   0        0        0     1880 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/columns.py
--rw-rw-rw-   0        0        0     1064 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/create.py
--rw-rw-rw-   0        0        0      887 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/dask.py
--rw-rw-rw-   0        0        0     1830 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/dataframe.py
--rw-rw-rw-   0        0        0     5122 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/engine.py
--rw-rw-rw-   0        0        0     3921 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.984490 pyoptimus-3.0.0b2/optimus/engines/dask/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/io/__init__.py
--rw-rw-rw-   0        0        0      925 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/io/jdbc.py
--rw-rw-rw-   0        0        0    11407 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/io/load.py
--rw-rw-rw-   0        0        0     3976 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/io/save.py
--rw-rw-rw-   0        0        0      613 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/mask.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.987490 pyoptimus-3.0.0b2/optimus/engines/dask/ml/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/ml/__init__.py
--rw-rw-rw-   0        0        0     3691 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/ml/encoding.py
--rw-rw-rw-   0        0        0     4199 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/ml/models.py
--rw-rw-rw-   0        0        0      160 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask/rows.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:36.996493 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/__init__.py
--rw-rw-rw-   0        0        0     4896 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/columns.py
--rw-rw-rw-   0        0        0      702 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/create.py
--rw-rw-rw-   0        0        0     1011 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/dask_cudf.py
--rw-rw-rw-   0        0        0     2344 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/dataframe.py
--rw-rw-rw-   0        0        0     5673 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/engine.py
--rw-rw-rw-   0        0        0     3570 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.001493 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/__init__.py
--rw-rw-rw-   0        0        0     1234 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/jdbc.py
--rw-rw-rw-   0        0        0     8338 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/load.py
--rw-rw-rw-   0        0        0     3113 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/save.py
--rw-rw-rw-   0        0        0      576 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/mask.py
--rw-rw-rw-   0        0        0      659 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/dask_cudf/rows.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.007493 pyoptimus-3.0.0b2/optimus/engines/ibis/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/__init__.py
--rw-rw-rw-   0        0        0     6224 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/columns.py
--rw-rw-rw-   0        0        0     1634 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/dataframe.py
--rw-rw-rw-   0        0        0     1073 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/engine.py
--rw-rw-rw-   0        0        0     4184 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.010493 pyoptimus-3.0.0b2/optimus/engines/ibis/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/io/__init__.py
--rw-rw-rw-   0        0        0     3840 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/io/jdbc.py
--rw-rw-rw-   0        0        0     3603 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/io/save.py
--rw-rw-rw-   0        0        0     5202 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/ibis/rows.py
--rw-rw-rw-   0        0        0     3927 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/jit.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.020495 pyoptimus-3.0.0b2/optimus/engines/pandas/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/__init__.py
--rw-rw-rw-   0        0        0     3065 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/columns.py
--rw-rw-rw-   0        0        0     2090 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/constants.py
--rw-rw-rw-   0        0        0      651 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/create.py
--rw-rw-rw-   0        0        0     2129 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/dataframe.py
--rw-rw-rw-   0        0        0     1339 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/engine.py
--rw-rw-rw-   0        0        0     3500 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.026497 pyoptimus-3.0.0b2/optimus/engines/pandas/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/__init__.py
--rw-rw-rw-   0        0        0     1400 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/extract.py
--rw-rw-rw-   0        0        0      759 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/jdbc.py
--rw-rw-rw-   0        0        0     4259 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/json.py
--rw-rw-rw-   0        0        0    10296 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/load.py
--rw-rw-rw-   0        0        0     3702 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/io/save.py
--rw-rw-rw-   0        0        0      534 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/mask.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.030499 pyoptimus-3.0.0b2/optimus/engines/pandas/ml/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/ml/__init__.py
--rw-rw-rw-   0        0        0     3178 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/ml/encoding.py
--rw-rw-rw-   0        0        0     3637 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/ml/keycollision.py
--rw-rw-rw-   0        0        0    19341 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/ml/models.py
--rw-rw-rw-   0        0        0       66 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/pandas.py
--rw-rw-rw-   0        0        0     3744 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/pandas/rows.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.043502 pyoptimus-3.0.0b2/optimus/engines/spark/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/__init__.py
--rw-rw-rw-   0        0        0     4787 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/audf.py
--rw-rw-rw-   0        0        0    70116 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/columns.py
--rw-rw-rw-   0        0        0     3477 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/constants.py
--rw-rw-rw-   0        0        0     2226 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/create.py
--rw-rw-rw-   0        0        0    12142 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/dataframe.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.046503 pyoptimus-3.0.0b2/optimus/engines/spark/dl/
--rw-rw-rw-   0        0        0      125 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/dl/__init__.py
--rw-rw-rw-   0        0        0     1729 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/dl/models.py
--rw-rw-rw-   0        0        0    15582 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/engine.py
--rw-rw-rw-   0        0        0    12877 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.051504 pyoptimus-3.0.0b2/optimus/engines/spark/io/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/io/__init__.py
--rw-rw-rw-   0        0        0     8570 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/io/jdbc.py
--rw-rw-rw-   0        0        0     7775 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/io/load.py
--rw-rw-rw-   0        0        0     1818 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/io/properties.py
--rw-rw-rw-   0        0        0     6505 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/io/save.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.058506 pyoptimus-3.0.0b2/optimus/engines/spark/ml/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/__init__.py
--rw-rw-rw-   0        0        0     3542 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/distancecluster.py
--rw-rw-rw-   0        0        0     6559 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/encoding.py
--rw-rw-rw-   0        0        0     5158 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/keycollision.py
--rw-rw-rw-   0        0        0     4360 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/models.py
--rw-rw-rw-   0        0        0     7695 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/ml/pipelines.py
--rw-rw-rw-   0        0        0     9903 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/rows.py
--rw-rw-rw-   0        0        0     2442 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/engines/spark/spark.py
--rw-rw-rw-   0        0        0    21312 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/expressions.py
--rw-rw-rw-   0        0        0     1082 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.083512 pyoptimus-3.0.0b2/optimus/helpers/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/__init__.py
--rw-rw-rw-   0        0        0     3999 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/check.py
--rw-rw-rw-   0        0        0    13712 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/columns.py
--rw-rw-rw-   0        0        0     7646 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/columns_expression.py
--rw-rw-rw-   0        0        0    16166 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/constants.py
--rw-rw-rw-   0        0        0     3239 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/converter.py
--rw-rw-rw-   0        0        0      530 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/core.py
--rw-rw-rw-   0        0        0      590 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/debug.py
--rw-rw-rw-   0        0        0      406 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/decorators.py
--rw-rw-rw-   0        0        0      135 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/exceptions.py
--rw-rw-rw-   0        0        0      274 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/filters.py
--rw-rw-rw-   0        0        0    18408 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/functions.py
--rw-rw-rw-   0        0        0     2152 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/functions_spark.py
--rw-rw-rw-   0        0        0     1836 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/io.py
--rw-rw-rw-   0        0        0     1260 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/json.py
--rw-rw-rw-   0        0        0     1154 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/logger.py
--rw-rw-rw-   0        0        0     1415 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/output.py
--rw-rw-rw-   0        0        0     2738 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/parser.py
--rw-rw-rw-   0        0        0      245 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/pickle.py
--rw-rw-rw-   0        0        0     3371 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/raiseit.py
--rw-rw-rw-   0        0        0    10344 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/helpers/test.py
--rw-rw-rw-   0        0        0    14613 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/infer.py
--rw-rw-rw-   0        0        0     4608 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/infer_spark.py
--rw-rw-rw-   0        0        0     2701 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/optimus.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.094514 pyoptimus-3.0.0b2/optimus/outliers/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/__init__.py
--rw-rw-rw-   0        0        0     4066 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/abstract_outliers_bounds.py
--rw-rw-rw-   0        0        0     2266 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/abstract_outliers_threshold.py
--rw-rw-rw-   0        0        0     2174 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/mad.py
--rw-rw-rw-   0        0        0     1730 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/modified_z_score.py
--rw-rw-rw-   0        0        0      818 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/outliers.py
--rw-rw-rw-   0        0        0     2025 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/tukey.py
--rw-rw-rw-   0        0        0     1223 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/outliers/z_score.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.098513 pyoptimus-3.0.0b2/optimus/plots/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/plots/__init__.py
--rw-rw-rw-   0        0        0     7589 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/plots/functions.py
--rw-rw-rw-   0        0        0     3845 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/plots/plots.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.102517 pyoptimus-3.0.0b2/optimus/profiler/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/__init__.py
--rw-rw-rw-   0        0        0       17 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/constants.py
--rw-rw-rw-   0        0        0     2333 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/functions.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.104515 pyoptimus-3.0.0b2/optimus/profiler/templates/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/templates/__init__.py
--rw-rw-rw-   0        0        0      491 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/templates/html.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.108516 pyoptimus-3.0.0b2/optimus/profiler/templates/out/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/templates/out/__init__.py
--rw-rw-rw-   0        0        0     2256 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/templates/out/general_info.html
--rw-rw-rw-   0        0        0    11481 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/profiler/templates/out/one_column.html
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.109516 pyoptimus-3.0.0b2/optimus/templates/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.112516 pyoptimus-3.0.0b2/optimus/templates/out/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/templates/out/__init__.py
--rw-rw-rw-   0        0        0     1883 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/templates/out/table.html
--rw-rw-rw-   0        0        0      196 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b2/optimus/version.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.145524 pyoptimus-3.0.0b2/pyoptimus.egg-info/
--rw-rw-rw-   0        0        0    22877 2021-06-17 04:20:36.000000 pyoptimus-3.0.0b2/pyoptimus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7630 2021-06-17 04:20:36.000000 pyoptimus-3.0.0b2/pyoptimus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-17 04:20:36.000000 pyoptimus-3.0.0b2/pyoptimus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1400 2021-06-17 04:20:36.000000 pyoptimus-3.0.0b2/pyoptimus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-06-17 04:20:36.000000 pyoptimus-3.0.0b2/pyoptimus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2021-06-17 04:20:37.203540 pyoptimus-3.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0     2842 2021-06-17 03:49:31.000000 pyoptimus-3.0.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.184535 pyoptimus-3.0.0b2/tests/
--rw-rw-rw-   0        0        0        2 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-17 04:20:37.195538 pyoptimus-3.0.0b2/tests/creator/
--rw-rw-rw-   0        0        0        0 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/creator/__init__.py
--rw-rw-rw-   0        0        0    30062 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/creator/creator-cudf.py
--rw-rw-rw-   0        0        0     5015 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/creator/creator-dask-debug.py
--rw-rw-rw-   0        0        0    29943 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/creator/creator-dask.py
--rw-rw-rw-   0        0        0     4128 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/creator/creator-ext.py
--rw-rw-rw-   0        0        0     4787 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/creator/creator-profiler.py
--rw-rw-rw-   0        0        0    36136 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/creator/creator.py
--rw-rw-rw-   0        0        0    29715 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/creator/cudf.py
--rw-rw-rw-   0        0        0     1482 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_dataframe.py
--rw-rw-rw-   0        0        0   249989 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_cols.py
--rw-rw-rw-   0        0        0     9569 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_cols_2.py
--rw-rw-rw-   0        0        0   239031 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_cols_dask.py
--rw-rw-rw-   0        0        0   402343 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_cols_pandas.py
--rw-rw-rw-   0        0        0  1327275 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_distance_cluster.py
--rw-rw-rw-   0        0        0     6638 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_ext.py
--rw-rw-rw-   0        0        0    48170 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_keycollision.py
--rw-rw-rw-   0        0        0     1649 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_ml_2.py
--rw-rw-rw-   0        0        0    17841 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_outliers.py
--rw-rw-rw-   0        0        0     6551 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_profiler.py
--rw-rw-rw-   0        0        0     4789 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_df_rows.py
--rw-rw-rw-   0        0        0     1511 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_dl.py
--rw-rw-rw-   0        0        0      904 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/test_example_notebooks.py
--rw-rw-rw-   0        0        0    10090 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_meta.py
--rw-rw-rw-   0        0        0     4832 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_ml.py
--rw-rw-rw-   0        0        0    15604 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b2/tests/test_op_io.py
--rw-rw-rw-   0        0        0     2398 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_optimus.py
--rw-rw-rw-   0        0        0      408 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_optimus_spark_session.py
--rw-rw-rw-   0        0        0     9235 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_plot.py
--rw-rw-rw-   0        0        0     3227 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_profiler.py
--rw-rw-rw-   0        0        0     8199 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b2/tests/test_sql.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.177933 pyoptimus-3.0.0b3/
+-rw-rw-rw-   0        0        0    11357 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/LICENSE
+-rw-rw-rw-   0        0        0      118 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10014 2021-06-17 15:28:40.178935 pyoptimus-3.0.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     7412 2021-06-17 15:18:56.000000 pyoptimus-3.0.0b3/README.md
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.905873 pyoptimus-3.0.0b3/optimus/
+-rw-rw-rw-   0        0        0      354 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.906874 pyoptimus-3.0.0b3/optimus/css/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/css/__init__.py
+-rw-rw-rw-   0        0        0      997 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/css/styles.css
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.908875 pyoptimus-3.0.0b3/optimus/engines/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.923877 pyoptimus-3.0.0b3/optimus/engines/base/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/__init__.py
+-rw-rw-rw-   0        0        0    30906 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/basedataframe.py
+-rw-rw-rw-   0        0        0    94652 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/columns.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.926880 pyoptimus-3.0.0b3/optimus/engines/base/commons/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/commons/__init__.py
+-rw-rw-rw-   0        0        0     7459 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/commons/functions.py
+-rw-rw-rw-   0        0        0       71 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/contants.py
+-rw-rw-rw-   0        0        0      658 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/create.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.928877 pyoptimus-3.0.0b3/optimus/engines/base/cudf/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/cudf/__init__.py
+-rw-rw-rw-   0        0        0      148 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/cudf/columns.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.934879 pyoptimus-3.0.0b3/optimus/engines/base/dask/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/__init__.py
+-rw-rw-rw-   0        0        0     6899 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/columns.py
+-rw-rw-rw-   0        0        0     2144 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/constants.py
+-rw-rw-rw-   0        0        0     7830 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/dataframe.py
+-rw-rw-rw-   0        0        0     1811 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.936879 pyoptimus-3.0.0b3/optimus/engines/base/dask/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/io/__init__.py
+-rw-rw-rw-   0        0        0    16855 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/io/jdbc.py
+-rw-rw-rw-   0        0        0     6997 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dask/rows.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.939880 pyoptimus-3.0.0b3/optimus/engines/base/dataframe/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dataframe/__init__.py
+-rw-rw-rw-   0        0        0     4863 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dataframe/columns.py
+-rw-rw-rw-   0        0        0     6837 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/dataframe/dataframe.py
+-rw-rw-rw-   0        0        0      896 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/engine.py
+-rw-rw-rw-   0        0        0    14674 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.955885 pyoptimus-3.0.0b3/optimus/engines/base/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/__init__.py
+-rw-rw-rw-   0        0        0     9132 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/connect.py
+-rw-rw-rw-   0        0        0     1325 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/driver_context.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.968887 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/__init__.py
+-rw-rw-rw-   0        0        0     2131 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/abstract_driver.py
+-rw-rw-rw-   0        0        0     1269 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/bigquery.py
+-rw-rw-rw-   0        0        0      912 2021-06-14 14:00:20.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/cassandra.py
+-rw-rw-rw-   0        0        0     1659 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/impala.py
+-rw-rw-rw-   0        0        0     1656 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/mysql.py
+-rw-rw-rw-   0        0        0     1641 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/oracle.py
+-rw-rw-rw-   0        0        0     1906 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/postgresql.py
+-rw-rw-rw-   0        0        0     1359 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/presto.py
+-rw-rw-rw-   0        0        0     1618 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/redshift.py
+-rw-rw-rw-   0        0        0     1112 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/sqlite.py
+-rw-rw-rw-   0        0        0     1151 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/sqlserver.py
+-rw-rw-rw-   0        0        0     2544 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/factory.py
+-rw-rw-rw-   0        0        0     5394 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/load.py
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/io/save.py
+-rw-rw-rw-   0        0        0     7451 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/mask.py
+-rw-rw-rw-   0        0        0     3683 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/meta.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.970888 pyoptimus-3.0.0b3/optimus/engines/base/ml/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/ml/__init__.py
+-rw-rw-rw-   0        0        0      360 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/ml/contants.py
+-rw-rw-rw-   0        0        0     2808 2021-06-16 19:39:11.000000 pyoptimus-3.0.0b3/optimus/engines/base/profile.py
+-rw-rw-rw-   0        0        0     9245 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/remote.py
+-rw-rw-rw-   0        0        0    10138 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/rows.py
+-rw-rw-rw-   0        0        0     5718 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/base/stringclustering.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.980890 pyoptimus-3.0.0b3/optimus/engines/cudf/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/__init__.py
+-rw-rw-rw-   0        0        0     9094 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/columns.py
+-rw-rw-rw-   0        0        0     2363 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/constants.py
+-rw-rw-rw-   0        0        0      739 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/create.py
+-rw-rw-rw-   0        0        0       62 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/cudf.py
+-rw-rw-rw-   0        0        0     1941 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/dataframe.py
+-rw-rw-rw-   0        0        0     1178 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/engine.py
+-rw-rw-rw-   0        0        0     3752 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.984891 pyoptimus-3.0.0b3/optimus/engines/cudf/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/io/__init__.py
+-rw-rw-rw-   0        0        0      972 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/io/jdbc.py
+-rw-rw-rw-   0        0        0     8025 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/io/load.py
+-rw-rw-rw-   0        0        0     3769 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/io/save.py
+-rw-rw-rw-   0        0        0      572 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/mask.py
+-rw-rw-rw-   0        0        0     3855 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/cudf/rows.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.996894 pyoptimus-3.0.0b3/optimus/engines/dask/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/__init__.py
+-rw-rw-rw-   0        0        0     1880 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/columns.py
+-rw-rw-rw-   0        0        0     1064 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/create.py
+-rw-rw-rw-   0        0        0      887 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/dask.py
+-rw-rw-rw-   0        0        0     1830 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/dataframe.py
+-rw-rw-rw-   0        0        0     5122 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/engine.py
+-rw-rw-rw-   0        0        0     3921 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:39.999894 pyoptimus-3.0.0b3/optimus/engines/dask/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/io/__init__.py
+-rw-rw-rw-   0        0        0      925 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/io/jdbc.py
+-rw-rw-rw-   0        0        0    11407 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/io/load.py
+-rw-rw-rw-   0        0        0     3976 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/io/save.py
+-rw-rw-rw-   0        0        0      613 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/mask.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.002895 pyoptimus-3.0.0b3/optimus/engines/dask/ml/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/ml/__init__.py
+-rw-rw-rw-   0        0        0     3691 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/ml/encoding.py
+-rw-rw-rw-   0        0        0     4199 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/ml/models.py
+-rw-rw-rw-   0        0        0      160 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask/rows.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.013897 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/__init__.py
+-rw-rw-rw-   0        0        0     4896 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/columns.py
+-rw-rw-rw-   0        0        0      702 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/create.py
+-rw-rw-rw-   0        0        0     1011 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/dask_cudf.py
+-rw-rw-rw-   0        0        0     2344 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/dataframe.py
+-rw-rw-rw-   0        0        0     5673 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/engine.py
+-rw-rw-rw-   0        0        0     3570 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.017898 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/__init__.py
+-rw-rw-rw-   0        0        0     1234 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/jdbc.py
+-rw-rw-rw-   0        0        0     8338 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/load.py
+-rw-rw-rw-   0        0        0     3113 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/save.py
+-rw-rw-rw-   0        0        0      576 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/mask.py
+-rw-rw-rw-   0        0        0      659 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/dask_cudf/rows.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.024900 pyoptimus-3.0.0b3/optimus/engines/ibis/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/__init__.py
+-rw-rw-rw-   0        0        0     6224 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/columns.py
+-rw-rw-rw-   0        0        0     1634 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/dataframe.py
+-rw-rw-rw-   0        0        0     1073 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/engine.py
+-rw-rw-rw-   0        0        0     4184 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.026899 pyoptimus-3.0.0b3/optimus/engines/ibis/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/io/__init__.py
+-rw-rw-rw-   0        0        0     3840 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/io/jdbc.py
+-rw-rw-rw-   0        0        0     3603 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/io/save.py
+-rw-rw-rw-   0        0        0     5202 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/ibis/rows.py
+-rw-rw-rw-   0        0        0     3927 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/jit.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.038902 pyoptimus-3.0.0b3/optimus/engines/pandas/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3065 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/columns.py
+-rw-rw-rw-   0        0        0     2090 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/constants.py
+-rw-rw-rw-   0        0        0      651 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/create.py
+-rw-rw-rw-   0        0        0     2129 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/dataframe.py
+-rw-rw-rw-   0        0        0     1339 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/engine.py
+-rw-rw-rw-   0        0        0     3500 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.044903 pyoptimus-3.0.0b3/optimus/engines/pandas/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/__init__.py
+-rw-rw-rw-   0        0        0     1400 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/extract.py
+-rw-rw-rw-   0        0        0      759 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/jdbc.py
+-rw-rw-rw-   0        0        0     4259 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/json.py
+-rw-rw-rw-   0        0        0    10296 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/load.py
+-rw-rw-rw-   0        0        0     3702 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/io/save.py
+-rw-rw-rw-   0        0        0      534 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/mask.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.047905 pyoptimus-3.0.0b3/optimus/engines/pandas/ml/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/ml/__init__.py
+-rw-rw-rw-   0        0        0     3178 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/ml/encoding.py
+-rw-rw-rw-   0        0        0     3637 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/ml/keycollision.py
+-rw-rw-rw-   0        0        0    19341 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/ml/models.py
+-rw-rw-rw-   0        0        0       66 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/pandas.py
+-rw-rw-rw-   0        0        0     3744 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/pandas/rows.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.059908 pyoptimus-3.0.0b3/optimus/engines/spark/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/__init__.py
+-rw-rw-rw-   0        0        0     4787 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/audf.py
+-rw-rw-rw-   0        0        0    70116 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/columns.py
+-rw-rw-rw-   0        0        0     3477 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/constants.py
+-rw-rw-rw-   0        0        0     2226 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/create.py
+-rw-rw-rw-   0        0        0    12142 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/dataframe.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.061909 pyoptimus-3.0.0b3/optimus/engines/spark/dl/
+-rw-rw-rw-   0        0        0      125 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/dl/__init__.py
+-rw-rw-rw-   0        0        0     1729 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/dl/models.py
+-rw-rw-rw-   0        0        0    15582 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/engine.py
+-rw-rw-rw-   0        0        0    12877 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.067910 pyoptimus-3.0.0b3/optimus/engines/spark/io/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/io/__init__.py
+-rw-rw-rw-   0        0        0     8570 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/io/jdbc.py
+-rw-rw-rw-   0        0        0     7775 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/io/load.py
+-rw-rw-rw-   0        0        0     1818 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/io/properties.py
+-rw-rw-rw-   0        0        0     6505 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/io/save.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.073910 pyoptimus-3.0.0b3/optimus/engines/spark/ml/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/__init__.py
+-rw-rw-rw-   0        0        0     3542 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/distancecluster.py
+-rw-rw-rw-   0        0        0     6559 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/encoding.py
+-rw-rw-rw-   0        0        0     5158 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/keycollision.py
+-rw-rw-rw-   0        0        0     4360 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/models.py
+-rw-rw-rw-   0        0        0     7695 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/ml/pipelines.py
+-rw-rw-rw-   0        0        0     9903 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/rows.py
+-rw-rw-rw-   0        0        0     2442 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/engines/spark/spark.py
+-rw-rw-rw-   0        0        0    21312 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/expressions.py
+-rw-rw-rw-   0        0        0     1082 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.096916 pyoptimus-3.0.0b3/optimus/helpers/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/__init__.py
+-rw-rw-rw-   0        0        0     3999 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/check.py
+-rw-rw-rw-   0        0        0    13712 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/columns.py
+-rw-rw-rw-   0        0        0     7646 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/columns_expression.py
+-rw-rw-rw-   0        0        0    16166 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/constants.py
+-rw-rw-rw-   0        0        0     3239 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/converter.py
+-rw-rw-rw-   0        0        0      530 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/core.py
+-rw-rw-rw-   0        0        0      590 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/debug.py
+-rw-rw-rw-   0        0        0      406 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/decorators.py
+-rw-rw-rw-   0        0        0      135 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/exceptions.py
+-rw-rw-rw-   0        0        0      274 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/filters.py
+-rw-rw-rw-   0        0        0    18408 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/functions.py
+-rw-rw-rw-   0        0        0     2152 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/functions_spark.py
+-rw-rw-rw-   0        0        0     1836 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/io.py
+-rw-rw-rw-   0        0        0     1260 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/json.py
+-rw-rw-rw-   0        0        0     1154 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/logger.py
+-rw-rw-rw-   0        0        0     1415 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/output.py
+-rw-rw-rw-   0        0        0     2738 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/parser.py
+-rw-rw-rw-   0        0        0      245 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/pickle.py
+-rw-rw-rw-   0        0        0     3371 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/raiseit.py
+-rw-rw-rw-   0        0        0    10344 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/helpers/test.py
+-rw-rw-rw-   0        0        0    14613 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/infer.py
+-rw-rw-rw-   0        0        0     4608 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/infer_spark.py
+-rw-rw-rw-   0        0        0     2701 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/optimus.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.106919 pyoptimus-3.0.0b3/optimus/outliers/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/__init__.py
+-rw-rw-rw-   0        0        0     4066 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/abstract_outliers_bounds.py
+-rw-rw-rw-   0        0        0     2266 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/abstract_outliers_threshold.py
+-rw-rw-rw-   0        0        0     2174 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/mad.py
+-rw-rw-rw-   0        0        0     1730 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/modified_z_score.py
+-rw-rw-rw-   0        0        0      818 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/outliers.py
+-rw-rw-rw-   0        0        0     2025 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/tukey.py
+-rw-rw-rw-   0        0        0     1223 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/outliers/z_score.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.109922 pyoptimus-3.0.0b3/optimus/plots/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/plots/__init__.py
+-rw-rw-rw-   0        0        0     7589 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/plots/functions.py
+-rw-rw-rw-   0        0        0     3845 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/plots/plots.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.113920 pyoptimus-3.0.0b3/optimus/profiler/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/__init__.py
+-rw-rw-rw-   0        0        0       17 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/constants.py
+-rw-rw-rw-   0        0        0     2333 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/functions.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.114920 pyoptimus-3.0.0b3/optimus/profiler/templates/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/templates/__init__.py
+-rw-rw-rw-   0        0        0      491 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/templates/html.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.118921 pyoptimus-3.0.0b3/optimus/profiler/templates/out/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/templates/out/__init__.py
+-rw-rw-rw-   0        0        0     2256 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/templates/out/general_info.html
+-rw-rw-rw-   0        0        0    11481 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/profiler/templates/out/one_column.html
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.119921 pyoptimus-3.0.0b3/optimus/templates/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.121922 pyoptimus-3.0.0b3/optimus/templates/out/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/templates/out/__init__.py
+-rw-rw-rw-   0        0        0     1883 2021-06-14 14:00:21.000000 pyoptimus-3.0.0b3/optimus/templates/out/table.html
+-rw-rw-rw-   0        0        0      196 2021-06-17 15:22:44.000000 pyoptimus-3.0.0b3/optimus/version.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.139927 pyoptimus-3.0.0b3/pyoptimus.egg-info/
+-rw-rw-rw-   0        0        0    10014 2021-06-17 15:28:39.000000 pyoptimus-3.0.0b3/pyoptimus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7630 2021-06-17 15:28:39.000000 pyoptimus-3.0.0b3/pyoptimus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-17 15:28:39.000000 pyoptimus-3.0.0b3/pyoptimus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1400 2021-06-17 15:28:39.000000 pyoptimus-3.0.0b3/pyoptimus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2021-06-17 15:28:39.000000 pyoptimus-3.0.0b3/pyoptimus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      211 2021-06-17 15:28:40.187936 pyoptimus-3.0.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2021-06-17 03:49:31.000000 pyoptimus-3.0.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.168932 pyoptimus-3.0.0b3/tests/
+-rw-rw-rw-   0        0        0        2 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-17 15:28:40.176934 pyoptimus-3.0.0b3/tests/creator/
+-rw-rw-rw-   0        0        0        0 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/creator/__init__.py
+-rw-rw-rw-   0        0        0    30062 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/creator/creator-cudf.py
+-rw-rw-rw-   0        0        0     5015 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/creator/creator-dask-debug.py
+-rw-rw-rw-   0        0        0    29943 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/creator/creator-dask.py
+-rw-rw-rw-   0        0        0     4128 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/creator/creator-ext.py
+-rw-rw-rw-   0        0        0     4787 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/creator/creator-profiler.py
+-rw-rw-rw-   0        0        0    36136 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/creator/creator.py
+-rw-rw-rw-   0        0        0    29715 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/creator/cudf.py
+-rw-rw-rw-   0        0        0     1482 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_dataframe.py
+-rw-rw-rw-   0        0        0   249989 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_cols.py
+-rw-rw-rw-   0        0        0     9569 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_cols_2.py
+-rw-rw-rw-   0        0        0   239031 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_cols_dask.py
+-rw-rw-rw-   0        0        0   402343 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_cols_pandas.py
+-rw-rw-rw-   0        0        0  1327275 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_distance_cluster.py
+-rw-rw-rw-   0        0        0     6638 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_ext.py
+-rw-rw-rw-   0        0        0    48170 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_keycollision.py
+-rw-rw-rw-   0        0        0     1649 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_ml_2.py
+-rw-rw-rw-   0        0        0    17841 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_outliers.py
+-rw-rw-rw-   0        0        0     6551 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_profiler.py
+-rw-rw-rw-   0        0        0     4789 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_df_rows.py
+-rw-rw-rw-   0        0        0     1511 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_dl.py
+-rw-rw-rw-   0        0        0      904 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/test_example_notebooks.py
+-rw-rw-rw-   0        0        0    10090 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_meta.py
+-rw-rw-rw-   0        0        0     4832 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_ml.py
+-rw-rw-rw-   0        0        0    15604 2021-06-17 00:24:56.000000 pyoptimus-3.0.0b3/tests/test_op_io.py
+-rw-rw-rw-   0        0        0     2398 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_optimus.py
+-rw-rw-rw-   0        0        0      408 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_optimus_spark_session.py
+-rw-rw-rw-   0        0        0     9235 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_plot.py
+-rw-rw-rw-   0        0        0     3227 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_profiler.py
+-rw-rw-rw-   0        0        0     8199 2021-06-14 14:00:22.000000 pyoptimus-3.0.0b3/tests/test_sql.py
```

### Comparing `pyoptimus-3.0.0b2/LICENSE` & `pyoptimus-3.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/css/styles.css` & `pyoptimus-3.0.0b3/optimus/css/styles.css`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/basedataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/base/basedataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/base/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/commons/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/base/commons/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/create.py` & `pyoptimus-3.0.0b3/optimus/engines/base/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/constants.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/constants.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dask/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dask/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dataframe/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dataframe/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/dataframe/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/base/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/base/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/base/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/connect.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/connect.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/driver_context.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/driver_context.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/abstract_driver.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/abstract_driver.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/bigquery.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/bigquery.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/cassandra.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/cassandra.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/impala.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/impala.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/mysql.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/mysql.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/oracle.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/oracle.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/postgresql.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/postgresql.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/presto.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/presto.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/redshift.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/redshift.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/sqlite.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/drivers/sqlserver.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/drivers/sqlserver.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/factory.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/factory.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/base/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/mask.py` & `pyoptimus-3.0.0b3/optimus/engines/base/mask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/meta.py` & `pyoptimus-3.0.0b3/optimus/engines/base/meta.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/profile.py` & `pyoptimus-3.0.0b3/optimus/engines/base/profile.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/remote.py` & `pyoptimus-3.0.0b3/optimus/engines/base/remote.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/base/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/base/stringclustering.py` & `pyoptimus-3.0.0b3/optimus/engines/base/stringclustering.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/constants.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/constants.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/create.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/mask.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/mask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/cudf/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/cudf/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/create.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/dask.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/dask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/mask.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/mask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/ml/encoding.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask/ml/models.py` & `pyoptimus-3.0.0b3/optimus/engines/dask/ml/models.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/create.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/dask_cudf.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/dask_cudf.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/mask.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/mask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/dask_cudf/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/dask_cudf/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/ibis/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/ibis/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/jit.py` & `pyoptimus-3.0.0b3/optimus/engines/jit.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/constants.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/constants.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/create.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/io/extract.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/io/extract.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/io/json.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/io/json.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/mask.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/mask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/ml/encoding.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/ml/keycollision.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/ml/keycollision.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/ml/models.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/ml/models.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/pandas/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/pandas/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/audf.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/audf.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/columns.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/constants.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/constants.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/create.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/create.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/dataframe.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/dl/models.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/dl/models.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/engine.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/engine.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/functions.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/io/jdbc.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/io/jdbc.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/io/load.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/io/load.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/io/properties.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/io/properties.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/io/save.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/io/save.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/ml/distancecluster.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/ml/distancecluster.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/ml/encoding.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/ml/encoding.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/ml/keycollision.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/ml/keycollision.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/ml/models.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/ml/models.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/ml/pipelines.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/ml/pipelines.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/rows.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/engines/spark/spark.py` & `pyoptimus-3.0.0b3/optimus/engines/spark/spark.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/expressions.py` & `pyoptimus-3.0.0b3/optimus/expressions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/functions.py` & `pyoptimus-3.0.0b3/optimus/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/check.py` & `pyoptimus-3.0.0b3/optimus/helpers/check.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/columns.py` & `pyoptimus-3.0.0b3/optimus/helpers/columns.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/columns_expression.py` & `pyoptimus-3.0.0b3/optimus/helpers/columns_expression.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/constants.py` & `pyoptimus-3.0.0b3/optimus/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/converter.py` & `pyoptimus-3.0.0b3/optimus/helpers/converter.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/core.py` & `pyoptimus-3.0.0b3/optimus/helpers/core.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/debug.py` & `pyoptimus-3.0.0b3/optimus/helpers/debug.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/functions.py` & `pyoptimus-3.0.0b3/optimus/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/functions_spark.py` & `pyoptimus-3.0.0b3/optimus/helpers/functions_spark.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/io.py` & `pyoptimus-3.0.0b3/optimus/helpers/io.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/json.py` & `pyoptimus-3.0.0b3/optimus/helpers/json.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/logger.py` & `pyoptimus-3.0.0b3/optimus/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/output.py` & `pyoptimus-3.0.0b3/optimus/helpers/output.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/parser.py` & `pyoptimus-3.0.0b3/optimus/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/raiseit.py` & `pyoptimus-3.0.0b3/optimus/helpers/raiseit.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/helpers/test.py` & `pyoptimus-3.0.0b3/optimus/helpers/test.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/infer.py` & `pyoptimus-3.0.0b3/optimus/infer.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/infer_spark.py` & `pyoptimus-3.0.0b3/optimus/infer_spark.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/optimus.py` & `pyoptimus-3.0.0b3/optimus/optimus.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/abstract_outliers_bounds.py` & `pyoptimus-3.0.0b3/optimus/outliers/abstract_outliers_bounds.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/abstract_outliers_threshold.py` & `pyoptimus-3.0.0b3/optimus/outliers/abstract_outliers_threshold.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/mad.py` & `pyoptimus-3.0.0b3/optimus/outliers/mad.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/modified_z_score.py` & `pyoptimus-3.0.0b3/optimus/outliers/modified_z_score.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/outliers.py` & `pyoptimus-3.0.0b3/optimus/outliers/outliers.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/tukey.py` & `pyoptimus-3.0.0b3/optimus/outliers/tukey.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/outliers/z_score.py` & `pyoptimus-3.0.0b3/optimus/outliers/z_score.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/plots/functions.py` & `pyoptimus-3.0.0b3/optimus/plots/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/plots/plots.py` & `pyoptimus-3.0.0b3/optimus/plots/plots.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/profiler/functions.py` & `pyoptimus-3.0.0b3/optimus/profiler/functions.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/profiler/templates/out/general_info.html` & `pyoptimus-3.0.0b3/optimus/profiler/templates/out/general_info.html`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/profiler/templates/out/one_column.html` & `pyoptimus-3.0.0b3/optimus/profiler/templates/out/one_column.html`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/optimus/templates/out/table.html` & `pyoptimus-3.0.0b3/optimus/templates/out/table.html`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/pyoptimus.egg-info/SOURCES.txt` & `pyoptimus-3.0.0b3/pyoptimus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/pyoptimus.egg-info/requires.txt` & `pyoptimus-3.0.0b3/pyoptimus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/setup.py` & `pyoptimus-3.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator-cudf.py` & `pyoptimus-3.0.0b3/tests/creator/creator-cudf.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator-dask-debug.py` & `pyoptimus-3.0.0b3/tests/creator/creator-dask-debug.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator-dask.py` & `pyoptimus-3.0.0b3/tests/creator/creator-dask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator-ext.py` & `pyoptimus-3.0.0b3/tests/creator/creator-ext.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator-profiler.py` & `pyoptimus-3.0.0b3/tests/creator/creator-profiler.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/creator.py` & `pyoptimus-3.0.0b3/tests/creator/creator.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/creator/cudf.py` & `pyoptimus-3.0.0b3/tests/creator/cudf.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_dataframe.py` & `pyoptimus-3.0.0b3/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_cols.py` & `pyoptimus-3.0.0b3/tests/test_df_cols.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_cols_2.py` & `pyoptimus-3.0.0b3/tests/test_df_cols_2.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_cols_dask.py` & `pyoptimus-3.0.0b3/tests/test_df_cols_dask.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_cols_pandas.py` & `pyoptimus-3.0.0b3/tests/test_df_cols_pandas.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_distance_cluster.py` & `pyoptimus-3.0.0b3/tests/test_df_distance_cluster.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_ext.py` & `pyoptimus-3.0.0b3/tests/test_df_ext.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_keycollision.py` & `pyoptimus-3.0.0b3/tests/test_df_keycollision.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_ml_2.py` & `pyoptimus-3.0.0b3/tests/test_df_ml_2.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_outliers.py` & `pyoptimus-3.0.0b3/tests/test_df_outliers.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_profiler.py` & `pyoptimus-3.0.0b3/tests/test_df_profiler.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_df_rows.py` & `pyoptimus-3.0.0b3/tests/test_df_rows.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_dl.py` & `pyoptimus-3.0.0b3/tests/test_dl.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_example_notebooks.py` & `pyoptimus-3.0.0b3/tests/test_example_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_meta.py` & `pyoptimus-3.0.0b3/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_ml.py` & `pyoptimus-3.0.0b3/tests/test_ml.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_op_io.py` & `pyoptimus-3.0.0b3/tests/test_op_io.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_optimus.py` & `pyoptimus-3.0.0b3/tests/test_optimus.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_plot.py` & `pyoptimus-3.0.0b3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_profiler.py` & `pyoptimus-3.0.0b3/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `pyoptimus-3.0.0b2/tests/test_sql.py` & `pyoptimus-3.0.0b3/tests/test_sql.py`

 * *Files identical despite different names*

