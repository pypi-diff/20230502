# Comparing `tmp/peppyproject-1.0.0.tar.gz` & `tmp/peppyproject-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peppyproject-1.0.0.tar", last modified: Tue Feb 14 17:19:44 2023, max compression
+gzip compressed data, was "peppyproject-1.0.1.tar", last modified: Tue May  2 12:58:56 2023, max compression
```

## Comparing `peppyproject-1.0.0.tar` & `peppyproject-1.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-14 17:19:25.000000 peppyproject-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-14 17:19:25.000000 peppyproject-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-14 17:19:25.000000 peppyproject-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43439 2023-02-14 17:19:44.745385 peppyproject-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-14 17:19:25.000000 peppyproject-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/peppyproject/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/peppyproject/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/flake8.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/ruff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-14 17:19:25.000000 peppyproject-1.0.0/peppyproject/tools/setuptools_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/peppyproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43439 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-14 17:19:44.000000 peppyproject-1.0.0/peppyproject.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-14 17:19:25.000000 peppyproject-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:19:44.745385 peppyproject-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/tests/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/input/pyproject_toml/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/pyproject_toml/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/input/setup_cfg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/input/setup_cfg/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_cfg/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_cfg/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_cfg/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_cfg/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_cfg/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/input/setup_py/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_py/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_py/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_py/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/input/setup_py/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.741385 peppyproject-1.0.0/tests/data/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/reference/pyproject_toml/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/reference/pyproject_toml/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/reference/setup_cfg/
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/reference/setup_cfg/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:19:44.745385 peppyproject-1.0.0/tests/data/reference/setup_py/
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/data/reference/setup_py/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tests/test_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-14 17:19:25.000000 peppyproject-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.760673 peppyproject-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.760673 peppyproject-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 12:58:42.000000 peppyproject-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-02 12:58:42.000000 peppyproject-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 12:58:42.000000 peppyproject-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43501 2023-05-02 12:58:56.768673 peppyproject-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-02 12:58:42.000000 peppyproject-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.764673 peppyproject-1.0.1/peppyproject/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13194 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.764673 peppyproject-1.0.1/peppyproject/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/ruff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-02 12:58:42.000000 peppyproject-1.0.1/peppyproject/tools/setuptools_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.764673 peppyproject-1.0.1/peppyproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43501 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 12:58:56.000000 peppyproject-1.0.1/peppyproject.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-02 12:58:42.000000 peppyproject-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:58:56.768673 peppyproject-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.764673 peppyproject-1.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.760673 peppyproject-1.0.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.760673 peppyproject-1.0.1/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/input/pyproject_toml/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/pyproject_toml/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/input/setup_cfg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/input/setup_cfg/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_cfg/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_cfg/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_cfg/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_cfg/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_cfg/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/input/setup_py/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_py/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_py/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_py/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/input/setup_py/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.760673 peppyproject-1.0.1/tests/data/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/reference/pyproject_toml/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/reference/pyproject_toml/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/reference/setup_cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/reference/setup_cfg/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:58:56.768673 peppyproject-1.0.1/tests/data/reference/setup_py/
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/data/reference/setup_py/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tests/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-02 12:58:42.000000 peppyproject-1.0.1/tox.ini
```

### Comparing `peppyproject-1.0.0/.github/workflows/build.yml` & `peppyproject-1.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/LICENSE` & `peppyproject-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/PKG-INFO` & `peppyproject-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peppyproject
-Version: 1.0.0
+Version: 1.0.1
 Summary: create a PEP621-compliant `pyproject.toml` file from existing build configuration
 Author: Zach Burnett
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,14 +709,21 @@
 
 ```shell
 pip install peppyproject
 ```
 
 ### Usage
 
+> **Warning**
+> `peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse a `setup.py` file. **It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking; thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.**
+
+```
+peppyproject . -o pyproject.toml
+```
+
 ```
 Usage: peppyproject [OPTIONS] [DIRECTORY]
 
   read a Python project configuration and output a PEP621-compliant `pyproject.toml`
 
 Arguments:
   [DIRECTORY]  directory from which to read configuration
@@ -724,17 +731,13 @@
 Options:
   -o, --output PATH  path to which to write TOML
   --help             Show this message and exit.
 ```
 
 ### API
 
-`peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse
-a `setup.py` file. It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking;
-thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.
-
 ```python
 from peppyproject import PyProjectConfiguration
 
 configuration = PyProjectConfiguration.from_directory('./my_python_project')
 configuration.to_file('./my_python_project/pyproject.toml')
 ```
```

### Comparing `peppyproject-1.0.0/README.md` & `peppyproject-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 
 ```shell
 pip install peppyproject
 ```
 
 ### Usage
 
+> **Warning**
+> `peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse a `setup.py` file. **It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking; thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.**
+
+```
+peppyproject . -o pyproject.toml
+```
+
 ```
 Usage: peppyproject [OPTIONS] [DIRECTORY]
 
   read a Python project configuration and output a PEP621-compliant `pyproject.toml`
 
 Arguments:
   [DIRECTORY]  directory from which to read configuration
@@ -31,17 +38,13 @@
 Options:
   -o, --output PATH  path to which to write TOML
   --help             Show this message and exit.
 ```
 
 ### API
 
-`peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse
-a `setup.py` file. It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking;
-thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.
-
 ```python
 from peppyproject import PyProjectConfiguration
 
 configuration = PyProjectConfiguration.from_directory('./my_python_project')
 configuration.to_file('./my_python_project/pyproject.toml')
-```
+```
```

### Comparing `peppyproject-1.0.0/peppyproject/__main__.py` & `peppyproject-1.0.1/peppyproject/__main__.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/base.py` & `peppyproject-1.0.1/peppyproject/base.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/configuration.py` & `peppyproject-1.0.1/peppyproject/configuration.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/files.py` & `peppyproject-1.0.1/peppyproject/files.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tables.py` & `peppyproject-1.0.1/peppyproject/tables.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tools/coverage.py` & `peppyproject-1.0.1/peppyproject/tools/coverage.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tools/flake8.py` & `peppyproject-1.0.1/peppyproject/tools/flake8.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tools/ruff.py` & `peppyproject-1.0.1/peppyproject/tools/ruff.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tools/setuptools.py` & `peppyproject-1.0.1/peppyproject/tools/setuptools.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject/tools/setuptools_scm.py` & `peppyproject-1.0.1/peppyproject/tools/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/peppyproject.egg-info/PKG-INFO` & `peppyproject-1.0.1/peppyproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peppyproject
-Version: 1.0.0
+Version: 1.0.1
 Summary: create a PEP621-compliant `pyproject.toml` file from existing build configuration
 Author: Zach Burnett
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -709,14 +709,21 @@
 
 ```shell
 pip install peppyproject
 ```
 
 ### Usage
 
+> **Warning**
+> `peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse a `setup.py` file. **It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking; thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.**
+
+```
+peppyproject . -o pyproject.toml
+```
+
 ```
 Usage: peppyproject [OPTIONS] [DIRECTORY]
 
   read a Python project configuration and output a PEP621-compliant `pyproject.toml`
 
 Arguments:
   [DIRECTORY]  directory from which to read configuration
@@ -724,17 +731,13 @@
 Options:
   -o, --output PATH  path to which to write TOML
   --help             Show this message and exit.
 ```
 
 ### API
 
-`peppyproject` uses `ini2toml[full]` to read `setup.cfg` and INI files, and `ast.literal_eval()` to read and parse
-a `setup.py` file. It assumes you have vetted the ``setup.py`` and does not perform any sanitization or safety checking;
-thus, it is inadvisable to use on unknown or potentially malicious ``setup.py`` scripts.
-
 ```python
 from peppyproject import PyProjectConfiguration
 
 configuration = PyProjectConfiguration.from_directory('./my_python_project')
 configuration.to_file('./my_python_project/pyproject.toml')
 ```
```

### Comparing `peppyproject-1.0.0/peppyproject.egg-info/SOURCES.txt` & `peppyproject-1.0.1/peppyproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/pyproject.toml` & `peppyproject-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "ini2toml[full]",
-    "tomli",
-    "tomli-w",
+    "tomli>=2",
+    "tomli-w>=1",
     "typepigeon>=2.0.1",
     "typer",
 ]
 dynamic = [
     "version",
 ]
```

### Comparing `peppyproject-1.0.0/tests/data/input/pyproject_toml/LICENSE` & `peppyproject-1.0.1/tests/data/input/pyproject_toml/LICENSE`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/pyproject_toml/README.md` & `peppyproject-1.0.1/tests/data/input/pyproject_toml/README.md`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/pyproject_toml/pyproject.toml` & `peppyproject-1.0.1/tests/data/input/pyproject_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/pyproject_toml/tox.ini` & `peppyproject-1.0.1/tests/data/input/pyproject_toml/tox.ini`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_cfg/docs/conf.py` & `peppyproject-1.0.1/tests/data/input/setup_cfg/docs/conf.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_cfg/pyproject.toml` & `peppyproject-1.0.1/tests/data/input/setup_cfg/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_cfg/setup.cfg` & `peppyproject-1.0.1/tests/data/input/setup_cfg/setup.cfg`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_cfg/setup.py` & `peppyproject-1.0.1/tests/data/input/setup_cfg/setup.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_cfg/tox.ini` & `peppyproject-1.0.1/tests/data/input/setup_cfg/tox.ini`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_py/LICENSE` & `peppyproject-1.0.1/tests/data/input/setup_py/LICENSE`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_py/README.rst` & `peppyproject-1.0.1/tests/data/input/setup_py/README.rst`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/input/setup_py/setup.py` & `peppyproject-1.0.1/tests/data/input/setup_py/setup.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/reference/pyproject_toml/pyproject.toml` & `peppyproject-1.0.1/tests/data/reference/pyproject_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/data/reference/setup_cfg/pyproject.toml` & `peppyproject-1.0.1/tests/data/reference/setup_cfg/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -238,17 +238,15 @@
 inputs_root = "jwst-pipeline"
 results_root = "jwst-pipeline-results"
 text_file_format = "rst"
 doctest_plus = "enabled"
 doctest_rst = "enabled"
 addopts = "--show-capture=no --open-files --report-crds-context"
 filterwarnings = [
-    "ignore:Models",
-    "in",
-    "math_functions:astropy.utils.exceptions.AstropyUserWarning",
+    "ignore:Models in math_functions:astropy.utils.exceptions.AstropyUserWarning",
 ]
 
 [tool.coverage.run]
 omit = [
     "jwst/conftest.py",
     "jwst/setup.py",
     "jwst/tests/test*",
```

### Comparing `peppyproject-1.0.0/tests/data/reference/setup_py/pyproject.toml` & `peppyproject-1.0.1/tests/data/reference/setup_py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/test_cli.py` & `peppyproject-1.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/test_configuration.py` & `peppyproject-1.0.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/test_read.py` & `peppyproject-1.0.1/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tests/test_write.py` & `peppyproject-1.0.1/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `peppyproject-1.0.0/tox.ini` & `peppyproject-1.0.1/tox.ini`

 * *Files identical despite different names*

