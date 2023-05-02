# Comparing `tmp/pyrsm-0.7.9.1.tar.gz` & `tmp/pyrsm-0.7.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.7.9.1.tar", last modified: Sat Mar 25 21:33:10 2023, max compression
+gzip compressed data, was "pyrsm-0.7.9.2.tar", last modified: Tue May  2 07:26:11 2023, max compression
```

## Comparing `pyrsm-0.7.9.1.tar` & `pyrsm-0.7.9.2.tar`

### file list

```diff
@@ -1,75 +1,74 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.815423 pyrsm-0.7.9.1/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.7.9.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.7.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      594 2023-03-25 21:33:10.815487 pyrsm-0.7.9.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.7.9.1/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.7.9.1/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.809103 pyrsm-0.7.9.1/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      273 2023-03-25 21:31:41.000000 pyrsm-0.7.9.1/pyrsm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    54325 2023-03-05 03:46:45.000000 pyrsm-0.7.9.1/pyrsm/basics.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.7.9.1/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.809763 pyrsm-0.7.9.1/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.810695 pyrsm-0.7.9.1/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/basics/consider.pkl
--rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/basics/demand_uk.pkl
--rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/basics/newspaper.pkl
--rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/basics/salary.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.811512 pyrsm-0.7.9.1/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/avengers.pkl
--rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/diamonds.pkl
--rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/publishers.pkl
--rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/superheroes.pkl
--rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/data/titanic.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.811767 pyrsm-0.7.9.1/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/design/rndnames.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.813126 pyrsm-0.7.9.1/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/catalog.pkl
--rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/direct_marketing.pkl
--rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/dvd.pkl
--rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/houseprices.pkl
--rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/ideal.pkl
--rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/ketchup.pkl
--rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/movie_contract.pkl
--rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/model/ratings.pkl
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.814510 pyrsm-0.7.9.1/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/carpet.pkl
--rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/city.pkl
--rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/city2.pkl
--rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/computer.pkl
--rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/movie.pkl
--rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/mp3.pkl
--rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/retailers.pkl
--rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/shopping.pkl
--rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/toothpaste.pkl
--rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/data/multivariate/tpbrands.pkl
--rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.7.9.1/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2749 2023-01-05 19:05:17.000000 pyrsm-0.7.9.1/pyrsm/logistic_regression.py
--rw-r--r--   0 root         (0) staff       (20)    10788 2023-03-25 07:14:58.000000 pyrsm-0.7.9.1/pyrsm/logit.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.7.9.1/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37516 2023-03-25 08:04:57.000000 pyrsm-0.7.9.1/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/pyrsm/props.py
--rw-r--r--   0 root         (0) staff       (20)    17202 2023-03-20 18:45:59.000000 pyrsm-0.7.9.1/pyrsm/regression.py
--rw-r--r--   0 root         (0) staff       (20)     5397 2023-03-05 06:38:26.000000 pyrsm-0.7.9.1/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    12058 2023-03-25 08:01:05.000000 pyrsm-0.7.9.1/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22812 2023-03-25 08:12:47.000000 pyrsm-0.7.9.1/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.809637 pyrsm-0.7.9.1/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      594 2023-03-25 21:33:10.000000 pyrsm-0.7.9.1/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1661 2023-03-25 21:33:10.000000 pyrsm-0.7.9.1/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-25 21:33:10.000000 pyrsm-0.7.9.1/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      130 2023-03-25 21:33:10.000000 pyrsm-0.7.9.1/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-03-25 21:33:10.000000 pyrsm-0.7.9.1/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)      936 2023-03-25 21:33:10.815842 pyrsm-0.7.9.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-25 21:33:10.815322 pyrsm-0.7.9.1/tests/
--rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.7.9.1/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.7.9.1/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.7.9.1/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.7.9.1/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-01-15 08:28:47.000000 pyrsm-0.7.9.1/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.7.9.1/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.7.9.1/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.588299 pyrsm-0.7.9.2/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.7.9.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      215 2023-03-25 21:03:06.000000 pyrsm-0.7.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      594 2023-05-02 07:26:11.588385 pyrsm-0.7.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-03-25 21:31:10.000000 pyrsm-0.7.9.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.7.9.2/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.581397 pyrsm-0.7.9.2/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      273 2023-05-01 23:50:01.000000 pyrsm-0.7.9.2/pyrsm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    54297 2023-05-02 07:18:43.000000 pyrsm-0.7.9.2/pyrsm/basics.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.7.9.2/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582197 pyrsm-0.7.9.2/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582853 pyrsm-0.7.9.2/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     6996 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/consider.pkl
+-rw-r--r--   0 root         (0) staff       (20)    13754 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/demand_uk.pkl
+-rw-r--r--   0 root         (0) staff       (20)     5508 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/newspaper.pkl
+-rw-r--r--   0 root         (0) staff       (20)     8545 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/basics/salary.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.584075 pyrsm-0.7.9.2/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1620 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/avengers.pkl
+-rw-r--r--   0 root         (0) staff       (20)   207435 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/diamonds.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1557 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/publishers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1660 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/superheroes.pkl
+-rw-r--r--   0 root         (0) staff       (20)    69129 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/data/titanic.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.584353 pyrsm-0.7.9.2/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3414 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/design/rndnames.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.586045 pyrsm-0.7.9.2/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8197 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/catalog.pkl
+-rw-r--r--   0 root         (0) staff       (20)    41039 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/direct_marketing.pkl
+-rw-r--r--   0 root         (0) staff       (20)   342723 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/dvd.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4468 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/houseprices.pkl
+-rw-r--r--   0 root         (0) staff       (20)    33206 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ideal.pkl
+-rw-r--r--   0 root         (0) staff       (20)   126402 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ketchup.pkl
+-rw-r--r--   0 root         (0) staff       (20)      315 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/movie_contract.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3123 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/model/ratings.pkl
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.587357 pyrsm-0.7.9.2/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3125 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/carpet.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2423 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/city.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3923 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/city2.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2625 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/computer.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3442 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/movie.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2994 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/mp3.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3278 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/retailers.pkl
+-rw-r--r--   0 root         (0) staff       (20)     2357 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/shopping.pkl
+-rw-r--r--   0 root         (0) staff       (20)     4872 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/toothpaste.pkl
+-rw-r--r--   0 root         (0) staff       (20)     3678 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/data/multivariate/tpbrands.pkl
+-rw-r--r--   0 root         (0) staff       (20)     1966 2023-01-26 08:23:23.000000 pyrsm-0.7.9.2/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)    16298 2023-05-02 07:18:17.000000 pyrsm-0.7.9.2/pyrsm/logit.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-02-28 23:28:31.000000 pyrsm-0.7.9.2/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.7.9.2/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/pyrsm/props.py
+-rw-r--r--   0 root         (0) staff       (20)    15639 2023-05-02 07:18:33.000000 pyrsm-0.7.9.2/pyrsm/regression.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.7.9.2/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    11145 2023-05-02 07:11:09.000000 pyrsm-0.7.9.2/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    23286 2023-04-30 01:31:14.000000 pyrsm-0.7.9.2/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.582065 pyrsm-0.7.9.2/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      594 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1632 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      130 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-05-02 07:26:11.000000 pyrsm-0.7.9.2/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)      936 2023-05-02 07:26:11.588694 pyrsm-0.7.9.2/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-02 07:26:11.588188 pyrsm-0.7.9.2/tests/
+-rw-r--r--   0 root         (0) staff       (20)      722 2022-03-07 07:21:43.000000 pyrsm-0.7.9.2/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1072 2023-03-05 06:28:28.000000 pyrsm-0.7.9.2/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-01-31 08:59:01.000000 pyrsm-0.7.9.2/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     2756 2023-01-21 01:15:24.000000 pyrsm-0.7.9.2/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-01-15 08:28:47.000000 pyrsm-0.7.9.2/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2036 2023-03-05 06:38:03.000000 pyrsm-0.7.9.2/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     1979 2022-02-13 01:24:09.000000 pyrsm-0.7.9.2/tests/test_utils.py
```

### Comparing `pyrsm-0.7.9.1/LICENSE` & `pyrsm-0.7.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/PKG-INFO` & `pyrsm-0.7.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.7.9.1
+Version: 0.7.9.2
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.7.9.1/README.md` & `pyrsm-0.7.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/basics.py` & `pyrsm-0.7.9.2/pyrsm/basics.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,15 +469,15 @@
 class prob_calc:
     # Probability calculator
     def __init__(self, distribution: str, params: dict) -> None:
         self.distribution = distribution
         self.__dict__.update(params)
         print("Probability calculator")
 
-    def calculate(self):
+    def summary(self):
         print(f"Distribution: {self.distribution}")
 
         def calc_f_dist(
             dfn: int, dfd: int, lb: float = 0, ub: float = 0.95, decimals: int = 3
         ) -> tuple[float, float]:
             print(f"Df 1:\t{dfn}")
             print(f"Df 2:\t{dfd}")
@@ -685,20 +685,15 @@
         comparison_value: float,
     ):
         self.data = data
         self.variable = variable
         self.alt_hypo = alt_hypo
         self.conf = conf
         self.comparison_value = comparison_value
-        self.t_val = None
-        self.p_val = None
 
-        print("Single mean test")
-
-    def calculate(self) -> None:
         result = stats.ttest_1samp(
             a=self.data[self.variable],
             popmean=self.comparison_value,
             nan_policy="omit",
             alternative=self.alt_hypo,
         )
 
@@ -708,28 +703,27 @@
         self.n = len(self.data[self.variable])
         self.n_missing = self.data[self.variable].isna().sum()
 
         self.sd = self.data[self.variable].std()
         self.se = self.data[self.variable].sem()
         z_score = stats.norm.ppf((1 + self.conf) / 2)
 
-        self.me = z_score * self.sd / sqrt(self.n)
+        self.me = (z_score * self.sd / sqrt(self.n)).real
         self.diff = self.mean - self.comparison_value
         self.df = self.n - 1
         self.x_percent = self.mean - stats.t.ppf(self.conf, self.df) * self.se
         self.hundred_percent = self.mean - stats.t.ppf(0, self.df) * self.se
 
     def summary(self, dec=3) -> None:
-        if self.t_val == None:
-            self.calculate()
-        data_name = ""
+        print("Single mean test")
         if hasattr(self.data, "description"):
             data_name = self.data.description.split("\n")[0].split()[1].lower()
-        if len(data_name) > 0:
-            print(f"Data: {data_name}")
+        else:
+            data_name = "Not available"
+        print(f"Data: {data_name}")
         print(f"Variable: {self.variable}")
         print(f"Confidence: {self.conf}")
 
         print(f"Null hyp.: the mean of {self.variable} = {self.comparison_value}")
 
         alt_hypo = ">"
         if self.alt_hypo == "lesser":
@@ -837,16 +831,14 @@
         self.sample_type = sample_type
         self.multiple_comp_adjustment = multiple_comp_adjustment
         self.test_type = test_type
 
         self.t_val = None
         self.p_val = None
 
-        print(f"Pairwise mean comparisons {self.test_type}")
-
         def welch_dof(v1: str, v2: str) -> float:
             x = self.data[self.data[self.var1] == v1][self.var2]
             y = self.data[self.data[self.var1] == v2][self.var2]
             dof = (x.var() / x.size + y.var() / y.size) ** 2 / (
                 (x.var() / x.size) ** 2 / (x.size - 1)
                 + (y.var() / y.size) ** 2 / (y.size - 1)
             )
@@ -934,21 +926,20 @@
                 "df",
                 # "0%",
                 # str(self.conf * 100) + "%",
             ],
         )
 
     def summary(self, dec=3) -> None:
-        if self.t_val == None:
-            self.calculate()
-        data_name = ""
+        print(f"Pairwise mean comparisons {self.test_type}")
         if hasattr(self.data, "description"):
             data_name = self.data.description.split("\n")[0].split()[1].lower()
-        if len(data_name) > 0:
-            print(f"Data: {data_name}")
+        else:
+            data_name = "Not available"
+        print(f"Data: {data_name}")
         print(f"Variables: {self.var1}, {self.var2}")
         print(f"Confidence: {self.conf}")
         print(f"Adjustment: {self.multiple_comp_adjustment}")
 
         print(self.table1.round(dec).to_string(index=False))
         print(self.table2.round(dec).to_string(index=False))
 
@@ -968,48 +959,42 @@
         self.variable = variable
         self.level = level
         self.alt_hypo = alt_hypo
         self.conf = conf
         self.comparison_value = comparison_value
         self.test_type = test_type
 
-        self.p_val = None
-
-        print(f"Single proportion ({self.test_type})")
-
-    def calculate(self) -> None:
         self.ns = len(self.data[self.data[self.variable] == self.level])
         self.n_missing = self.data[self.variable].isna().sum()
         self.n = len(self.data) - self.n_missing
         self.p = self.ns / self.n
-        self.sd = sqrt(self.p * (1 - self.p))
-        self.se = self.sd / sqrt(self.n)
+        self.sd = sqrt(self.p * (1 - self.p)).real
+        self.se = (self.sd / sqrt(self.n)).real
 
-        z_score = stats.norm.ppf((1 + self.conf) / 2)
+        z_score = stats.norm.ppf((1 + self.conf) / 2).real
 
         self.me = z_score * self.se
 
         self.diff = self.p - self.comparison_value
 
         results = stats.binomtest(self.ns, self.n, self.comparison_value, self.alt_hypo)
 
         self.p_val = results.pvalue
         proportion_ci = results.proportion_ci(self.conf)
         self.zero_percent = proportion_ci.low
         self.x_percent = proportion_ci.high
 
     def summary(self) -> None:
-        if self.p_val == None:
-            self.calculate()
-        data_name = ""
+        print(f"Single proportion ({self.test_type})")
         if hasattr(self.data, "description"):
             data_name = self.data.description.split("\n")[0].split()[1].lower()
-        if len(data_name) > 0:
-            print(f"Data: {data_name}")
+        else:
+            data_name = "Not available"
 
+        print(f"Data: {data_name}")
         print(f"Variable: {self.variable}")
         print(f"Level: {self.level} in {self.variable}")
         print(f"Confidence: {self.conf}")
         print(
             f"Null hyp.: the proportion of {self.level} in {self.variable} = {self.comparison_value}"
         )
 
@@ -1060,19 +1045,19 @@
         self.var = var
         self.level = level
         self.combinations = combinations
         self.alt_hypo = alt_hypo
         self.conf = conf
         self.multiple_comp_adjustment = multiple_comp_adjustment
 
-        self.p_val = None
+        # self.p_val = None
 
-        print("Pairwise proportion comparisons")
+        # print("Pairwise proportion comparisons")
 
-    def calculate(self) -> None:
+        # def calculate(self) -> None:
         combinations_elements = set()
         for combination in self.combinations:
             combinations_elements.add(combination[0])
             combinations_elements.add(combination[1])
         combinations_elements = list(combinations_elements)
 
         rows1 = []
@@ -1084,15 +1069,15 @@
             ns = len(subset)
             n_missing = subset.isna().sum()
             n = (
                 len(self.data[(self.data[self.grouping_var] == element)][self.var])
                 - n_missing
             )
             p = ns / n
-            print(f"ns: {ns}, n: {n}, p: {p}, nmissing: {n_missing}")
+            # print(f"ns: {ns}, n: {n}, p: {p}, nmissing: {n_missing}")
             sd = sqrt(p * (1 - p))
             se = sd / sqrt(n)
             z_score = stats.norm.ppf((1 + self.conf) / 2)
             # was printing out imaginary part in som cases
             me = np.real(z_score * sd / sqrt(n))
             row = [element, ns, p, n, n_missing, sd, se, me]
             rows1.append(row)
@@ -1146,15 +1131,23 @@
                 len(self.data[self.data[self.grouping_var] == v2][self.var])
                 - n_missing2
             )
             p2 = ns2 / n2
 
             diff = p1 - p2
 
-            chisq, self.p_val, df, _ = stats.chi2_contingency()  # unsure about this
+            observed = pd.crosstab(
+                self.data[v1], columns=self.data[v2], margins=True, margins_name="Total"
+            )
+            chisq, self.p_val, df, _ = stats.chi2_contingency(
+                self.observed.drop(columns="Total").drop("Total", axis=0),
+                correction=False,
+            )
+            # chisq, self.p_val, df, _ = stats.chi2_contingency()  # unsure about this
+
             # print(f"chisq: {chisq}")
 
             row = [
                 null_hypo,
                 alt_hypo,
                 diff,
                 self.p_val,
@@ -1176,29 +1169,23 @@
                 "df",
                 # "0%",
                 # str(self.conf * 100) + "%",
             ],
         )
 
     def summary(self, dec: int = 3) -> None:
-        if self.p_val == None:
-            self.calculate()
-        data_name = ""
         if hasattr(self.data, "description"):
             data_name = self.data.description.split("\n")[0].split()[1].lower()
-        if len(data_name) > 0:
-            print(f"Data: {data_name}")
-
+        else:
+            data_name = "Not available"
+        print(f"Data: {data_name}")
         print(f"Variables: {self.grouping_var}, {self.var}")
         print(f"Level: {self.level} in {self.var}")
         print(f"Confidence: {self.conf}")
-        print(f"Adjustment: {self.multiple_comp_adjustment}")
-
-        print()
-
+        print(f"Adjustment: {self.multiple_comp_adjustment}\n")
         print(self.table1.round(dec).to_string(index=False))
         print(self.table2.round(dec).to_string(index=False))
 
 
 class central_limit_theorem:
     def __init__(
         self,
@@ -1400,19 +1387,20 @@
                     for column in self._expected_df.columns.tolist()[:-1]
                 },
                 columns=self._expected_df.columns.tolist()[:-1],
             )
 
     def summary(self) -> None:
         print("Goodness of fit test")
-        data_name = ""
         if hasattr(self.data, "description"):
             data_name = self.data.description.split("\n")[0].split()[1].lower()
-        print(f"Data: {data_name}")
+        else:
+            data_name = "Not available"
 
+        print(f"Data: {data_name}")
         if self.variable not in self.data.columns:
             print(f"{self.variable} does not exist in chosen dataset")
             return
 
         print(f"Variable: {self.variable}")
         num_levels = self.data[self.variable].nunique()
         if self.probabilities is None:
```

### Comparing `pyrsm-0.7.9.1/pyrsm/bins.py` & `pyrsm-0.7.9.2/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/basics/consider.pkl` & `pyrsm-0.7.9.2/pyrsm/data/basics/consider.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/basics/demand_uk.pkl` & `pyrsm-0.7.9.2/pyrsm/data/basics/demand_uk.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/basics/newspaper.pkl` & `pyrsm-0.7.9.2/pyrsm/data/basics/newspaper.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/basics/salary.pkl` & `pyrsm-0.7.9.2/pyrsm/data/basics/salary.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/data/avengers.pkl` & `pyrsm-0.7.9.2/pyrsm/data/data/avengers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/data/diamonds.pkl` & `pyrsm-0.7.9.2/pyrsm/data/data/diamonds.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/data/publishers.pkl` & `pyrsm-0.7.9.2/pyrsm/data/data/publishers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/data/superheroes.pkl` & `pyrsm-0.7.9.2/pyrsm/data/data/superheroes.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/data/titanic.pkl` & `pyrsm-0.7.9.2/pyrsm/data/data/titanic.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/design/rndnames.pkl` & `pyrsm-0.7.9.2/pyrsm/data/design/rndnames.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/catalog.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/catalog.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/direct_marketing.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/direct_marketing.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/dvd.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/dvd.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/houseprices.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/houseprices.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/ideal.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/ideal.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/ketchup.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/ketchup.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/model/ratings.pkl` & `pyrsm-0.7.9.2/pyrsm/data/model/ratings.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/carpet.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/carpet.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/city.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/city.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/city2.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/city2.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/computer.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/computer.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/movie.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/movie.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/mp3.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/mp3.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/retailers.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/retailers.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/shopping.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/shopping.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/toothpaste.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/toothpaste.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/data/multivariate/tpbrands.pkl` & `pyrsm-0.7.9.2/pyrsm/data/multivariate/tpbrands.pkl`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/example_data.py` & `pyrsm-0.7.9.2/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/logit.py` & `pyrsm-0.7.9.2/pyrsm/logit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,65 @@
+from typing import Union, Optional
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import statsmodels as sm
+from statsmodels.genmod.families import Binomial
+from statsmodels.genmod.families.links import logit
 import statsmodels.formula.api as smf
 from statsmodels.stats.outliers_influence import variance_inflation_factor
 from scipy import stats
 from scipy.special import expit
 from .utils import ifelse
 from .stats import weighted_mean, weighted_sd
 from .perf import auc
-from .regression import sig_stars, model_fit_reg
+from .regression import sig_stars
+
+# from statsmodels.regression.linear_model import RegressionResults as rrs
+from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
+
+
+def get_mfit(fitted) -> tuple[Optional[dict], Optional[str]]:
+    mfit_dct = None
+    model_type = None
+    if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
+        fw = None
+        if fitted.model._has_freq_weights:
+            fw = fitted.model.freq_weights
+
+        mfit_dct = {
+            "pseudo_rsq_mcf": [1 - fitted.llf / fitted.llnull],
+            "pseudo_rsq_mcf_adj": [1 - (fitted.llf - fitted.df_model) / fitted.llnull],
+            "AUC": [auc(fitted.model.endog, fitted.fittedvalues, weights=fw)],
+            "log_likelihood": fitted.llf,
+            "AIC": [fitted.aic],
+            "BIC": [fitted.bic_llf],
+            "chisq": [fitted.pearson_chi2],
+            "chisq_df": [fitted.df_model],
+            "chisq_pval": [1 - stats.chi2.cdf(fitted.pearson_chi2, fitted.df_model)],
+            "nobs": [fitted.nobs],
+        }
+
+        model_type = "logistic"
+
+    elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
+        mfit_dct = {
+            "rsq": [fitted.rsquared],
+            "rsq_adj": [fitted.rsquared_adj],
+            "fvalue": [fitted.fvalue],
+            "ftest_df_model": [fitted.df_model],
+            "ftest_df_resid": [fitted.df_resid],
+            "ftest_pval": [fitted.f_pvalue],
+            "nobs": [fitted.nobs],
+        }
+
+        model_type = "regression"
+
+    return mfit_dct, model_type
 
 
 def or_ci(fitted, alpha=0.05, intercept=False, importance=False, data=None, dec=3):
     """
     Confidence interval for Odds ratios
 
     Parameters
@@ -245,88 +290,181 @@
             "prediction": prediction,
             f"{low*100}%": expit(Xb - me),
             f"{high*100}%": expit(Xb + me),
         }
     )
 
 
-def model_fit_lr(fitted, dec: int = 3, prn: bool = True):
+def model_fit(fitted, dec: int = 3, prn: bool = True) -> Union[str, pd.DataFrame]:
     """
-    Compute various model fit statistics for a fitted logistic regression model
+    Compute various model fit statistics for a fitted linear or logistic regression model
 
     Parameters
     ----------
-    fitted : statmodels glm object
-        Logistic regression model fitted using statsmodels
+    fitted : statmodels ols or glm object
+        Regression model fitted using statsmodels
     dec : int
         Number of decimal places to use in rounding
     prn : bool
         If True, print output, else return a Pandas dataframe with the results
 
     Returns
     -------
         If prn is True, print output, else return a Pandas dataframe with the results
     """
-
     if hasattr(fitted, "df_resid"):
         weighted_nobs = (
             fitted.df_resid + fitted.df_model + int(hasattr(fitted.params, "Intercept"))
         )
         if weighted_nobs > fitted.nobs:
             fitted.nobs = weighted_nobs
+    mfit_dct, model_type = get_mfit(fitted)
+    if not mfit_dct:
+        return "Only linear and logistic regression models are currently supported."
 
-    if fitted.model._has_freq_weights:
-        fw = fitted.model.freq_weights
-    else:
-        fw = None
-
-    mfit = pd.DataFrame().assign(
-        pseudo_rsq_mcf=[1 - fitted.llf / fitted.llnull],
-        pseudo_rsq_mcf_adj=[1 - (fitted.llf - fitted.df_model) / fitted.llnull],
-        AUC=[auc(fitted.model.endog, fitted.fittedvalues, weights=fw)],
-        log_likelihood=fitted.llf,
-        BIC=[fitted.bic_llf],
-        AIC=[fitted.aic],
-        chisq=[fitted.pearson_chi2],
-        chisq_df=[fitted.df_model],
-        chisq_pval=[1 - stats.chi2.cdf(fitted.pearson_chi2, fitted.df_model)],
-        nobs=[fitted.nobs],
-    )
+    mfit = pd.DataFrame(mfit_dct)
 
-    output = f"""
-Pseudo R-squared (McFadden): {mfit.pseudo_rsq_mcf.values[0].round(dec)}
+    if prn:
+        output = "Model type not supported"
+        if model_type == "logistic":
+            output = f"""Pseudo R-squared (McFadden): {mfit.pseudo_rsq_mcf.values[0].round(dec)}
 Pseudo R-squared (McFadden adjusted): {mfit.pseudo_rsq_mcf_adj.values[0].round(dec)}
 Area under the RO Curve (AUC): {mfit.AUC.values[0].round(dec)}
 Log-likelihood: {mfit.log_likelihood.values[0].round(dec)}, AIC: {mfit.AIC.values[0].round(dec)}, BIC: {mfit.BIC.values[0].round(dec)}
-Chi-squared: {mfit.chisq.values[0].round(dec)} df({mfit.chisq_df.values[0]}), p.value {np.where(mfit.chisq_pval.values[0] < .001, "< 0.001", mfit.chisq_pval.values[0].round(dec))} 
-Nr obs: {mfit.nobs.values[0]:,.0f}
-"""
-
-    if prn:
-        print(output)
+Chi-squared: {mfit.chisq.values[0].round(dec)}, df({mfit.chisq_df.values[0]}), p.value {np.where(mfit.chisq_pval.values[0] < .001, "< 0.001", mfit.chisq_pval.values[0].round(dec))} 
+Nr obs: {mfit.nobs.values[0]:,.0f}"""
+        elif model_type == "regression":
+            output = f"""R-squared: {mfit.rsq.values[0].round(dec)}, Adjusted R-squared: {mfit.rsq_adj.values[0].round(dec)}
+F-statistic: {mfit.fvalue[0].round(dec)} df({mfit.ftest_df_model.values[0]:.0f}, {mfit.ftest_df_resid.values[0]:.0f}), p.value {np.where(mfit.ftest_pval.values[0] < .001, "< 0.001", mfit.ftest_pval.values[0].round(dec))}
+Nr obs: {mfit.nobs.values[0]:,.0f}"""
+        return output
     else:
         return mfit
 
 
-def model_fit(fitted, dec: int = 3, prn: bool = True):
-    """
-    Compute various model fit statistics for a fitted linear or logistic regression model
+class logistic:
+    def __init__(
+        self,
+        dataset: pd.DataFrame,
+        rvar: Optional[str] = None,
+        lev: Optional[str] = None,
+        evar: Optional[list[str]] = None,
+        form: Optional[str] = None,
+    ) -> None:
+        """
+        Initialize logistic regression model
+
+        Parameters
+        ----------
+        dataset: pandas DataFrame; dataset
+        evar: List of strings; contains the names of the columns of data to be used as explanatory variables
+        rvar: String; name of the column to be used as the response variable
+        lev: String; name of the level in the response variable
+        ssq: Boolean; whether sum of squared errors need to be reported
+        form: String; formula for the regression equation to use if evar and rvar are not provided
+        """
+        self.dataset = dataset
+        self.rvar = rvar
+        self.lev = lev
+        self.evar = evar
+        self.form = form
+
+        if self.form:
+            self.fitted = smf.glm(
+                formula=self.form, data=self.dataset, family=Binomial(link=logit())
+            ).fit()
+            self.evar = extract_evars(self.fitted.model, self.dataset.columns)
+            self.rvar = extract_rvar(self.fitted.model, self.dataset.columns)
+            self.lev = self.dataset.at[0, self.rvar]
+        else:
+            self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
+            self.fitted = smf.glm(
+                formula=self.form, data=self.dataset, family=Binomial(link=logit())
+            ).fit()
+
+        df = pd.DataFrame(np.exp(self.fitted.params), columns=["OR"]).dropna()
+        df["OR%"] = 100 * ifelse(df["OR"] < 1, -(1 - df["OR"]), df["OR"] - 1)
+        df["coefficient"] = self.fitted.params
+        df["std.error"] = self.fitted.params / self.fitted.tvalues
+        # wierd but this is what statsmodels uses in summary
+        df["z.value"] = self.fitted.tvalues
+        df["p.value"] = self.fitted.pvalues
+        df["  "] = sig_stars(self.fitted.pvalues)
+        self.coef = df.reset_index()
+
+    def summary(self, dec=3) -> None:
+        """
+        Summarize output from a logistic regression model
+        """
 
-    Parameters
-    ----------
-    fitted : statmodels ols or glm object
-        Regression model fitted using statsmodels
-    dec : int
-        Number of decimal places to use in rounding
-    prn : bool
-        If True, print output, else return a Pandas dataframe with the results
+        if hasattr(self.dataset, "description"):
+            data_name = self.dataset.description.split("\n")[0].split()[1].lower()
+        else:
+            data_name = "Not available"
 
-    Returns
-    -------
-        If prn is True, print output, else return a Pandas dataframe with the results
-    """
-    if isinstance(fitted, sm.genmod.generalized_linear_model.GLMResultsWrapper):
-        model_fit_lr(fitted, dec=dec, prn=prn)
-    elif isinstance(fitted, sm.regression.linear_model.RegressionResultsWrapper):
-        model_fit_reg(fitted, dec=dec, prn=prn)
-    else:
-        return "Only linear and logistic regression models are currently supported."
+        print("Logistic regression (GLM)")
+        print(f"Data                 : {data_name}")
+        print(f"Response variable    : {self.rvar}")
+        print(f"Level                : {self.lev}")
+        print(f"Explanatory variables: {', '.join(self.evar)}")
+        print(f"Null hyp.: there is no effect x on {self.rvar}")
+        print(f"Alt. hyp.: there is an effect of x on {self.rvar}")
+
+        self.coef["OR"] = self.coef["OR"].round(dec)
+        self.coef["coefficient"] = self.coef["coefficient"].round(2)
+        self.coef["std.error"] = self.coef["std.error"].round(dec)
+        self.coef["z.value"] = self.coef["z.value"].round(dec)
+        self.coef["p.value"] = ifelse(
+            self.coef["p.value"] < 0.001, "< .001", self.coef["p.value"].round(dec)
+        )
+        self.coef["OR%"] = [f"{round(o, max(dec-2, 0))}%" for o in self.coef["OR%"]]
+        print(f"\n{self.coef.to_string(index=False)}")
+        print("\nSignif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1")
+        print(f"\n{model_fit(self.fitted)}")
+
+    def ci(self, alpha=0.05, intercept=False, dec=3) -> None:
+        """
+        Confidence intervals for Odds Ratios
+        """
+        print(
+            f"\n{or_ci(self.fitted, alpha=alpha, intercept=intercept).to_string(index=False)}"
+        )
+
+    def plot(
+        self,
+        plots="or",
+        alpha=0.05,
+        intercept=False,
+        incl=None,
+        excl=None,
+        incl_int=[],
+        fix=True,
+        hline=False,
+        figsize=None,
+    ) -> None:
+        """
+        Plots for a logistic regression model
+        """
+        if "or" in plots:
+            or_plot(
+                self.fitted,
+                alpha=alpha,
+                intercept=intercept,
+                incl=incl,
+                excl=excl,
+                figsize=figsize,
+            )
+        if "pred" in plots:
+            pred_plot_sm(
+                self.fitted,
+                self.dataset,
+                incl=incl,
+                excl=[],
+                incl_int=incl_int,
+                fix=fix,
+                hline=hline,
+                nnv=20,
+                minq=0.025,
+                maxq=0.975,
+            )
+        if "vimp" in plots:
+            vimp_plot_sm(self.fitted, self.dataset, rep=10, ax=None, ret=False)
```

### Comparing `pyrsm-0.7.9.1/pyrsm/notebook.py` & `pyrsm-0.7.9.2/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/perf.py` & `pyrsm-0.7.9.2/pyrsm/perf.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
     tlev,
     cost=1,
     margin=2,
     scale=1,
     qnt=10,
 ):
     """
-    Plot an Incremental Profit chart for Uplift modeling
+    Tabulate Incremental Profit for Uplift modeling
 
     Parameters
     ----------
     df : Pandas dataframe or a dictionary of dataframes with keys to show multiple curves for different models or data samples
     rvar : str
         Name of the response variable column in df
     lev : str
@@ -433,15 +433,15 @@
     marker : str
         Marker to use for line plot
     **kwargs : Named arguments to be passed to the seaborn lineplot function
 
     Returns
     -------
     Seaborn object
-        Plot of Incremental Uplift per quantile
+        Plot of Incremental Profit per quantile
     """
 
     dct = ifelse(isinstance(df, dict), df, {"": df})
     pred = ifelse(isinstance(pred, str), [pred], pred)
     group = ifelse(len(pred) > 1 or len(dct.keys()) > 1, "pred", None)
 
     rd = inc_profit_tab(df, rvar, lev, pred, tvar, tlev, cost, margin, scale, qnt)
@@ -1132,15 +1132,15 @@
             total=[total],
             TPR=[TPR],
             TNR=[TNR],
             precision=[precision],
             Fscore=[2 * (precision * TPR) / (precision + TPR)],
             accuracy=[(TP + TN) / total],
             kappa=[metrics.cohen_kappa_score(pos, gtbe)],
-            profit=[profit],
+            profit=[profit * scale],
             index=[0],
             ROME=[profit / (cost * (TP + FP))],
             contact=[contact],
             AUC=[metrics.auc(fpr, tpr)],
         )
 
     result = pd.DataFrame()
```

### Comparing `pyrsm-0.7.9.1/pyrsm/props.py` & `pyrsm-0.7.9.2/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/pyrsm/regression.py` & `pyrsm-0.7.9.2/pyrsm/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,61 +119,14 @@
 
     if intercept is False:
         df = df.loc[df["index"] != "Intercept"]
 
     return df
 
 
-def model_fit_reg(fitted, dec: int = 3, prn: bool = True):
-    """
-    Compute various model fit statistics for a fitted linear regression model
-
-    Parameters
-    ----------
-    fitted : statmodels ols object
-        Linear regression (OLS) model fitted using statsmodels
-    dec : int
-        Number of decimal places to use in rounding
-    prn : bool
-        If True, print output, else return a Pandas dataframe with the results
-
-    Returns
-    -------
-        If prn is True, print output, else return a Pandas dataframe with the results
-    """
-
-    if hasattr(fitted, "df_resid"):
-        weighted_nobs = (
-            fitted.df_resid + fitted.df_model + int(hasattr(fitted.params, "Intercept"))
-        )
-        if weighted_nobs > fitted.nobs:
-            fitted.nobs = weighted_nobs
-
-        mfit = pd.DataFrame().assign(
-            rsq=[fitted.rsquared],
-            rsq_adj=[fitted.rsquared_adj],
-            fvalue=[fitted.fvalue],
-            ftest_df_model=[fitted.df_model],
-            ftest_df_resid=[fitted.df_resid],
-            ftest_pval=[fitted.f_pvalue],
-            nobs=[fitted.nobs],
-        )
-
-        output = f"""
-    R-squared: {mfit.rsq.values[0].round(dec)}, Adjusted R-squared: {mfit.rsq_adj.values[0].round(dec)}
-    F-statistic: {mfit.fvalue[0].round(dec)} df({mfit.ftest_df_model.values[0]:.0f}, {mfit.ftest_df_resid.values[0]:.0f}), p.value {np.where(mfit.ftest_pval.values[0] < .001, "< 0.001", mfit.ftest_pval.values[0].round(dec))}
-    Nr obs: {mfit.nobs.values[0]:,.0f}
-    """
-
-    if prn:
-        print(output)
-    else:
-        return mfit
-
-
 def evalreg(df, rvar: str, pred: str, dec: int = 3):
     """
     Evaluate regression models. Calculates R-squared, MSE, and MAE
 
     Parameters
     ----------
     df : Pandas DataFrame or a dictionary of DataFrames with keys to show results for
@@ -353,17 +306,18 @@
         rvar = model.endog_names
     else:
         form = f"{rvar} ~ {' + '.join(evars)}"
         model = smf.ols(form, data=dataset)
 
     res = model.fit()
 
-    data_name = ""
     if hasattr(dataset, "description"):
         data_name = dataset.description.split("\n")[0].split()[1].lower()
+    else:
+        data_name = "Not available"
 
     print("Data: ", data_name)
     print("Response variable    :", rvar)
     print("Explanatory variables:", ", ".join(evars))
     print(f"Null hyp.: the effect of x on {rvar} is zero")
     print(f"Alt. hyp.: the effect of x on {rvar} is not zero")
     summary = res.summary()
```

### Comparing `pyrsm-0.7.9.1/pyrsm/stats.py` & `pyrsm-0.7.9.2/pyrsm/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 
     if excl is not None:
         isNum = setdiff(isNum, excl)
     dfs = df[isNum]
     if train is None:
         train = np.array([True] * df.shape[0])
     if wt is None:
-        df[isNum] = (dfs - dfs[train].mean().values) / (
+        df.loc[:, isNum] = (dfs - dfs[train].mean().values) / (
             sf * dfs[train].std(ddof=ddof).values
         )
     else:
         wt = np.array(wt)
-        df[isNum] = (dfs - weighted_mean(dfs[train], wt[train])) / (
+        df.loc[:, isNum] = (dfs - weighted_mean(dfs[train], wt[train])) / (
             sf * weighted_sd(dfs[train], wt[train], ddof=ddof)
         )
     return df
```

### Comparing `pyrsm-0.7.9.1/pyrsm/utils.py` & `pyrsm-0.7.9.2/pyrsm/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 import pandas as pd
+from scipy import stats
 import inspect as ins
 from itertools import product
 from datetime import date, datetime
 from math import ceil
 from IPython.display import display, Markdown
 from sys import modules
 import json
 
-from math import log
-
 
 def add_description(df, md="", path=""):
     """
     Add a description to a Pandas dataframe in markdown format
 
     Parameters
     ----------
@@ -196,37 +195,39 @@
     df = pd.DataFrame({"var1": ["a", "b", "a"], "freq": [5, 2, 3]})
     table2data(df, "freq")
     """
 
     return df.loc[df.index.repeat(df[freq])]
 
 
-def setdiff(x, y):
+def setdiff(x, y, sort=False):
     """
     Returns a numpy array of unique elements in x that are not in y
 
     Parameters
     ----------
 
     x : List type or that can be converted to a list
     y : List type or that can be converted to a list
+    sort : boolean
+        Sort the output
 
     Returns
     -------
     list
         Elements in x that are not in y
 
     Examples
     --------
     setdiff(["a", "b", "c"], ["b", "x"])
     """
 
     x = np.unique(np.array(x))
     y = np.unique(np.array(y))
-    return list(np.setdiff1d(x, y, assume_unique=True))
+    return list(np.setdiff1d(x, y, assume_unique=sort))
 
 
 def union(x, y):
     """
     Return the unique, sorted array of values that are in either of the two input arrays
 
     Parameters
@@ -440,35 +441,7 @@
                 .rename(col)
             )
             series_list.append(categorical_grouped)
         else:
             series_list.append(df[col])
     categorical_grouped_df = pd.concat(series_list, axis=1)
     return categorical_grouped_df, True
-
-
-# class Transform:
-#     def __init__(
-#         self, data: pd.DataFrame, cols: list[str], transform_type: str
-#     ) -> None:
-#         self.transform_type = transform_type
-#         self.data = data
-#         self.cols = cols
-
-#     def transform(self) -> pd.DataFrame:
-#         if self.transform_type == "ln":
-#             return self.transform_log()
-#         elif self.transform_type == "log2":
-#             return self.transform_log(base=2)
-
-#     def transform_log(self, base: int = None) -> pd.DataFrame:
-#         new_cols = {
-#             col: col + "_ln" if col in self.cols else col for col in self.data.columns
-#         }
-#         for old_col in self.cols:
-#             if base != None:
-#                 self.data[old_col] = self.data[old_col].transform(log, base)
-#             else:
-#                 self.data[old_col] = self.data[old_col].transform(log)
-
-#         self.data.rename(new_cols, axis=1, inplace=True)
-#         return self.data
```

### Comparing `pyrsm-0.7.9.1/pyrsm/visualize.py` & `pyrsm-0.7.9.2/pyrsm/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,22 @@
     """
     pattern = r"\b\w+\b"
     evars = re.findall(pattern, model.formula)[1:]
     evars = [v for v in evars if v in cn]
     return [v for i, v in enumerate(evars) if v not in evars[:i]]
 
 
+def extract_rvar(model, cn):
+    """
+    Extract name of the response variable in a statsmodels model
+    """
+    pattern = r"\b\w+\b"
+    return re.findall(pattern, model.formula)[0]
+
+
 def pred_plot_sm(
     fitted,
     df,
     incl=None,
     excl=[],
     incl_int=[],
     fix=True,
@@ -169,20 +177,21 @@
             return (mmin, mmax)
         elif not isinstance(fix, bool) and len(fix) == 2:
             return fix
         else:
             return False
 
     rvar = model.endog_names
-    if isinstance(hline, bool) and hline == True:
-        hline = df[rvar].mean()
-
-    if not isinstance(hline, float) and not isinstance(hline, int):
-        hline = False
-        min_max = (np.Inf, -np.Inf)
+    if isinstance(hline, bool):
+        if hline:
+            hline = df[rvar].mean()
+            min_max = (hline - plot_margin * hline, hline + plot_margin * hline)
+        else:
+            hline = False
+            min_max = (np.Inf, -np.Inf)
     else:
         min_max = (hline - plot_margin * hline, hline + plot_margin * hline)
 
     if incl is None:
         incl = extract_evars(model, df.columns)
     else:
         incl = ifelse(isinstance(incl, str), [incl], incl)
@@ -338,15 +347,22 @@
     """
     # features names used in the sklearn model
     fn = fitted.feature_names_in_
 
     not_transformed = [c for c in df.columns for f in fn if c == f]
     if transformed is None:
         transformed = list(
-            set([c for c in df.columns for f in fn if f"{c}_" in f and c != f])
+            set(
+                [
+                    c
+                    for c in df.columns
+                    for f in fn
+                    if f"{c}_" in f and c != f and f"{c}_" not in df.columns
+                ]
+            )
         )
 
     ints = intersect(transformed, not_transformed)
     if len(ints) > 0:
         trn = '", "'.join(transformed)
         ints = ", ".join(ints)
         not_transformed = setdiff(not_transformed, transformed)
@@ -374,23 +390,24 @@
 
     def dummify(df, trs):
         if len(trs) > 0:
             return pd.concat([pd.get_dummies(df[trs]), df.drop(trs, axis=1)], axis=1)
         else:
             return df
 
-    if rvar is not None and isinstance(hline, bool) and hline == True:
-        hline = df[rvar].mean()
-
     # margin to add above and below in plots
     plot_margin = 0.025
 
-    if not isinstance(hline, float) and not isinstance(hline, int):
-        hline = False
-        min_max = (np.Inf, -np.Inf)
+    if isinstance(hline, bool):
+        if hline and rvar is not None:
+            hline = df[rvar].mean()
+            min_max = (hline - plot_margin * hline, hline + plot_margin * hline)
+        else:
+            hline = False
+            min_max = (np.Inf, -np.Inf)
     else:
         min_max = (hline - plot_margin * hline, hline + plot_margin * hline)
 
     def calc_ylim(lab, lst, min_max):
         if isinstance(fix, bool) and fix == True:
             vals = lst[lab]
             min_vals = min(vals)
@@ -535,20 +552,20 @@
         Add the plot to a the axis object from a matplotlib subplot
     ret: bool
         Return the variable importance table as a sorted DataFrame
     """
     fw = None
     if hasattr(fitted, "model"):
         model = fitted.model
-        if model._has_freq_weights:
+        if hasattr(model, "_has_freq_weights") and model._has_freq_weights:
             fw = model.freq_weights
     else:
         return "This function requires a fitted linear or logistic regression"
 
-    rvar = model.endog_names
+    rvar = extract_rvar(model, df.columns)
     evars = extract_evars(model, df.columns)
     df = df[[rvar] + evars].copy().reset_index(drop=True).dropna()
 
     if len(model.endog) != df.shape[0]:
         raise Exception(
             "The number of rows in the DataFrame should be the same as the number of rows in the data used to estimate the model"
         )
```

### Comparing `pyrsm-0.7.9.1/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.7.9.2/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.7.9.1
+Version: 0.7.9.2
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.7.9.1/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.7.9.2/pyrsm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.md
 pyproject.toml
 setup.cfg
 pyrsm/__init__.py
 pyrsm/basics.py
 pyrsm/bins.py
 pyrsm/example_data.py
-pyrsm/logistic_regression.py
 pyrsm/logit.py
 pyrsm/notebook.py
 pyrsm/perf.py
 pyrsm/props.py
 pyrsm/regression.py
 pyrsm/stats.py
 pyrsm/utils.py
```

### Comparing `pyrsm-0.7.9.1/setup.cfg` & `pyrsm-0.7.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_basics.py` & `pyrsm-0.7.9.2/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_bins.py` & `pyrsm-0.7.9.2/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_example_data.py` & `pyrsm-0.7.9.2/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_perf.py` & `pyrsm-0.7.9.2/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_regression.py` & `pyrsm-0.7.9.2/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_stats.py` & `pyrsm-0.7.9.2/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.7.9.1/tests/test_utils.py` & `pyrsm-0.7.9.2/tests/test_utils.py`

 * *Files identical despite different names*

