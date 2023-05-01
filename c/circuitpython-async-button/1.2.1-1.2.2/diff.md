# Comparing `tmp/circuitpython-async-button-1.2.1.tar.gz` & `tmp/circuitpython-async-button-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-async-button-1.2.1.tar", last modified: Mon Apr 10 19:57:58 2023, max compression
+gzip compressed data, was "circuitpython-async-button-1.2.2.tar", last modified: Mon May  1 21:57:43 2023, max compression
```

## Comparing `circuitpython-async-button-1.2.1.tar` & `circuitpython-async-button-1.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.063371 circuitpython-async-button-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/async_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.067371 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 19:57:58.000000 circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/events.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_double.json
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_long.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_single.json
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/docs/timing_triple.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_button_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_multibutton_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/examples/async_simplebutton_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-10 19:57:43.000000 circuitpython-async-button-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:58.071371 circuitpython-async-button-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_multi_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-10 19:57:50.000000 circuitpython-async-button-1.2.1/tests/test_async_simple_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.547347 circuitpython-async-button-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.547347 circuitpython-async-button-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.547347 circuitpython-async-button-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.547347 circuitpython-async-button-1.2.2/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/async_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-01 21:57:43.000000 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-01 21:57:43.000000 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:57:43.000000 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 21:57:43.000000 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 21:57:43.000000 circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/events.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/timing_double.json
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/timing_long.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/timing_single.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/docs/timing_triple.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/examples/async_button_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/examples/async_multibutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/examples/async_simplebutton_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-01 21:57:27.000000 circuitpython-async-button-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:43.551347 circuitpython-async-button-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/tests/test_async_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/tests/test_async_multi_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-01 21:57:36.000000 circuitpython-async-button-1.2.2/tests/test_async_simple_button.py
```

### Comparing `circuitpython-async-button-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-async-button-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/.gitignore` & `circuitpython-async-button-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/.pre-commit-config.yaml` & `circuitpython-async-button-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/.pylintrc` & `circuitpython-async-button-1.2.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/CODE_OF_CONDUCT.md` & `circuitpython-async-button-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/LICENSE` & `circuitpython-async-button-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/LICENSES/CC-BY-4.0.txt` & `circuitpython-async-button-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/LICENSES/MIT.txt` & `circuitpython-async-button-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/LICENSES/Unlicense.txt` & `circuitpython-async-button-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/PKG-INFO` & `circuitpython-async-button-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.2.1
+Version: 1.2.2
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.2.1/README.rst` & `circuitpython-async-button-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/async_button.py` & `circuitpython-async-button-1.2.2/async_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,19 @@
   https://github.com/adafruit/Adafruit_CircuitPython_asyncio
 
 * CircuitPython ticks module:
   https://github.com/adafruit/Adafruit_CircuitPython_Ticks
 """
 
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https://github.com/furbrain/CircuitPython_async_button.git"
 
 import asyncio
-from asyncio import Task, Event
+from asyncio import Event
 
 from adafruit_ticks import ticks_add, ticks_less, ticks_ms
 
 try:
     from typing import Dict, Sequence, Awaitable, Any, Union
 except ImportError:
     pass
@@ -252,15 +252,14 @@
         while True:
             if self.keys.events.get_into(evt):
                 if evt.pressed:
                     self._trigger(self.PRESSED)
                     now = getattr(
                         evt, "timestamp", ticks_ms()
                     )  # use now if timestamp not there
-                    # print(now, self.last_click_tm, self.double_click_max_duration)
                     if ticks_less(now, dbl_clk_expires):
                         self._increase_clicks()
                     else:
                         self.last_click = self.SINGLE
                     long_click_due = ticks_add(
                         now, int(self.long_click_min_duration * 1000)
                     )
@@ -325,24 +324,30 @@
 
         # multiple click types - needs more complex algorithm
         evts: Dict[int, TaskWrapper] = {}
         one_event_done = asyncio.Event()
         for evt_type in click_types:
             coro = self.events[evt_type].wait()
             evts[evt_type] = TaskWrapper(coro, one_event_done)
-        await one_event_done.wait()
-        if len(evts) > 1:
-            await asyncio.sleep(0)  # ensure all event types get an opportunity to run
-        results = []
-        for evt_type, evt in evts.items():
-            if evt.done():
-                results.append(evt_type)
-            else:
-                evt.cancel()  # cancel unfired events
-        return results
+        try:
+            await one_event_done.wait()
+            if len(evts) > 1:
+                await asyncio.sleep(
+                    0
+                )  # ensure all event types get an opportunity to run
+            results = []
+            for evt_type, evt in evts.items():
+                if evt.done():
+                    results.append(evt_type)
+            return results
+        finally:
+            # make sure all tasks are cancelled on exit
+            for evt in evts.values():
+                if not evt.done():
+                    evt.cancel()
 
     async def wait_for_click(self):
         """
         Wait for any click and return it
 
         :return: Which click happened i.e. one of `SINGLE`, `DOUBLE`, `TRIPLE` or `LONG`
         """
@@ -394,19 +399,23 @@
             >>> # Long click on button B
             >>> print(button, result) # "b", Button.Long
         """
         if len(kwargs) == 1:
             button = list(kwargs)[0]
             results = await self.buttons[button].wait(kwargs[button])
             return button, results[0]
-        tasks: Dict[Any, Task] = {}
+        tasks: Dict[Any, TaskWrapper] = {}
         click_happened = asyncio.Event()
         for key, value in kwargs.items():
             tasks[key] = TaskWrapper(self.buttons[key].wait(value), click_happened)
-        await click_happened.wait()
-        result = (None, None)
-        for key, task in tasks.items():
-            if task.done():
-                result = (key, task.result()[0])
-            else:
-                task.cancel()
-        return result
+        try:
+            await click_happened.wait()
+            result = (None, None)
+            for key, task in tasks.items():
+                if task.done():
+                    result = (key, task.result()[0])
+            return result
+        finally:
+            # make sure all tasks are cancelled on exit
+            for task in tasks.values():
+                if not task.done():
+                    task.cancel()
```

### Comparing `circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/PKG-INFO` & `circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-button
-Version: 1.2.1
+Version: 1.2.2
 Summary: a library for reading buttons using asyncio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_button
 Keywords: adafruit,blinka,circuitpython,micropython,async_button,async,asyncio,countio,keypad,button,press
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-async-button-1.2.1/circuitpython_async_button.egg-info/SOURCES.txt` & `circuitpython-async-button-1.2.2/circuitpython_async_button.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/_static/favicon.ico` & `circuitpython-async-button-1.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/conf.py` & `circuitpython-async-button-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/events.rst` & `circuitpython-async-button-1.2.2/docs/events.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/index.rst` & `circuitpython-async-button-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/timing_double.json` & `circuitpython-async-button-1.2.2/docs/timing_double.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/timing_long.json` & `circuitpython-async-button-1.2.2/docs/timing_long.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/timing_single.json` & `circuitpython-async-button-1.2.2/docs/timing_single.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/docs/timing_triple.json` & `circuitpython-async-button-1.2.2/docs/timing_triple.json`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/examples/async_button_test.py` & `circuitpython-async-button-1.2.2/examples/async_button_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/examples/async_multibutton_test.py` & `circuitpython-async-button-1.2.2/examples/async_multibutton_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/examples/async_simplebutton_test.py` & `circuitpython-async-button-1.2.2/examples/async_simplebutton_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/pyproject.toml` & `circuitpython-async-button-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-async-button"
 description = "a library for reading buttons using asyncio"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_async_button"}
 keywords = [
     "adafruit",
```

### Comparing `circuitpython-async-button-1.2.1/tests/test_async_button.py` & `circuitpython-async-button-1.2.2/tests/test_async_button.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/tests/test_async_multi_button.py` & `circuitpython-async-button-1.2.2/tests/test_async_multi_button.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-button-1.2.1/tests/test_async_simple_button.py` & `circuitpython-async-button-1.2.2/tests/test_async_simple_button.py`

 * *Files identical despite different names*

