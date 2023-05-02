# Comparing `tmp/oceanum-0.7.4.tar.gz` & `tmp/oceanum-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.7.4.tar", last modified: Fri Jan 27 07:48:08 2023, max compression
+gzip compressed data, was "oceanum-0.7.5.tar", last modified: Tue May  2 20:34:52 2023, max compression
```

## Comparing `oceanum-0.7.4.tar` & `oceanum-0.7.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.274113 oceanum-0.7.4/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2022-03-11 03:30:04.000000 oceanum-0.7.4/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2022-02-24 22:26:12.000000 oceanum-0.7.4/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2022-05-20 01:30:23.000000 oceanum-0.7.4/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2022-02-24 22:26:12.000000 oceanum-0.7.4/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2022-02-24 22:26:12.000000 oceanum-0.7.4/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-01-27 07:48:08.274113 oceanum-0.7.4/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2022-05-20 01:30:52.000000 oceanum-0.7.4/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.258113 oceanum-0.7.4/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2022-03-11 19:57:18.000000 oceanum-0.7.4/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.250113 oceanum-0.7.4/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.250113 oceanum-0.7.4/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.258113 oceanum-0.7.4/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2022-12-01 21:44:17.000000 oceanum-0.7.4/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.4/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.4/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.250113 oceanum-0.7.4/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.258113 oceanum-0.7.4/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2022-03-11 19:44:27.000000 oceanum-0.7.4/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2022-04-07 02:34:44.000000 oceanum-0.7.4/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2022-09-21 00:26:04.000000 oceanum-0.7.4/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.254113 oceanum-0.7.4/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.262113 oceanum-0.7.4/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2022-04-08 05:43:00.000000 oceanum-0.7.4/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2022-09-21 00:26:04.000000 oceanum-0.7.4/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2022-09-21 00:26:04.000000 oceanum-0.7.4/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2022-04-08 05:43:00.000000 oceanum-0.7.4/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2022-09-21 00:26:04.000000 oceanum-0.7.4/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      160 2022-10-12 22:11:24.000000 oceanum-0.7.4/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2022-03-11 04:02:04.000000 oceanum-0.7.4/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2022-03-11 19:49:35.000000 oceanum-0.7.4/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-01-10 19:39:49.000000 oceanum-0.7.4/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-01-10 19:32:56.000000 oceanum-0.7.4/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-01-10 19:39:49.000000 oceanum-0.7.4/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2022-10-12 19:27:10.000000 oceanum-0.7.4/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.262113 oceanum-0.7.4/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-01-23 08:55:30.000000 oceanum-0.7.4/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2022-03-11 20:11:41.000000 oceanum-0.7.4/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.266113 oceanum-0.7.4/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2022-03-11 20:13:21.000000 oceanum-0.7.4/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2022-11-15 20:33:48.000000 oceanum-0.7.4/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    20495 2023-01-16 20:20:49.000000 oceanum-0.7.4/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-01-27 07:47:32.000000 oceanum-0.7.4/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-01-16 20:20:49.000000 oceanum-0.7.4/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     6888 2022-12-07 23:59:25.000000 oceanum-0.7.4/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4683 2023-01-26 06:10:28.000000 oceanum-0.7.4/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.262113 oceanum-0.7.4/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-01-27 07:48:08.000000 oceanum-0.7.4/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-01-27 07:48:08.274113 oceanum-0.7.4/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2022-12-12 20:30:18.000000 oceanum-0.7.4/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.266113 oceanum-0.7.4/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-02-24 22:26:12.000000 oceanum-0.7.4/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-01-27 07:48:08.274113 oceanum-0.7.4/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2022-09-21 00:26:04.000000 oceanum-0.7.4/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2022-12-12 20:29:37.000000 oceanum-0.7.4/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2022-09-21 00:26:04.000000 oceanum-0.7.4/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2022-11-15 08:03:53.000000 oceanum-0.7.4/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2022-11-15 03:23:40.000000 oceanum-0.7.4/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2022-09-28 03:24:15.000000 oceanum-0.7.4/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2022-10-09 05:38:00.000000 oceanum-0.7.4/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-01-16 20:20:49.000000 oceanum-0.7.4/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2022-10-26 22:51:30.000000 oceanum-0.7.4/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      684 2022-07-06 05:55:09.000000 oceanum-0.7.4/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2022-12-12 20:29:37.000000 oceanum-0.7.4/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.655561 oceanum-0.7.5/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2022-03-11 03:30:04.000000 oceanum-0.7.5/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2022-02-24 22:26:12.000000 oceanum-0.7.5/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       89 2022-05-20 01:30:23.000000 oceanum-0.7.5/HISTORY.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2022-02-24 22:26:12.000000 oceanum-0.7.5/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2022-02-24 22:26:12.000000 oceanum-0.7.5/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-05-02 20:34:52.655561 oceanum-0.7.5/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2022-05-20 01:30:52.000000 oceanum-0.7.5/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.639561 oceanum-0.7.5/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2022-03-11 19:57:18.000000 oceanum-0.7.5/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.635561 oceanum-0.7.5/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.635561 oceanum-0.7.5/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.643561 oceanum-0.7.5/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2022-12-01 21:44:17.000000 oceanum-0.7.5/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.5/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.5/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.635561 oceanum-0.7.5/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.643561 oceanum-0.7.5/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2022-03-11 19:44:27.000000 oceanum-0.7.5/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2022-04-07 02:34:44.000000 oceanum-0.7.5/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2022-09-21 00:26:04.000000 oceanum-0.7.5/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.635561 oceanum-0.7.5/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.643561 oceanum-0.7.5/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2022-04-08 05:43:00.000000 oceanum-0.7.5/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2022-09-21 00:26:04.000000 oceanum-0.7.5/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2022-09-21 00:26:04.000000 oceanum-0.7.5/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2022-04-08 05:43:00.000000 oceanum-0.7.5/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2022-09-21 00:26:04.000000 oceanum-0.7.5/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      160 2022-10-12 22:11:24.000000 oceanum-0.7.5/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2022-03-11 04:02:04.000000 oceanum-0.7.5/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2022-03-11 19:49:35.000000 oceanum-0.7.5/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-01-10 19:39:49.000000 oceanum-0.7.5/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-01-10 19:32:56.000000 oceanum-0.7.5/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-01-10 19:39:49.000000 oceanum-0.7.5/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2022-10-12 19:27:10.000000 oceanum-0.7.5/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.643561 oceanum-0.7.5/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-05-02 20:31:18.000000 oceanum-0.7.5/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2022-03-11 20:11:41.000000 oceanum-0.7.5/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.647561 oceanum-0.7.5/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2022-03-11 20:13:21.000000 oceanum-0.7.5/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2022-11-15 20:33:48.000000 oceanum-0.7.5/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    20478 2023-05-02 20:29:57.000000 oceanum-0.7.5/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-03-21 00:40:55.000000 oceanum-0.7.5/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-01-16 20:20:49.000000 oceanum-0.7.5/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7113 2023-03-20 01:52:59.000000 oceanum-0.7.5/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4683 2023-03-20 03:18:19.000000 oceanum-0.7.5/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.647561 oceanum-0.7.5/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-05-02 20:34:52.000000 oceanum-0.7.5/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-05-02 20:34:52.659560 oceanum-0.7.5/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2022-12-12 20:30:18.000000 oceanum-0.7.5/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.651561 oceanum-0.7.5/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-02-24 22:26:12.000000 oceanum-0.7.5/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-02 20:34:52.655561 oceanum-0.7.5/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2022-09-21 00:26:04.000000 oceanum-0.7.5/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2022-12-12 20:29:37.000000 oceanum-0.7.5/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2022-09-21 00:26:04.000000 oceanum-0.7.5/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2022-11-15 08:03:53.000000 oceanum-0.7.5/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2022-11-15 03:23:40.000000 oceanum-0.7.5/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2022-09-28 03:24:15.000000 oceanum-0.7.5/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2022-10-09 05:38:00.000000 oceanum-0.7.5/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-01-16 20:20:49.000000 oceanum-0.7.5/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2022-10-26 22:51:30.000000 oceanum-0.7.5/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-03-06 19:00:50.000000 oceanum-0.7.5/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2022-12-12 20:29:37.000000 oceanum-0.7.5/tests/test_video_compat.py
```

### Comparing `oceanum-0.7.4/CONTRIBUTING.rst` & `oceanum-0.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/LICENSE` & `oceanum-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/PKG-INFO` & `oceanum-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.4
+Version: 0.7.5
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.4/README.rst` & `oceanum-0.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/Makefile` & `oceanum-0.7.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/api.rst` & `oceanum-0.7.5/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.7.5/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/conf.py` & `oceanum-0.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/installation.rst` & `oceanum-0.7.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/make.bat` & `oceanum-0.7.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/oceanum.datamesh.rst` & `oceanum-0.7.5/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/docs/usage.rst` & `oceanum-0.7.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/oceanum/datamesh/catalog.py` & `oceanum-0.7.5/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/oceanum/datamesh/connection.py` & `oceanum-0.7.5/oceanum/datamesh/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             geofilter (Union[:obj:`oceanum.datamesh.query.GeoFilter`, dict, shapely.geometry], Optional): Spatial filter as valid Query Geofilter or geojson geometry as dict or shapely Geometry
 
         Returns:
             :obj:`oceanum.datamesh.Catalog`: A datamesh catalog instance
         """
         query = {}
         if search:
-            query["search"] = search.replace(" ", ",")
+            query["search"] = search
         if timefilter:
             times = TimeFilter(times=timefilter).times
             query["in_trange"] = f"{times[0]}Z,{times[1]}Z"
         if geofilter:
             if isinstance(geofilter, GeoFilter):
                 geos = geofilter.geom
             else:
@@ -469,15 +469,15 @@
             if key not in ["driver", "schema"]:
                 setattr(ds, key, properties[key])
         if geometry:
             ds.geom = geometry
         try:
             self._metadata_write(ds)
         except:
-            raise DatameshWriteError("Cannot register datasource {datasource_id}: {e}")
+            raise DatameshWriteError(f"Cannot register datasource {datasource_id}: {e}")
         return ds
 
     @asyncwrapper
     def write_datasource_async(
         self, datasource_id, data, append=None, overwrite=False, **properties
     ):
         """Write a datasource to datamesh from the work environment asynchronously
```

### Comparing `oceanum-0.7.4/oceanum/datamesh/datasource.py` & `oceanum-0.7.5/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/oceanum/datamesh/query.py` & `oceanum-0.7.5/oceanum/datamesh/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,17 @@
         description="""
             - For type='range', [timestart, tend].
         """,
     )
     resolution: Optional[str] = Field(
         title="Temporal resolution of data",
         default="native",
-        description="Maximum resolution of the data for temporal downsampling. Only valid with range type",
+        description=""""
+            Maximum resolution of the data for temporal downsampling. 
+            Must be a valid pandas [DateOffset.freqstr](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.tseries.offsets.DateOffset.freqstr.html#pandas.tseries.offsets.DateOffset.freqstr). Only valid with range type""",
     )
     resample: Optional[ResampleType] = Field(
         title="Temporal resampling method",
         default=ResampleType.mean,
         description="Resampling method applied when reducing tempral resolution. Only valid with range type",
     )
```

### Comparing `oceanum-0.7.4/oceanum/datamesh/zarr.py` & `oceanum-0.7.5/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/oceanum.egg-info/PKG-INFO` & `oceanum-0.7.5/oceanum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.4
+Version: 0.7.5
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.4/oceanum.egg-info/SOURCES.txt` & `oceanum-0.7.5/oceanum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/setup.py` & `oceanum-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/data/grid_data_1.nc` & `oceanum-0.7.5/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/data/ocean_test_1.mp4` & `oceanum-0.7.5/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/data/point_data_1.csv` & `oceanum-0.7.5/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_catalog.py` & `oceanum-0.7.5/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_datamesh_connect.py` & `oceanum-0.7.5/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_datamesh_load.py` & `oceanum-0.7.5/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_datamesh_query.py` & `oceanum-0.7.5/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_datamesh_write.py` & `oceanum-0.7.5/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_datasource.py` & `oceanum-0.7.5/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.4/tests/test_video_compat.py` & `oceanum-0.7.5/tests/test_video_compat.py`

 * *Files identical despite different names*

