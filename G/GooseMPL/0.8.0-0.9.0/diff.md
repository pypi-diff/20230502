# Comparing `tmp/GooseMPL-0.8.0.tar.gz` & `tmp/GooseMPL-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GooseMPL-0.8.0.tar", last modified: Fri Dec 17 17:46:39 2021, max compression
+gzip compressed data, was "GooseMPL-0.9.0.tar", last modified: Sun Jan  2 15:50:02 2022, max compression
```

## Comparing `GooseMPL-0.8.0.tar` & `GooseMPL-0.9.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.488918 GooseMPL-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.480918 GooseMPL-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.480918 GooseMPL-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.480918 GooseMPL-0.8.0/GooseMPL/
--rw-r--r--   0 runner    (1001) docker     (121)    52964 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/GooseMPL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.484918 GooseMPL-0.8.0/GooseMPL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-17 17:46:39.000000 GooseMPL-0.8.0/GooseMPL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-12-17 17:46:39.488918 GooseMPL-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.484918 GooseMPL-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.480918 GooseMPL-0.8.0/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.484918 GooseMPL-0.8.0/docs/examples/goosempl/
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)   138022 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/histogram.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/histogram_powerlaw.py
--rw-r--r--   0 runner    (1001) docker     (121)   118637 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/histogram_powerlaw.svg
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/patch.py
--rw-r--r--   0 runner    (1001) docker     (121)    28913 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/patch.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/random_from_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    91586 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/random_from_cdf.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/goosempl/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.488918 GooseMPL-0.8.0/docs/examples/pyplot/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    20565 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colorbar.svg
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colormap-part.py
--rw-r--r--   0 runner    (1001) docker     (121)    84443 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colormap-part.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)    40278 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/colormap.svg
--rw-r--r--   0 runner    (1001) docker     (121)      553 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image.py
--rw-r--r--   0 runner    (1001) docker     (121)    35428 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image_subplots.py
--rw-r--r--   0 runner    (1001) docker     (121)    48393 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image_subplots.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image_subplots_bottom.py
--rw-r--r--   0 runner    (1001) docker     (121)    43505 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/image_subplots_bottom.svg
--rw-r--r--   0 runner    (1001) docker     (121)      322 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/legend_background.py
--rw-r--r--   0 runner    (1001) docker     (121)    31890 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/legend_background.svg
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/legend_external.py
--rw-r--r--   0 runner    (1001) docker     (121)    26796 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/legend_external.svg
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/multicolor.py
--rw-r--r--   0 runner    (1001) docker     (121)    27036 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/multicolor.svg
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot-cmap.py
--rw-r--r--   0 runner    (1001) docker     (121)    83668 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot-cmap.svg
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot-cycler.py
--rw-r--r--   0 runner    (1001) docker     (121)    71400 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot-cycler.svg
--rw-r--r--   0 runner    (1001) docker     (121)      557 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    31917 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/plot.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7730 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/subplot.py
--rw-r--r--   0 runner    (1001) docker     (121)    49656 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/subplot.svg
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)    21032 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-formatter.svg
--rw-r--r--   0 runner    (1001) docker     (121)      523 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log.py
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log.svg
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log_1.py
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log_1.svg
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log_2.py
--rw-r--r--   0 runner    (1001) docker     (121)    19898 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-log_2.svg
--rw-r--r--   0 runner    (1001) docker     (121)      448 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-position.py
--rw-r--r--   0 runner    (1001) docker     (121)    35621 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-position.svg
--rw-r--r--   0 runner    (1001) docker     (121)      559 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-rotation-log.py
--rw-r--r--   0 runner    (1001) docker     (121)    27997 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/examples/pyplot/tick-rotation-log.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/goosempl.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/style.rst
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/docs/tips.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-17 17:46:39.488918 GooseMPL-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      595 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-17 17:46:39.488918 GooseMPL-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     5389 2021-12-17 17:46:28.000000 GooseMPL-0.8.0/test/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.913969 GooseMPL-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.901968 GooseMPL-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/GooseMPL/
+-rw-r--r--   0 runner    (1001) docker     (121)    55455 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/GooseMPL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/GooseMPL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-02 15:50:02.000000 GooseMPL-0.9.0/GooseMPL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2022-01-02 15:50:02.913969 GooseMPL-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.905968 GooseMPL-0.9.0/docs/examples/goosempl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)   138022 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/histogram.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/histogram_powerlaw.py
+-rw-r--r--   0 runner    (1001) docker     (121)   118637 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/histogram_powerlaw.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/patch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28913 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/patch.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/random_from_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    91586 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/random_from_cdf.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/goosempl/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.909968 GooseMPL-0.9.0/docs/examples/pyplot/
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20565 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colorbar.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colormap-part.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84443 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colormap-part.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40278 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/colormap.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35428 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image_subplots.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48393 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image_subplots.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image_subplots_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43505 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/image_subplots_bottom.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/legend_background.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31890 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/legend_background.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/legend_external.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26796 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/legend_external.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/multicolor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27036 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/multicolor.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot-cmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)    83668 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot-cmap.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot-cycler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71400 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot-cycler.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31917 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/plot.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7730 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/subplot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49656 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/subplot.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21032 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-formatter.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log_1.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19898 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-log_2.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-position.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35621 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-position.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-rotation-log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27997 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/examples/pyplot/tick-rotation-log.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/goosempl.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/style.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/docs/tips.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-02 15:50:02.913969 GooseMPL-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 15:50:02.909968 GooseMPL-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     6975 2022-01-02 15:49:53.000000 GooseMPL-0.9.0/test/main.py
```

### Comparing `GooseMPL-0.8.0/.github/workflows/ci.yml` & `GooseMPL-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/.github/workflows/pre-commit.yml` & `GooseMPL-0.9.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/.github/workflows/pythonpublish.yml` & `GooseMPL-0.9.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/.gitignore` & `GooseMPL-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/.pre-commit-config.yaml` & `GooseMPL-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/GooseMPL/__init__.py` & `GooseMPL-0.9.0/GooseMPL/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1193,15 +1193,15 @@
     # remove access in labels
     plt.setp(lines[1:], label="_")
 
     # return handles
     return lines
 
 
-def _fit_powerlaw(
+def _fit_loglog(
     logx: ArrayLike,
     logy: ArrayLike,
     prefactor: float,
     exponent: float,
     **fit_opts,
 ) -> (float, float):
 
@@ -1254,25 +1254,28 @@
     Warning: If this function is used to plot the fit, beware that the fit is plotted using just
     two data-points if the axis is set to log-log scale
     (as the fit will be a straight line on that scale).
 
     :param xdata: Data points along the x-axis.
     :param ydata: Data points along the y-axis.
     :param yerr: Error-bar for ``ydata``.
-    :param prefactor: Prefactor (fitted if not specified).
-    :param exponent: Exponent (fitted if not specified).
+    :param prefactor: Prefactor :math:`c` (fitted if not specified).
+    :param exponent: Exponent :math:`b` (fitted if not specified).
     :param axis: Axis to plot along (not plotted if not specified).
     :param fmt: Format for the label (if plotting). E.g. ``r"${0:.3f} x^{{{1:.2f}}}$"``.
     :param kwargs: Other plot options.
 
     :return:
         ``prefactor, exponent[, h]``
         The (fitted) prefector and exponent, and optionally the handle (if plotting)
     """
 
+    xdata = np.array(xdata)
+    ydata = np.array(ydata)
+
     i = np.logical_and(xdata > 0, ydata > 0)
     logx = np.log(xdata[i])
     logy = np.log(ydata[i])
 
     j = np.logical_or(np.isnan(logx), np.isnan(logy))
     logx = logx[~j]
     logy = logy[~j]
@@ -1281,15 +1284,15 @@
 
     if yerr is not None:
         logyerr = np.log(yerr[i])
         logyerr = logyerr[~j]
         fit_opts["sigma"] = logyerr
         fit_opts["absolute_sigma"] = True
 
-    prefactor, exponent = _fit_powerlaw(logx, logy, prefactor, exponent, **fit_opts)
+    prefactor, exponent = _fit_loglog(logx, logy, prefactor, exponent, **fit_opts)
 
     if axis is None:
         return (prefactor, exponent)
 
     xp = np.array([np.min(np.exp(logx)), np.max(np.exp(logx))])
 
     if axis.get_xscale() != "log" or axis.get_yscale() != "log":
@@ -1325,25 +1328,28 @@
     Warning: If this function is used to plot the fit, beware that the fit is plotted using just
     two data-points if the axis is set to semilogy-scale
     (as the fit will be a straight line on that scale).
 
     :param xdata: Data points along the x-axis.
     :param ydata: Data points along the y-axis.
     :param yerr: Error-bar for ``ydata``.
-    :param prefactor: Prefactor (fitted if not specified).
-    :param exponent: Exponent (fitted if not specified).
+    :param prefactor: Prefactor :math:`c` (fitted if not specified).
+    :param exponent: Exponent :math:`b` (fitted if not specified).
     :param axis: Axis to plot along (not plotted if not specified).
     :param fmt: Format for the label (if plotting). E.g. ``r"${0:.3f} \exp ({1:.2f} x)$"``.
     :param kwargs: Other plot options.
 
     :return:
         ``prefactor, exponent[, h]``
         The (fitted) prefector and exponent, and optionally the handle (if plotting)
     """
 
+    xdata = np.array(xdata)
+    ydata = np.array(ydata)
+
     i = ydata > 0
     x = xdata[i]
     logy = np.log(ydata[i])
 
     j = np.isnan(logy)
     logy = logy[~j]
     x = x[~j]
@@ -1352,15 +1358,15 @@
 
     if yerr is not None:
         logyerr = np.log(yerr[i])
         logyerr = logyerr[~j]
         fit_opts["sigma"] = logyerr
         fit_opts["absolute_sigma"] = True
 
-    prefactor, exponent = _fit_powerlaw(x, logy, prefactor, exponent, **fit_opts)
+    prefactor, exponent = _fit_loglog(x, logy, prefactor, exponent, **fit_opts)
 
     if axis is None:
         return (prefactor, exponent)
 
     xp = np.array([np.min(x), np.max(x)])
 
     if axis.get_yscale() != "log":
@@ -1373,14 +1379,90 @@
         kwargs["label"] = fmt.format(prefactor, exponent)
 
     h = axis.plot(xp, yp, **kwargs)
 
     return (prefactor, exponent, h)
 
 
+def fit_linear(
+    xdata: ArrayLike,
+    ydata: ArrayLike,
+    yerr: ArrayLike = None,
+    offset: float = None,
+    slope: float = None,
+    axis: plt.Axes = None,
+    fmt: str = None,
+    **kwargs,
+):
+    r"""
+    Fit a linear function :math:`y = a + b x`.
+
+    :param xdata: Data points along the x-axis.
+    :param ydata: Data points along the y-axis.
+    :param yerr: Error-bar for ``ydata``.
+    :param offset: Offset :math:`a` (fitted if not specified).
+    :param slope: Slope :math:`b` (fitted if not specified).
+    :param axis: Axis to plot along (not plotted if not specified).
+    :param fmt: Format for the label (if plotting). E.g. ``r"${0:.3f} + {1:.2f} x$"``.
+    :param kwargs: Other plot options.
+
+    :return:
+        ``offset, slope[, h]``
+        The (fitted) offset and slope, and optionally the handle (if plotting)
+    """
+
+    xdata = np.array(xdata)
+    ydata = np.array(ydata)
+
+    fit_opts = {}
+
+    if yerr is not None:
+        fit_opts["sigma"] = np.array(yerr)
+        fit_opts["absolute_sigma"] = True
+
+    if offset is None and slope is None:
+
+        def f(x, offset, slope):
+            return offset + slope * x
+
+        param, _ = curve_fit(f, xdata, ydata, **fit_opts)
+        offset = param[0]
+        slope = param[1]
+
+    elif offset is None:
+
+        def f(x, offset):
+            return offset + slope * x
+
+        param, _ = curve_fit(f, xdata, ydata, **fit_opts)
+        offset = param[0]
+
+    elif slope is None:
+
+        def f(x, slope):
+            return offset + slope * x
+
+        param, _ = curve_fit(f, xdata, ydata, **fit_opts)
+        slope = param[0]
+
+    if axis is None:
+        return (offset, slope)
+
+    xp = np.array([np.min(xdata), np.max(xdata)])
+    yp = offset + slope * xp
+
+    if fmt:
+        assert "label" not in kwargs
+        kwargs["label"] = fmt.format(offset, slope)
+
+    h = axis.plot(xp, yp, **kwargs)
+
+    return (offset, slope, h)
+
+
 def random_from_cdf(shape, P, x, linspace=False, shuffle=True):
     r"""
     Generate a random number based on a discrete cumulative probability density function.
 
     :arguments:
 
         **shape** (```<array_like>``)
@@ -1635,37 +1717,53 @@
         bin_edges = histogram_bin_edges_integer(bin_edges)
 
     # return
 
     return bin_edges
 
 
+def histogram_norm(count: ArrayLike, bin_edges: ArrayLike, norm: float = 1.0):
+    """
+    Renormalise a histogram.
+
+    :param count: Count.
+    :param bin_edges: Bin-edges.
+    :param norm: Area of the histogram.
+    """
+    assert len(bin_edges) == len(count) + 1
+    return count * norm / np.sum(np.diff(bin_edges) * count)
+
+
+def histogram_bin_edges2midpoint(bin_edges: ArrayLike):
+    """
+    Return the midpoints of every bin-edge.
+
+    :param bin_edges: Bin-edges.
+    :param count: Count per bin.
+    :param norm: Area of the histogram.
+    """
+    return 0.5 * np.diff(bin_edges) + bin_edges[:-1]
+
+
 def histogram(data, return_edges=True, **kwargs):
     r"""
     Compute histogram.
-    See `numpy.histrogram <https://docs.scipy.org/doc/numpy/reference/generated/numpy.histogram.html>`__
-
-    :extra options:
+    This function passes all options to
+    `numpy.histrogram <https://docs.scipy.org/doc/numpy/reference/generated/numpy.histogram.html>`__
+    In addition you can use:
 
-        **return_edges** ([``True``] | [``False``])
-            Return the bin edges if set to ``True``, return their midpoints otherwise.
+    :param return_edges: Return the bin edges if set to ``True``, return their midpoints otherwise.
     """
 
-    # use NumPy's default function to compute the histogram
     P, bin_edges = np.histogram(data, **kwargs)
 
-    # return default output
     if return_edges:
         return P, bin_edges
 
-    # convert bin_edges -> mid-points of each bin
-    x = np.diff(bin_edges) / 2.0 + bin_edges[:-1]
-
-    # return with bin mid-points
-    return P, x
+    return P, histogram_bin_edges2midpoint(bin_edges)
 
 
 def histogram_cumulative(data, **kwargs):
     r"""
     Compute cumulative histogram.
     See `numpy.histrogram <https://docs.scipy.org/doc/numpy/reference/generated/numpy.histogram.html>`__
```

### Comparing `GooseMPL-0.8.0/GooseMPL.egg-info/SOURCES.txt` & `GooseMPL-0.9.0/GooseMPL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/LICENSE` & `GooseMPL-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/README.md` & `GooseMPL-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/Makefile` & `GooseMPL-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/conf.py` & `GooseMPL-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/histogram.py` & `GooseMPL-0.9.0/docs/examples/goosempl/histogram.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/histogram.svg` & `GooseMPL-0.9.0/docs/examples/goosempl/histogram.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/histogram_powerlaw.py` & `GooseMPL-0.9.0/docs/examples/goosempl/histogram_powerlaw.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/histogram_powerlaw.svg` & `GooseMPL-0.9.0/docs/examples/goosempl/histogram_powerlaw.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/patch.py` & `GooseMPL-0.9.0/docs/examples/goosempl/patch.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/patch.svg` & `GooseMPL-0.9.0/docs/examples/goosempl/patch.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/random_from_cdf.py` & `GooseMPL-0.9.0/docs/examples/goosempl/random_from_cdf.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/random_from_cdf.svg` & `GooseMPL-0.9.0/docs/examples/goosempl/random_from_cdf.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/goosempl/readme.rst` & `GooseMPL-0.9.0/docs/examples/goosempl/readme.rst`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/colorbar.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/colorbar.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/colormap-part.py` & `GooseMPL-0.9.0/docs/examples/pyplot/colormap-part.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/colormap-part.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/colormap-part.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/colormap.py` & `GooseMPL-0.9.0/docs/examples/pyplot/colormap.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/colormap.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/colormap.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image.py` & `GooseMPL-0.9.0/docs/examples/pyplot/image.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/image.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image_subplots.py` & `GooseMPL-0.9.0/docs/examples/pyplot/image_subplots.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image_subplots.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/image_subplots.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image_subplots_bottom.py` & `GooseMPL-0.9.0/docs/examples/pyplot/image_subplots_bottom.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/image_subplots_bottom.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/image_subplots_bottom.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/legend_background.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/legend_background.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/legend_external.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/legend_external.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/multicolor.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/multicolor.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/plot-cmap.py` & `GooseMPL-0.9.0/docs/examples/pyplot/plot-cmap.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/plot-cmap.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/plot-cmap.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/plot-cycler.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/plot-cycler.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/plot.py` & `GooseMPL-0.9.0/docs/examples/pyplot/plot.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/plot.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/plot.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/readme.rst` & `GooseMPL-0.9.0/docs/examples/pyplot/readme.rst`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/subplot.py` & `GooseMPL-0.9.0/docs/examples/pyplot/subplot.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/subplot.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/subplot.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-formatter.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-formatter.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log.py` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log_1.py` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log_1.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log_1.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log_1.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log_2.py` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log_2.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-log_2.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-log_2.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-position.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-position.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-rotation-log.py` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-rotation-log.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/examples/pyplot/tick-rotation-log.svg` & `GooseMPL-0.9.0/docs/examples/pyplot/tick-rotation-log.svg`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/goosempl.rst` & `GooseMPL-0.9.0/docs/goosempl.rst`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/index.rst` & `GooseMPL-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/make.bat` & `GooseMPL-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/docs/style.rst` & `GooseMPL-0.9.0/docs/style.rst`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/setup.py` & `GooseMPL-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `GooseMPL-0.8.0/test/main.py` & `GooseMPL-0.9.0/test/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -168,15 +168,76 @@
         x = np.linspace(0, 1, 1000)
         y = 1.2 * np.exp(x * 3.4)
         prefactor, exponent = gplt.fit_exp(x, y, prefactor=1.2)
         self.assertTrue(np.isclose(prefactor, 1.2))
         self.assertTrue(np.isclose(exponent, 3.4))
 
 
+class Test_fit_linear(unittest.TestCase):
+    """
+    Fit a linear.
+    """
+
+    def test_offset_slope(self):
+
+        x = np.linspace(0, 1, 1000)
+        y = 1.2 + 3.4 * x
+        offset, slope = gplt.fit_linear(x, y)
+        self.assertTrue(np.isclose(offset, 1.2))
+        self.assertTrue(np.isclose(slope, 3.4))
+
+    def test_slope(self):
+
+        x = np.linspace(0, 1, 1000)
+        y = 1.2 + 3.4 * x
+        offset, slope = gplt.fit_linear(x, y, slope=3.4)
+        self.assertTrue(np.isclose(offset, 1.2))
+        self.assertTrue(np.isclose(slope, 3.4))
+
+    def test_offset(self):
+
+        x = np.linspace(0, 1, 1000)
+        y = 1.2 + 3.4 * x
+        offset, slope = gplt.fit_linear(x, y, offset=1.2)
+        self.assertTrue(np.isclose(offset, 1.2))
+        self.assertTrue(np.isclose(slope, 3.4))
+
+
+class Test_histogram_norm(unittest.TestCase):
+    """
+    Histogram normalisation.
+    """
+
+    def test_density(self):
+
+        data = [0, 0, 0, 1, 1, 2]
+        bin_edges = [-0.5, 0.5, 1.5, 2.5]
+        p = gplt.histogram_norm(*np.histogram(data, bins=bin_edges))
+        q = gplt.histogram_norm(p, bin_edges)
+        r, _ = np.histogram(data, bins=bin_edges, density=True)
+        self.assertTrue(np.allclose(p, r))
+        self.assertTrue(np.allclose(q, r))
+
+
+class Test_histogram_bin_edges2midpoint(unittest.TestCase):
+    """
+    Midpoints of bins
+    """
+
+    def test_simple(self):
+        bin_edges = [-0.5, 0.5, 1.5, 2.5]
+        mid = [0, 1, 2]
+        self.assertTrue(np.allclose(gplt.histogram_bin_edges2midpoint(bin_edges), mid))
+
+
 class Test_histogram_bin_edges_integer(unittest.TestCase):
+    """
+    Bin edges.
+    """
+
     def test_front(self):
 
         a = [0, 0.5, 1.5, 2.5]
         b = [0, 1.5, 2.5]
         self.assertTrue(np.allclose(gplt.histogram_bin_edges_integer(a), b))
 
     def test_middle(self):
```

