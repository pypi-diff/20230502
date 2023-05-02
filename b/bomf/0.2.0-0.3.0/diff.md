# Comparing `tmp/bomf-0.2.0.tar.gz` & `tmp/bomf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.2.0.tar", last modified: Mon Apr 24 12:32:52 2023, max compression
+gzip compressed data, was "bomf-0.3.0.tar", last modified: Tue May  2 07:15:40 2023, max compression
```

## Comparing `bomf-0.2.0.tar` & `bomf-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.909682 bomf-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-24 12:32:44.000000 bomf-0.2.0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-24 12:32:44.000000 bomf-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-24 12:32:44.000000 bomf-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 12:32:44.000000 bomf-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-24 12:32:52.909682 bomf-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-24 12:32:44.000000 bomf-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 12:32:44.000000 bomf-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:32:44.000000 bomf-0.2.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-24 12:32:44.000000 bomf-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-24 12:32:52.909682 bomf-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 12:32:44.000000 bomf-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.897682 bomf-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.901682 bomf-0.2.0/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-24 12:32:44.000000 bomf-0.2.0/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.905682 bomf-0.2.0/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 12:32:52.000000 bomf-0.2.0/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-24 12:32:44.000000 bomf-0.2.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:32:52.909682 bomf-0.2.0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-24 12:32:44.000000 bomf-0.2.0/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.282536 bomf-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-02 07:15:29.000000 bomf-0.3.0/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-02 07:15:29.000000 bomf-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-02 07:15:29.000000 bomf-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-02 07:15:29.000000 bomf-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-02 07:15:40.286537 bomf-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-02 07:15:29.000000 bomf-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-02 07:15:29.000000 bomf-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 07:15:29.000000 bomf-0.3.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-02 07:15:29.000000 bomf-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-02 07:15:40.290536 bomf-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 07:15:29.000000 bomf-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.282536 bomf-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-02 07:15:29.000000 bomf-0.3.0/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 07:15:40.000000 bomf-0.3.0/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-02 07:15:29.000000 bomf-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:15:40.286537 bomf-0.3.0/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18482 2023-05-02 07:15:29.000000 bomf-0.3.0/unittests/test_validation.py
```

### Comparing `bomf-0.2.0/.github/dependabot.yml` & `bomf-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/black.yml` & `bomf-0.3.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/codeql-analysis.yml` & `bomf-0.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/coverage.yml` & `bomf-0.3.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/packaging_test.yml` & `bomf-0.3.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/python-publish.yml` & `bomf-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/pythonlint.yml` & `bomf-0.3.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.github/workflows/unittests.yml` & `bomf-0.3.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.gitignore` & `bomf-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/.pre-commit-config.yaml` & `bomf-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/LICENSE` & `bomf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/PKG-INFO` & `bomf-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.2.0
+Version: 0.3.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.2.0/README.md` & `bomf-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/pyproject.toml` & `bomf-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/requirements.txt` & `bomf-0.3.0/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile requirements.in
+#    pip-compile '.\requirements.in'
 #
 attrs==23.1.0
     # via -r requirements.in
 bidict==0.22.1
     # via -r requirements.in
 bo4e==0.4.7
     # via -r requirements.in
-frozendict==2.3.7
+frozendict==2.3.8
     # via -r requirements.in
 iso3166==2.1.1
     # via bo4e
+networkx==3.1
+    # via -r requirements.in
 pydantic==1.10.7
     # via
     #   -r requirements.in
     #   bo4e
 pyhumps==3.8.0
     # via bo4e
 typeguard==2.13.3
```

### Comparing `bomf-0.2.0/setup.cfg` & `bomf-0.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 install_requires = 
 	attrs
 	bo4e
 	pydantic
 	typeguard
 	frozendict
 	bidict
+	networkx
 
 [options.packages.find]
 where = src
 exclude = 
 	unittests
 
 [options.package_data]
```

### Comparing `bomf-0.2.0/src/bomf/__init__.py` & `bomf-0.3.0/src/bomf/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 import attrs
 
 from bomf.filter import Filter
 from bomf.loader.entityloader import EntityLoader, LoadingSummary
 from bomf.mapper import Bo4eDataSetToTargetMapper, IntermediateDataSet, SourceToBo4eDataSetMapper, TargetDataModel
 from bomf.provider import KeyTyp, SourceDataProvider
-from bomf.validation import ValidatorSet
+from bomf.validation import ValidationManager
 
 
 # pylint:disable=too-few-public-methods
 @attrs.define(kw_only=True, auto_attribs=True)
 class MigrationStrategy(ABC, Generic[IntermediateDataSet, TargetDataModel]):
     """
     A migration strategy describes the whole migration flow of datasets from a source to a target system
     """
 
     source_data_set_to_bo4e_mapper: SourceToBo4eDataSetMapper[IntermediateDataSet]
     """
     A mapper that transforms source data models into data sets that consist of bo4e objects
     """
-    validation: ValidatorSet[IntermediateDataSet]
+    validation: ValidationManager[IntermediateDataSet]
     """
     a set of validation rules that are applied to the bo4e data sets
     """
     bo4e_to_target_mapper: Bo4eDataSetToTargetMapper[TargetDataModel, IntermediateDataSet]
     """
     a mapper that transforms bo4e data sets to a structure that suits the target system
     """
@@ -43,11 +43,13 @@
         1. create bo4e data source using the source_data_set_to_bo4e_mapper
         2. checking that all the bo4e data sets obey the validation rules
         3. mapping from bo4e to the target data model
         4. loading the target data models into the target system.
         """
         # todo: here we should add some logging and statistics stuff
         bo4e_datasets = await self.source_data_set_to_bo4e_mapper.create_data_sets()
-        await self.validation.validate(*bo4e_datasets)
-        target_data_models = await self.bo4e_to_target_mapper.create_target_models(bo4e_datasets)
+        validation_result = await self.validation.validate(*bo4e_datasets)
+        target_data_models = await self.bo4e_to_target_mapper.create_target_models(
+            validation_result.succeeded_data_sets
+        )
         loading_summaries = await self.target_loader.load_entities(target_data_models)
         return loading_summaries
```

### Comparing `bomf-0.2.0/src/bomf/filter/__init__.py` & `bomf-0.3.0/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.3.0/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf/loader/entityloader.py` & `bomf-0.3.0/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf/mapper/__init__.py` & `bomf-0.3.0/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf/model/__init__.py` & `bomf-0.3.0/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf/provider/__init__.py` & `bomf-0.3.0/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/src/bomf.egg-info/PKG-INFO` & `bomf-0.3.0/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.2.0
+Version: 0.3.0
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.2.0/src/bomf.egg-info/SOURCES.txt` & `bomf-0.3.0/src/bomf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,22 @@
 src/bomf/filter/sourcedataproviderfilter.py
 src/bomf/loader/__init__.py
 src/bomf/loader/entityloader.py
 src/bomf/mapper/__init__.py
 src/bomf/model/__init__.py
 src/bomf/provider/__init__.py
 src/bomf/validation/__init__.py
-src/bomf/validation/core.py
 src/bomf/validation/utils.py
+src/bomf/validation/core/__init__.py
+src/bomf/validation/core/analysis.py
+src/bomf/validation/core/errors.py
+src/bomf/validation/core/execution.py
+src/bomf/validation/core/types.py
+src/bomf/validation/core/utils.py
+src/bomf/validation/core/validator.py
 unittests/__init__.py
 unittests/example_source_data.json
 unittests/test_bo4e_data_set.py
 unittests/test_entity_loader.py
 unittests/test_filter.py
 unittests/test_mapper.py
 unittests/test_migration.py
```

### Comparing `bomf-0.2.0/tox.ini` & `bomf-0.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # the type_check environment checks the type hints using mypy
 setenv = PYTHONPATH = {toxinidir}/src
 deps =
     -rrequirements.txt
     {[testenv:tests]deps}
     mypy
     types-frozendict
+    networkx-stubs
 commands =
     mypy --show-error-codes --check-untyped-defs src/bomf
     mypy --show-error-codes --check-untyped-defs unittests
     # add single files (ending with .py) or packages here
 
 [testenv:coverage]
 # the coverage environment is called by the Github Action that runs the coverage measurement
```

### Comparing `bomf-0.2.0/unittests/test_bo4e_data_set.py` & `bomf-0.3.0/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/unittests/test_entity_loader.py` & `bomf-0.3.0/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/unittests/test_filter.py` & `bomf-0.3.0/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/unittests/test_mapper.py` & `bomf-0.3.0/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/unittests/test_migration.py` & `bomf-0.3.0/unittests/test_migration.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 from bomf import (
     Bo4eDataSetToTargetMapper,
     EntityLoader,
     Filter,
     MigrationStrategy,
     SourceDataProvider,
     SourceToBo4eDataSetMapper,
-    ValidatorSet,
+    ValidationManager,
 )
 from bomf.loader.entityloader import EntityLoadingResult
 from bomf.model import Bo4eDataSet
-from bomf.provider import KeyTyp, SourceDataModel
+from bomf.provider import KeyTyp
+from bomf.validation import PathMappedValidator, Validator
+from bomf.validation.core import SyncValidatorFunction
 
 _MySourceDataModel = Dict[str, str]
 _MyKeyTyp = str
 _MyTargetDataModel = List[str]
 
 
 class _MyIntermediateDataModel(Bo4eDataSet):
@@ -55,21 +57,24 @@
         # what_ever_you_like is a place holde for all the relation magic that may happen
         self._source_models = what_ever_you_like
 
     async def create_data_sets(self) -> List[_MyIntermediateDataModel]:
         return [_MyIntermediateDataModel(data=source) for source in self._source_models]
 
 
-async def _my_rule(data: Dict[str, str]) -> None:
+def _my_rule(data: dict[str, str]):
     if "invalid" in data:
         raise ValueError("'invalid' in data")
 
 
-_my_validation = ValidatorSet[_MyIntermediateDataModel]()
-_my_validation.register(_my_rule, {"data": "data"})
+_my_mapped_validator: PathMappedValidator[_MyIntermediateDataModel, SyncValidatorFunction] = PathMappedValidator(
+    Validator(_my_rule), {"data": "data"}
+)
+_my_validation = ValidationManager[_MyIntermediateDataModel]()
+_my_validation.register(_my_mapped_validator)
 
 
 class _MyToTargetMapper(Bo4eDataSetToTargetMapper[_MyTargetDataModel, _MyIntermediateDataModel]):
     async def create_target_model(self, dataset: _MyIntermediateDataModel) -> _MyTargetDataModel:
         my_dict = dataset.data
         for my_key, my_value in my_dict.items():
             return [my_key, my_value]
```

### Comparing `bomf-0.2.0/unittests/test_source_data_provider.py` & `bomf-0.3.0/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.2.0/unittests/test_validation.py` & `bomf-0.3.0/unittests/test_validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 from datetime import timedelta
 from typing import Optional
 
 import pytest
 from frozendict import frozendict
 from pydantic import BaseModel, Required
 
-from bomf import ValidatorSet
+from bomf import ValidationManager
 from bomf.model import Bo4eDataSet
-from bomf.validation import optional_field, required_field
-from bomf.validation.core import ValidationError, ValidatorParamInfos, ValidatorType, _ValidatorMapInternIndexType
+from bomf.validation import PathMappedValidator, Validator, optional_field, param, required_field
+from bomf.validation.core import ValidationError, ValidatorFunctionT
+from bomf.validation.core.types import (
+    AsyncValidatorFunction,
+    MappedValidatorT,
+    SyncValidatorFunction,
+    ValidatorFunction,
+)
 
 
 class Wrapper(BaseModel):
     x: str
     z: Optional[str] = Required
 
 
@@ -21,20 +27,20 @@
     x: str
     y: int
     z: Wrapper
     a: int = -1
 
 
 dataset_instance = DataSetTest(x="lo16", y=16, z=Wrapper.construct(x="Hello"))
-finishing_order: list[ValidatorType]
+finishing_order: list[ValidatorFunction]
 
 
-async def check_multiple_registration(_param_infos: dict[str, ValidatorParamInfos], x: str):
-    assert _param_infos["x"].attribute_path in (["x"], ["z", "x"])
-    if _param_infos["x"].attribute_path == ["x"]:
+def check_multiple_registration(x: str):
+    assert param("x").param_id in ("x", "z.x")
+    if param("x").param_id == "x":
         assert x == "lo16"
     else:
         assert x == "Hello"
     finishing_order.append(check_multiple_registration)
 
 
 async def check_x_expensive(x: str) -> None:
@@ -50,176 +56,199 @@
 
 async def check_xy_ending(x: str, y: int) -> None:
     if not x.endswith(str(y)):
         raise ValueError("x does not end with y")
     finishing_order.append(check_xy_ending)
 
 
-async def check_required_and_optional(zx: str, zz: Optional[str] = None) -> None:
+def check_required_and_optional(zx: str, zz: str | None = None) -> None:
     assert zx == "Hello"
     assert zz is None
 
 
-async def check_required_and_optional_with_utility(z: Wrapper) -> None:
-    assert required_field(z, ["x"], str) == "Hello"
-    assert optional_field(z, ["z"], str) is None
-
-
-async def check_with_param_info(x: str, _param_infos: dict[str, ValidatorParamInfos], zz: str = "test"):
-    assert len(_param_infos) == 2
-    assert "x" in _param_infos
-    assert "zz" in _param_infos
-    assert str == _param_infos["x"].param_type
-    assert str == _param_infos["zz"].param_type
-    assert _param_infos["x"].required
-    assert _param_infos["x"].provided
-    assert not _param_infos["zz"].required
-    assert not _param_infos["zz"].provided
-    assert ["x"] == _param_infos["x"].attribute_path
-    assert ["z", "z"] == _param_infos["zz"].attribute_path
+def check_required_and_optional_with_utility(z: Wrapper) -> None:
+    assert required_field(z, "x", str) == "Hello"
+    assert optional_field(z, "z", str) is None
 
 
-async def unprovided_but_required(zz: str):
+def check_with_param_info(x: str, zz: str = "test"):
+    x_param = param("x")
+    assert x_param.name == "x"
+    assert x_param.param_id == "x"
+    assert x_param.provided
+    assert x_param.value == x
+    zz_param = param("zz")
+    assert zz_param.name == "zz"
+    assert zz_param.param_id == "z.z"
+    assert not zz_param.provided
+    assert zz_param.value == zz and zz == "test"
+
+
+def check_with_param_info_fail(zz: str = "test"):
+    unmapped_param = param("zz")
+
+
+def unprovided_but_required(zz: str):
     pass
 
 
-async def check_fail(x: str) -> None:
+def check_fail(x: str) -> None:
     raise ValueError("I failed (on purpose! :O)")
 
 
-async def check_fail2(y: int) -> None:
+def check_fail2(y: int) -> None:
     raise ValueError("I failed (on purpose! :O - again :OOO)")
 
 
-async def check_fail3(y: int) -> None:
+def check_fail3(y: int) -> None:
     raise ValueError("This shouldn't be raised")
 
 
-async def check_different_fails(x: str):
+def check_different_fails(x: str):
     if x == "Hello":
         raise ValueError("Error 1")
     else:
         raise ValueError("Error 2")
 
 
-async def no_params():
+def no_params():
     pass
 
 
-async def special_param_type_check_fail(x: str, _param_infos: dict[int, float]):
+def missing_annotation_y(x: str, y) -> None:
     pass
 
 
-async def missing_annotation_y(x: str, y) -> None:
+def unmapped_param_rofl(x: str, rofl: str) -> None:
     pass
 
 
-async def unmapped_param_rofl(x: str, rofl: str) -> None:
-    pass
+def type_check_fail_y(x: str, y: str) -> int:
+    return 0
 
 
-async def type_check_fail_y(x: str, y: str) -> None:
-    pass
-
-
-def not_async(x: str) -> None:
-    pass
+validator_check_multiple_registration: Validator[DataSetTest, SyncValidatorFunction] = Validator(
+    check_multiple_registration
+)
+validator_check_x_expensive: Validator[DataSetTest, AsyncValidatorFunction] = Validator(check_x_expensive)
+validator_check_y_positive: Validator[DataSetTest, AsyncValidatorFunction] = Validator(check_y_positive)
+validator_check_xy_ending: Validator[DataSetTest, AsyncValidatorFunction] = Validator(check_xy_ending)
+validator_check_required_and_optional: Validator[DataSetTest, SyncValidatorFunction] = Validator(
+    check_required_and_optional
+)
+validator_check_required_and_optional_with_utility: Validator[DataSetTest, SyncValidatorFunction] = Validator(
+    check_required_and_optional_with_utility
+)
+validator_check_with_param_info: Validator[DataSetTest, SyncValidatorFunction] = Validator(check_with_param_info)
+validator_check_with_param_info_fail: Validator[DataSetTest, SyncValidatorFunction] = Validator(
+    check_with_param_info_fail
+)
+validator_unprovided_but_required: Validator[DataSetTest, SyncValidatorFunction] = Validator(unprovided_but_required)
+validator_check_fail: Validator[DataSetTest, SyncValidatorFunction] = Validator(check_fail)
+validator_check_fail2: Validator[DataSetTest, SyncValidatorFunction] = Validator(check_fail2)
+validator_check_fail3: Validator[DataSetTest, SyncValidatorFunction] = Validator(check_fail3)
+validator_check_different_fails: Validator[DataSetTest, SyncValidatorFunction] = Validator(check_different_fails)
+validator_type_check_fail_y: Validator[DataSetTest, SyncValidatorFunction] = Validator(
+    type_check_fail_y  # type:ignore[arg-type]
+)
 
 
 class TestValidation:
-    async def test_generic_type(self):
-        """
-        This test ensures, that the data_set_type property works as expected.
-        """
-        validator_set = ValidatorSet[DataSetTest]()
-        assert validator_set.data_set_type == DataSetTest
-
-    async def test_generic_type_fail(self):
-        """
-        This test ensures, that the data_set_type property works as expected.
-        """
-        validator_set = ValidatorSet()  # type:ignore[var-annotated]
-        with pytest.raises(TypeError) as exc:
-            _ = validator_set.data_set_type
-
-        assert "You have to use an instance of ValidatorSet and define the generic type." == str(exc.value)
-
-    async def test_async_validation(self):
+    async def test_async_validation_and_result(self):
         """
         This test checks if the validation functions run concurrently by just ensuring that the expensive task
         (simulated with sleep) will finish always at last.
         """
         global finishing_order
         finishing_order = []
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_x_expensive, {"x": "x"})
-        validator_set.register(check_y_positive, {"y": "y"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_check_x_expensive, {"x": "x"}))
+        validation_manager.register(PathMappedValidator(validator_check_y_positive, {"y": "y"}))
+        validation_summary = await validation_manager.validate(dataset_instance)
+        assert validation_summary.total == 1
+        assert validation_summary.num_succeeds == 1
+        assert len(validation_summary.succeeded_data_sets) == 1
+        assert validation_summary.succeeded_data_sets[0] == dataset_instance
+        assert validation_summary.num_fails == 0
+        assert len(validation_summary.data_set_errors) == 0
         assert validation_summary.num_errors_total == 0
+        assert len(validation_summary.num_errors_per_id) == 0
         assert finishing_order == [check_y_positive, check_x_expensive]
 
     async def test_depend_validation(self):
         """
         This test checks if the feature to define a dependent check works properly.
         This is achieved by setting up a validation function depending on an expensive task. The expensive task
         should finish first.
         """
         global finishing_order
         finishing_order = []
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_x_expensive, {"x": "x"})
-        validator_set.register(check_multiple_registration, {"x": "x"})
-        validator_set.register(check_multiple_registration, {"x": "z.x"})
-        validator_set.register(
-            check_xy_ending,
-            {"x": "x", "y": "y"},
-            depends_on=[
-                check_x_expensive,
-                (check_multiple_registration, {"x": "x"}),
-                (check_multiple_registration, frozendict({"x": "z.x"})),
-            ],
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_check_x_expensive, {"x": "x"}))
+        validation_manager.register(
+            PathMappedValidator(validator_check_multiple_registration, {"x": "x"}),
         )
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager.register(
+            PathMappedValidator(validator_check_multiple_registration, {"x": "z.x"}),
+        )
+        validation_manager.register(
+            PathMappedValidator(validator_check_xy_ending, {"x": "x", "y": "y"}),
+            depends_on={
+                PathMappedValidator(validator_check_x_expensive, {"x": "x"}),
+                PathMappedValidator(validator_check_multiple_registration, {"x": "x"}),
+                PathMappedValidator(validator_check_multiple_registration, {"x": "z.x"}),
+            },
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
         assert finishing_order == [
             check_multiple_registration,
             check_multiple_registration,
             check_x_expensive,
             check_xy_ending,
         ]
 
     async def test_depend_and_async_validation(self):
         """
         This test is a mix of the previous two and checks if the finishing order is as expected.
         """
         global finishing_order
         finishing_order = []
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_x_expensive, {"x": "x"})
-        validator_set.register(check_y_positive, {"y": "y"})
-        validator_set.register(check_xy_ending, {"x": "x", "y": "y"}, depends_on=[check_x_expensive, check_y_positive])
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_check_x_expensive, {"x": "x"}))
+        validation_manager.register(PathMappedValidator(validator_check_y_positive, {"y": "y"}))
+        validation_manager.register(
+            PathMappedValidator(validator_check_xy_ending, {"x": "x", "y": "y"}),
+            depends_on={
+                PathMappedValidator(validator_check_x_expensive, {"x": "x"}),
+                PathMappedValidator(validator_check_y_positive, {"y": "y"}),
+            },
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
         assert finishing_order == [check_y_positive, check_x_expensive, check_xy_ending]
 
     async def test_failing_validation(self):
         """
         Tests if a failing validation behaves as expected.
         """
         global finishing_order
         finishing_order = []
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_y_positive, {"y": "y"})
-        validator_set.register(check_fail, {"x": "x"})
-        validator_set.register(check_fail2, {"y": "y"})
-        validator_set.register(check_fail3, {"y": "y"}, depends_on=[check_fail])
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_check_y_positive, {"y": "y"}))
+        validation_manager.register(PathMappedValidator(validator_check_fail, {"x": "x"}))
+        validation_manager.register(PathMappedValidator(validator_check_fail2, {"y": "y"}))
+        validation_manager.register(
+            PathMappedValidator(validator_check_fail3, {"y": "y"}),
+            depends_on={PathMappedValidator(validator_check_fail, {"x": "x"})},
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
 
         assert validation_summary.num_errors_total == 3
-        sub_exception_msgs = {str(exception) for exception in validation_summary.errors}
+        sub_exception_msgs = {str(exception) for exception in validation_summary.all_errors}
         assert any("I failed (on purpose! :O)" in sub_exception_msg for sub_exception_msg in sub_exception_msgs)
         assert any(
             "I failed (on purpose! :O - again :OOO)" in sub_exception_msg for sub_exception_msg in sub_exception_msgs
         )
         assert any(
             "Execution abandoned due to failing dependent validators" in sub_exception_msg
             for sub_exception_msg in sub_exception_msgs
@@ -233,153 +262,171 @@
                 {"x": "x", "y": "y"},
                 "The parameter y has no annotated type.",
                 id="Missing parameter type annotation",
             ),
             pytest.param(
                 unmapped_param_rofl,
                 {"x": "x"},
-                "The parameter list of the validator function must match the parameter_map. " "['x', 'rofl'] != ['x']",
+                "unmapped_param_rofl misses parameter(s) {'rofl'}",
                 id="Unmapped parameter",
             ),
-            pytest.param(
-                not_async,
-                {"x": "x"},
-                "The provided validator function has to be a coroutine (e.g. use async).",
-                id="Function not async",
-            ),
-            pytest.param(no_params, {}, "The validator function must take at least one argument.", id="No params"),
+            pytest.param(no_params, {}, "The validator function must take at least one argument", id="No params"),
         ],
     )
     async def test_illegal_validator_functions(
-        self, validator_func: ValidatorType, param_map: dict[str, str], expected_error: str
+        self, validator_func: ValidatorFunctionT, param_map: dict[str, str], expected_error: str
     ):
-        validator_set = ValidatorSet[DataSetTest]()
+        validation_manager = ValidationManager[DataSetTest]()
         with pytest.raises(ValueError) as error:
-            validator_set.register(validator_func, param_map)
+            validation_manager.register(PathMappedValidator(Validator(validator_func), param_map))
 
         assert str(error.value) == expected_error
 
     async def test_illegal_dependency_registration(self):
-        validator_set = ValidatorSet[DataSetTest]()
+        validation_manager = ValidationManager[DataSetTest]()
         with pytest.raises(ValueError) as exc:
-            validator_set.register(check_fail, {"x": "x"}, depends_on=[check_multiple_registration])
+            validation_manager.register(
+                PathMappedValidator(validator_check_fail, {"x": "x"}),
+                depends_on={PathMappedValidator(validator_check_multiple_registration, {"x": "x"})},
+            )
         assert "The specified dependency is not registered: check_multiple_registration" == str(exc.value)
 
-        validator_set.register(check_multiple_registration, {"x": "x"})
-        validator_set.register(check_multiple_registration, {"x": "z.x"})
-
-        with pytest.raises(ValueError) as exc:
-            validator_set.register(check_fail, {"x": "x"}, depends_on=[check_multiple_registration])
-        assert (
-            "The dependency check_multiple_registration got registered multiple times. You have "
-            "to define the parameter mapping for the dependency to resolve the ambiguity." == str(exc.value)
-        )
-
     @pytest.mark.parametrize(
-        ["validator_func", "param_map", "expected_error"],
+        ["validator", "param_map", "expected_error"],
         [
             pytest.param(
-                special_param_type_check_fail,
-                {"x": "x"},
-                "type of keys of _param_infos must be int; got str instead",
-                id="Special param wrong type",
-            ),
-            pytest.param(
-                type_check_fail_y,
+                validator_type_check_fail_y,
                 {"x": "x", "y": "y"},
                 "type of y must be str; got int instead",
                 id="Wrong parameter type",
             ),
         ],
     )
-    async def test_type_error(self, validator_func: ValidatorType, param_map: dict[str, str], expected_error: str):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(validator_func, param_map)
-        validation_summary = await validator_set.validate(dataset_instance)
+    async def test_type_error(
+        self, validator: Validator[DataSetTest, ValidatorFunctionT], param_map: dict[str, str], expected_error: str
+    ):
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator, param_map))
+        validation_summary = await validation_manager.validate(dataset_instance)
 
         assert validation_summary.num_errors_total == 1
-        assert expected_error in str(validation_summary.errors[0])
+        assert expected_error in str(validation_summary.all_errors[0])
 
     async def test_timeout(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_x_expensive, {"x": "x"}, timeout=timedelta(milliseconds=100))
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_x_expensive, {"x": "x"}),
+            timeout=timedelta(milliseconds=100),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 1
-        sub_exception_msgs = [str(exception) for exception in validation_summary.errors]
+        sub_exception_msgs = [str(exception) for exception in validation_summary.all_errors]
         assert "Timeout (0.1s) during execution" in sub_exception_msgs[0]
         assert "Validator function: check_x_expensive" in sub_exception_msgs[0]
 
     async def test_unprovided_but_required(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(unprovided_but_required, {"zz": "z.z"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_unprovided_but_required, {"zz": "z.z"}))
+        validation_summary = await validation_manager.validate(dataset_instance)
 
         assert validation_summary.num_errors_total == 1
-        assert "zz is required but not existent in the provided data set. Couldn't find z in DataSetTest.z." in str(
-            validation_summary.errors[0]
-        )
+        assert "'z.z' does not exist" in str(validation_summary.all_errors[0])
 
     async def test_multiple_validator_registration(self):
         global finishing_order
         finishing_order = []
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_multiple_registration, {"x": "x"})
-        validator_set.register(check_multiple_registration, {"x": "z.x"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_multiple_registration, {"x": "x"}),
+        )
+        validation_manager.register(
+            PathMappedValidator(validator_check_multiple_registration, {"x": "z.x"}),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
         assert len(finishing_order) == 2
 
-    async def test_map_special_param(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        with pytest.raises(ValueError) as error:
-            validator_set.register(check_with_param_info, {"x": "x", "zz": "z.z", "_param_infos": "y"})
-
-        assert "Special parameters cannot be mapped." in str(error.value)
-
     async def test_required_and_optional(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_required_and_optional, {"zx": "z.x", "zz": "z.z"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_required_and_optional, {"zx": "z.x", "zz": "z.z"}),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
 
     async def test_param_info(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_with_param_info, {"x": "x", "zz": "z.z"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_with_param_info, {"x": "x", "zz": "z.z"}),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
 
+    @staticmethod
+    def wrapper_without_self_for_coverage():
+        def more_call_stack():
+            param("x")
+
+        more_call_stack()
+
+    async def test_param_info_fail(self):
+        expected_error = "did not provide parameter information for parameter 'zz'"
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_with_param_info_fail, {}),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
+        assert any(expected_error in str(error) for error in validation_summary.all_errors)
+        with pytest.raises(RuntimeError) as error:
+            param("x")
+        assert (
+            "You can call this function only directly from inside a function "
+            "which is executed by the validation framework" == str(error.value)
+        )
+        with pytest.raises(RuntimeError) as error:
+            TestValidation.wrapper_without_self_for_coverage()
+        assert (
+            "You can call this function only directly from inside a function "
+            "which is executed by the validation framework" == str(error.value)
+        )
+
     async def test_error_ids(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_fail, {"x": "x"})
-        validator_set.register(check_fail2, {"y": "y"})
-        validator_set.register(check_fail3, {"y": "y"}, depends_on=[check_fail])
-        validator_set.register(check_different_fails, {"x": "x"})
-        validator_set.register(check_different_fails, {"x": "z.x"})
-        validation_summary = await validator_set.validate(dataset_instance)
-        validation_summary2 = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(PathMappedValidator(validator_check_fail, {"x": "x"}))
+        validation_manager.register(PathMappedValidator(validator_check_fail2, {"y": "y"}))
+        validation_manager.register(
+            PathMappedValidator(validator_check_fail3, {"y": "y"}),
+            depends_on={PathMappedValidator(validator_check_fail, {"x": "x"})},
+        )
+        validation_manager.register(PathMappedValidator(validator_check_different_fails, {"x": "x"}))
+        validation_manager.register(PathMappedValidator(validator_check_different_fails, {"x": "z.x"}))
+        validation_summary = await validation_manager.validate(dataset_instance)
+        validation_summary2 = await validation_manager.validate(dataset_instance)
         # This is just to ensure that the ID generation for the errors is not completely random and has consistency
 
-        sub_exceptions1: dict[_ValidatorMapInternIndexType, ValidationError] = {
-            exception.validator: exception for exception in validation_summary.errors
+        sub_exceptions1: dict[MappedValidatorT, ValidationError] = {
+            exception.mapped_validator: exception for exception in validation_summary.all_errors
         }
-        sub_exceptions2: dict[_ValidatorMapInternIndexType, ValidationError] = {
-            exception.validator: exception for exception in validation_summary2.errors
+        sub_exceptions2: dict[MappedValidatorT, ValidationError] = {
+            exception.mapped_validator: exception for exception in validation_summary2.all_errors
         }
         assert len(sub_exceptions1) == 5
         # This is a self-consistency check to ensure that there is no unwanted randomness in the program.
         assert {str(sub_exception1) for sub_exception1 in sub_exceptions1.values()} == {
             str(sub_exception2) for sub_exception2 in sub_exceptions2.values()
         }
         # Different errors in the same function should get different error IDs.
         assert (
-            sub_exceptions1[check_different_fails, frozendict({"x": "x"})].error_id
-            != sub_exceptions1[check_different_fails, frozendict({"x": "z.x"})].error_id
+            sub_exceptions1[PathMappedValidator(validator_check_different_fails, {"x": "x"})].error_id
+            != sub_exceptions1[PathMappedValidator(validator_check_different_fails, {"x": "z.x"})].error_id
         )
         # This ensures that the ID is constant across python sessions - as long as the line number of the raising
         # exception in `check_fail` doesn't change.
-        assert sub_exceptions1[check_fail, frozendict({"x": "x"})].error_id == 47799448
+        assert sub_exceptions1[PathMappedValidator(validator_check_fail, {"x": "x"})].error_id == 47799448
 
     async def test_utility_required_and_optional(self):
-        validator_set = ValidatorSet[DataSetTest]()
-        validator_set.register(check_required_and_optional_with_utility, {"z": "z"})
-        validation_summary = await validator_set.validate(dataset_instance)
+        validation_manager = ValidationManager[DataSetTest]()
+        validation_manager.register(
+            PathMappedValidator(validator_check_required_and_optional_with_utility, {"z": "z"}),
+        )
+        validation_summary = await validation_manager.validate(dataset_instance)
         assert validation_summary.num_errors_total == 0
```

