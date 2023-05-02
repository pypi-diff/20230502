# Comparing `tmp/dvclive-2.8.0.tar.gz` & `tmp/dvclive-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvclive-2.8.0.tar", last modified: Thu Apr 27 16:09:24 2023, max compression
+gzip compressed data, was "dvclive-2.8.1.tar", last modified: Tue May  2 09:01:22 2023, max compression
```

## Comparing `dvclive-2.8.0.tar` & `dvclive-2.8.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.841721 dvclive-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-27 16:09:05.000000 dvclive-2.8.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 16:09:05.000000 dvclive-2.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.821719 dvclive-2.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 16:09:05.000000 dvclive-2.8.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 16:09:05.000000 dvclive-2.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-27 16:09:05.000000 dvclive-2.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-27 16:09:05.000000 dvclive-2.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-27 16:09:05.000000 dvclive-2.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-27 16:09:05.000000 dvclive-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-27 16:09:24.841721 dvclive-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-27 16:09:05.000000 dvclive-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-04-27 16:09:05.000000 dvclive-2.8.0/docs/dvc_plots_diff.png
--rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-04-27 16:09:05.000000 dvclive-2.8.0/docs/studio_compare.png
--rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-04-27 16:09:06.000000 dvclive-2.8.0/docs/vscode_experiments.png
--rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-04-27 16:09:06.000000 dvclive-2.8.0/docs/vscode_plots.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.825719 dvclive-2.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-04-27 16:09:06.000000 dvclive-2.8.0/examples/DVCLive-Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-27 16:09:06.000000 dvclive-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 16:09:24.841721 dvclive-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 16:09:06.000000 dvclive-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.821719 dvclive-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.829720 dvclive-2.8.0/src/dvclive/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/dvc.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/optuna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.833720 dvclive-2.8.0/src/dvclive/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/plots/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-27 16:09:06.000000 dvclive-2.8.0/src/dvclive/xgb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.833720 dvclive-2.8.0/src/dvclive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 16:09:24.000000 dvclive-2.8.0/src/dvclive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.837720 dvclive-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.837720 dvclive-2.8.0/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/plots/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_dvc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:09:24.841721 dvclive-2.8.0/tests/test_frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_lgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_frameworks/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_log_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 16:09:06.000000 dvclive-2.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 09:00:58.000000 dvclive-2.8.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 09:00:58.000000 dvclive-2.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 09:00:58.000000 dvclive-2.8.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-02 09:00:58.000000 dvclive-2.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-02 09:00:58.000000 dvclive-2.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-02 09:00:58.000000 dvclive-2.8.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-02 09:00:58.000000 dvclive-2.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-02 09:00:58.000000 dvclive-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-02 09:01:22.139661 dvclive-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-02 09:00:58.000000 dvclive-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.131661 dvclive-2.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   321138 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/dvc_plots_diff.png
+-rw-r--r--   0 runner    (1001) docker     (123)   676021 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/studio_compare.png
+-rw-r--r--   0 runner    (1001) docker     (123)   501824 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/vscode_experiments.png
+-rw-r--r--   0 runner    (1001) docker     (123)   627561 2023-05-02 09:00:58.000000 dvclive-2.8.1/docs/vscode_plots.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-02 09:00:58.000000 dvclive-2.8.1/examples/DVCLive-Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-02 09:00:58.000000 dvclive-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-02 09:01:22.139661 dvclive-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 09:00:58.000000 dvclive-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.127661 dvclive-2.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/src/dvclive/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/optuna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/src/dvclive/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/plots/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 09:00:58.000000 dvclive-2.8.1/src/dvclive/xgb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.135661 dvclive-2.8.1/src/dvclive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:01:21.000000 dvclive-2.8.1/src/dvclive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 09:01:22.000000 dvclive-2.8.1/src/dvclive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/plots/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_dvc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:01:22.139661 dvclive-2.8.1/tests/test_frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_lgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_frameworks/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_log_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 09:00:58.000000 dvclive-2.8.1/tests/test_utils.py
```

### Comparing `dvclive-2.8.0/.cruft.json` & `dvclive-2.8.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/.github/dependabot.yml` & `dvclive-2.8.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/.github/workflows/release.yml` & `dvclive-2.8.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/.github/workflows/tests.yml` & `dvclive-2.8.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/.gitignore` & `dvclive-2.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/.pre-commit-config.yaml` & `dvclive-2.8.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.262'
+    rev: 'v0.0.263'
     hooks:
       - id: ruff
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
     - id: mdformat
       args: ["--wrap=80"]
```

### Comparing `dvclive-2.8.0/CODE_OF_CONDUCT.rst` & `dvclive-2.8.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/CONTRIBUTING.rst` & `dvclive-2.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/LICENSE` & `dvclive-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/PKG-INFO` & `dvclive-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.8.0
+Version: 2.8.1
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.8.0 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.8.1 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.8.0/README.md` & `dvclive-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/docs/dvc_plots_diff.png` & `dvclive-2.8.1/docs/dvc_plots_diff.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/docs/studio_compare.png` & `dvclive-2.8.1/docs/studio_compare.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/docs/vscode_experiments.png` & `dvclive-2.8.1/docs/vscode_experiments.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/docs/vscode_plots.png` & `dvclive-2.8.1/docs/vscode_plots.png`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/examples/DVCLive-Quickstart.ipynb` & `dvclive-2.8.1/examples/DVCLive-Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/pyproject.toml` & `dvclive-2.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/setup.cfg` & `dvclive-2.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/catalyst.py` & `dvclive-2.8.1/src/dvclive/catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/dvc.py` & `dvclive-2.8.1/src/dvclive/dvc.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/error.py` & `dvclive-2.8.1/src/dvclive/error.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/fastai.py` & `dvclive-2.8.1/src/dvclive/fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/huggingface.py` & `dvclive-2.8.1/src/dvclive/huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/keras.py` & `dvclive-2.8.1/src/dvclive/keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/lgbm.py` & `dvclive-2.8.1/src/dvclive/lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/lightning.py` & `dvclive-2.8.1/src/dvclive/lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/live.py` & `dvclive-2.8.1/src/dvclive/live.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,21 +508,24 @@
 
     def _ensure_paths_are_tracked_in_dvc_exp(self):
         if self._inside_dvc_exp and self._dvc_repo:
             dir_spec = PathSpec.from_lines("gitwildmatch", [self.dir])
             outs_spec = PathSpec.from_lines(
                 "gitwildmatch", [str(o) for o in self._dvc_repo.index.outs]
             )
-            paths_to_track = [
-                f
-                for f in self._dvc_repo.scm.untracked_files()
-                if (dir_spec.match_file(f) and not outs_spec.match_file(f))
-            ]
-            if paths_to_track:
-                self._dvc_repo.scm.add(paths_to_track)
+            try:
+                paths_to_track = [
+                    f
+                    for f in self._dvc_repo.scm.untracked_files()
+                    if (dir_spec.match_file(f) and not outs_spec.match_file(f))
+                ]
+                if paths_to_track:
+                    self._dvc_repo.scm.add(paths_to_track)
+            except Exception as e:  # noqa: BLE001
+                logger.warning(f"Failed to git add paths:\n{e}")
 
     def save_dvc_exp(self):
         if self._save_dvc_exp:
             from dvc.exceptions import DvcException
 
             try:
                 self._experiment_rev = self._dvc_repo.experiments.save(
```

### Comparing `dvclive-2.8.0/src/dvclive/optuna.py` & `dvclive-2.8.1/src/dvclive/optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/plots/base.py` & `dvclive-2.8.1/src/dvclive/plots/base.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/plots/custom.py` & `dvclive-2.8.1/src/dvclive/plots/custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/plots/image.py` & `dvclive-2.8.1/src/dvclive/plots/image.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,18 +11,21 @@
     def output_path(self) -> Path:
         _path = self.output_folder / self.name
         _path.parent.mkdir(exist_ok=True, parents=True)
         return _path
 
     @staticmethod
     def could_log(val: object) -> bool:
-        if val.__class__.__module__ == "PIL.Image":
-            return True
-        if val.__class__.__module__ == "numpy":
-            return True
+        acceptable = {
+            ("numpy", "ndarray"),
+            ("PIL.Image", "Image"),
+        }
+        for cls in type(val).mro():
+            if (cls.__module__, cls.__name__) in acceptable:
+                return True
         if isinstance(val, (PurePath, str)):
             return True
         return False
 
     def dump(self, val, **kwargs) -> None:  # noqa: ARG002
         if val.__class__.__module__ == "numpy":
             from PIL import Image as ImagePIL
```

### Comparing `dvclive-2.8.0/src/dvclive/plots/metric.py` & `dvclive-2.8.1/src/dvclive/plots/metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/plots/sklearn.py` & `dvclive-2.8.1/src/dvclive/plots/sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/plots/utils.py` & `dvclive-2.8.1/src/dvclive/plots/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/report.py` & `dvclive-2.8.1/src/dvclive/report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/serialize.py` & `dvclive-2.8.1/src/dvclive/serialize.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/studio.py` & `dvclive-2.8.1/src/dvclive/studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/utils.py` & `dvclive-2.8.1/src/dvclive/utils.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive/xgb.py` & `dvclive-2.8.1/src/dvclive/xgb.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive.egg-info/PKG-INFO` & `dvclive-2.8.1/src/dvclive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvclive
-Version: 2.8.0
+Version: 2.8.1
 Summary: Metric logger for ML projects.
 Home-page: https://github.com/iterative/dvclive
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Project-URL: Documentation, https://dvc.org/doc/dvclive
 Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvclive Version: 2.8.0 Summary: Metric logger for
+Metadata-Version: 2.1 Name: dvclive Version: 2.8.1 Summary: Metric logger for
 ML projects. Home-page: https://github.com/iterative/dvclive Maintainer-email:
 support@dvc.org License: Apache-2.0 Project-URL: Documentation, https://
 dvc.org/doc/dvclive Project-URL: Source, https://github.com/iterative/dvclive
 Keywords: data-science,metrics,machine-learning,developer-tools,ai Platform:
 any Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

### Comparing `dvclive-2.8.0/src/dvclive.egg-info/SOURCES.txt` & `dvclive-2.8.1/src/dvclive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/src/dvclive.egg-info/requires.txt` & `dvclive-2.8.1/src/dvclive.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/conftest.py` & `dvclive-2.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/plots/test_custom.py` & `dvclive-2.8.1/tests/plots/test_custom.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/plots/test_image.py` & `dvclive-2.8.1/tests/plots/test_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 import pytest
 from PIL import Image
 
 from dvclive import Live
 from dvclive.plots import Image as LiveImage
 
 
+# From https://stackoverflow.com/questions/5165317/how-can-i-extend-image-class
+class ExtendedImage(Image.Image):
+    def __init__(self, img):
+        self._img = img
+
+    def __getattr__(self, key):
+        return getattr(self._img, key)
+
+
 def test_pil(tmp_dir):
     live = Live()
     img = Image.new("RGB", (10, 10), (250, 250, 250))
     live.log_image("image.png", img)
 
     assert (tmp_dir / live.plots_dir / LiveImage.subfolder / "image.png").exists()
 
@@ -78,7 +87,16 @@
     live.log_image("image.png", img)
 
     assert (tmp_dir / live.plots_dir / LiveImage.subfolder / "image.png").exists()
 
     Live()
 
     assert not (tmp_dir / live.plots_dir / LiveImage.subfolder).exists()
+
+
+def test_custom_class(tmp_dir):
+    live = Live()
+    img = Image.new("RGB", (10, 10), (250, 250, 250))
+    extended_img = ExtendedImage(img)
+    live.log_image("image.png", extended_img)
+
+    assert (tmp_dir / live.plots_dir / LiveImage.subfolder / "image.png").exists()
```

### Comparing `dvclive-2.8.0/tests/plots/test_metric.py` & `dvclive-2.8.1/tests/plots/test_metric.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/plots/test_sklearn.py` & `dvclive-2.8.1/tests/plots/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_dvc.py` & `dvclive-2.8.1/tests/test_dvc.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,7 +254,17 @@
     ]
 
     with Live(report=None) as live:
         live.log_metric("foo", 1)
         live.next_step()
 
     live._dvc_repo.scm.add.assert_called_with(["dvclive/metrics.json"])
+
+
+def test_errors_on_git_add_are_catched(tmp_dir, mocked_dvc_repo, monkeypatch):
+    monkeypatch.setenv(DVC_EXP_BASELINE_REV, "foo")
+    monkeypatch.setenv(DVC_EXP_NAME, "bar")
+    mocked_dvc_repo.scm.untracked_files.return_value = ["dvclive/metrics.json"]
+    mocked_dvc_repo.scm.add.side_effect = Exception("foo")
+
+    with Live(report=None) as live:
+        live.summary["foo"] = 1
```

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_catalyst.py` & `dvclive-2.8.1/tests/test_frameworks/test_catalyst.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_fastai.py` & `dvclive-2.8.1/tests/test_frameworks/test_fastai.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_huggingface.py` & `dvclive-2.8.1/tests/test_frameworks/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_keras.py` & `dvclive-2.8.1/tests/test_frameworks/test_keras.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_lgbm.py` & `dvclive-2.8.1/tests/test_frameworks/test_lgbm.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_lightning.py` & `dvclive-2.8.1/tests/test_frameworks/test_lightning.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_optuna.py` & `dvclive-2.8.1/tests/test_frameworks/test_optuna.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_frameworks/test_xgboost.py` & `dvclive-2.8.1/tests/test_frameworks/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_log_artifact.py` & `dvclive-2.8.1/tests/test_log_artifact.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_main.py` & `dvclive-2.8.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_report.py` & `dvclive-2.8.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_studio.py` & `dvclive-2.8.1/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvclive-2.8.0/tests/test_utils.py` & `dvclive-2.8.1/tests/test_utils.py`

 * *Files identical despite different names*

