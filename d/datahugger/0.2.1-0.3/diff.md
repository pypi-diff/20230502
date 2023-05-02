# Comparing `tmp/datahugger-0.2.1.tar.gz` & `tmp/datahugger-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datahugger-0.2.1.tar", last modified: Tue Feb 28 19:53:11 2023, max compression
+gzip compressed data, was "datahugger-0.3.tar", last modified: Tue May  2 15:13:45 2023, max compression
```

## Comparing `datahugger-0.2.1.tar` & `datahugger-0.3.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.276194 datahugger-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-28 19:52:59.000000 datahugger-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.260193 datahugger-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.268194 datahugger-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-28 19:52:59.000000 datahugger-0.2.1/.github/ISSUE_TEMPLATE/request-support-for-data-repository.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.268194 datahugger-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-28 19:52:59.000000 datahugger-0.2.1/.github/workflows/gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-28 19:52:59.000000 datahugger-0.2.1/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-28 19:52:59.000000 datahugger-0.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-28 19:52:59.000000 datahugger-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-28 19:52:59.000000 datahugger-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-28 19:52:59.000000 datahugger-0.2.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-28 19:52:59.000000 datahugger-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-02-28 19:53:11.276194 datahugger-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-02-28 19:52:59.000000 datahugger-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.268194 datahugger-0.2.1/datahugger/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.268194 datahugger-0.2.1/datahugger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-28 19:53:11.000000 datahugger-0.2.1/datahugger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger_repocard_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-02-28 19:52:59.000000 datahugger-0.2.1/datahugger_repocard_tagline.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.272194 datahugger-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/download.md
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.272194 datahugger-0.2.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/images/datahugger_architecture.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    19088 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/images/datahugger_architecture.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/images/datahugger_repo.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1320618 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/images/logos.ai
--rw-r--r--   0 runner    (1001) docker     (123)   508124 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/images/logos.png
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/object.md
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/options.md
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/repositories.md
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/repositories_not_supported.md
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/reproducible.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.272194 datahugger-0.2.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-02-28 19:52:59.000000 datahugger-0.2.1/docs/working.md
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-28 19:52:59.000000 datahugger-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-28 19:52:59.000000 datahugger-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.276194 datahugger-0.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-28 19:52:59.000000 datahugger-0.2.1/scripts/datacite_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-28 19:52:59.000000 datahugger-0.2.1/scripts/estimate_repos_supported.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 19:53:11.276194 datahugger-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 19:53:11.276194 datahugger-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-28 19:52:59.000000 datahugger-0.2.1/tests/test_dataset_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-02-28 19:52:59.000000 datahugger-0.2.1/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-28 19:52:59.000000 datahugger-0.2.1/tests/test_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-28 19:52:59.000000 datahugger-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.825730 datahugger-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.825730 datahugger-0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-02 15:13:32.000000 datahugger-0.3/.github/ISSUE_TEMPLATE/request-support-for-data-repository.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.829730 datahugger-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-02 15:13:32.000000 datahugger-0.3/.github/workflows/gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 15:13:32.000000 datahugger-0.3/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-02 15:13:32.000000 datahugger-0.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-02 15:13:32.000000 datahugger-0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-02 15:13:32.000000 datahugger-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-02 15:13:32.000000 datahugger-0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 15:13:32.000000 datahugger-0.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 15:13:32.000000 datahugger-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-02 15:13:45.833731 datahugger-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-02 15:13:32.000000 datahugger-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.829730 datahugger-0.3/datahugger/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.829730 datahugger-0.3/datahugger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 15:13:45.000000 datahugger-0.3/datahugger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger_repocard_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-05-02 15:13:32.000000 datahugger-0.3/datahugger_repocard_tagline.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.829730 datahugger-0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 15:13:32.000000 datahugger-0.3/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 15:13:32.000000 datahugger-0.3/docs/download.md
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-02 15:13:32.000000 datahugger-0.3/docs/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-02 15:13:32.000000 datahugger-0.3/docs/images/datahugger_architecture.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    19088 2023-05-02 15:13:32.000000 datahugger-0.3/docs/images/datahugger_architecture.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14377 2023-05-02 15:13:32.000000 datahugger-0.3/docs/images/datahugger_repo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1320618 2023-05-02 15:13:32.000000 datahugger-0.3/docs/images/logos.ai
+-rw-r--r--   0 runner    (1001) docker     (123)   508124 2023-05-02 15:13:32.000000 datahugger-0.3/docs/images/logos.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-02 15:13:32.000000 datahugger-0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:13:32.000000 datahugger-0.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 15:13:32.000000 datahugger-0.3/docs/object.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-02 15:13:32.000000 datahugger-0.3/docs/options.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-02 15:13:32.000000 datahugger-0.3/docs/repositories.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-02 15:13:32.000000 datahugger-0.3/docs/repositories_not_supported.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-02 15:13:32.000000 datahugger-0.3/docs/reproducible.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 15:13:32.000000 datahugger-0.3/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-02 15:13:32.000000 datahugger-0.3/docs/working.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    79184 2023-05-02 15:13:32.000000 datahugger-0.3/examples/example_datahugger_in_workflow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-02 15:13:32.000000 datahugger-0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 15:13:32.000000 datahugger-0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 15:13:32.000000 datahugger-0.3/scripts/datacite_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-02 15:13:32.000000 datahugger-0.3/scripts/estimate_repos_supported.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:13:45.833731 datahugger-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:13:45.833731 datahugger-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-02 15:13:32.000000 datahugger-0.3/tests/test_dataset_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-02 15:13:32.000000 datahugger-0.3/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-02 15:13:32.000000 datahugger-0.3/tests/test_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 15:13:32.000000 datahugger-0.3/tests/test_utils.py
```

### Comparing `datahugger-0.2.1/.github/workflows/python-package.yml` & `datahugger-0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/.github/workflows/python-publish.yml` & `datahugger-0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/.gitignore` & `datahugger-0.3/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -123,7 +123,9 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+examples/data/
```

### Comparing `datahugger-0.2.1/LICENSE` & `datahugger-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/PKG-INFO` & `datahugger-0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,18 @@
-Metadata-Version: 2.1
-Name: datahugger
-Version: 0.2.1
-Summary: One downloader for many scientific data and code repositories!
-Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: docs
-License-File: LICENSE
-
 <p align="center">
   <img alt="Datahugger - Where DOI hugs Data" src="https://github.com/J535D165/datahugger/raw/main/datahugger_repocard_tagline.svg">
 </p>
 
 # Datahugger - Where DOI :open_hands: Data
 
 Datahugger is a tool to download scientific datasets, software, and code from a large number of repositories based on their DOI [(wiki)](https://en.wikipedia.org/wiki/Digital_object_identifier) or URL. With Datahugger, you can automate the downloading of data and improve the reproducibility of your research. Datahugger provides a straightforward [Python interface](#download-with-python) as well as an intuitive [Command Line Interface](#download-with-command-line) (CLI).
 
 ## Supported repositories
 
-Datahugger offers support for more than [<!-- count -->226<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
+Datahugger offers support for more than [<!-- count -->350<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
 
 [![Datahugger support Zenodo, Dataverse, DataOne, GitHub, FigShare, HuggingFace, Mendeley Data, Dryad, OSF, and many more](https://github.com/J535D165/datahugger/raw/main/docs/images/logos.png)](https://j535d165.github.io/datahugger/repositories)
 
 We are still expanding Datahugger with support for more repositories. You can
 help by [requesting support for a repository](https://github.com/J535D165/datahugger/issues/new/choose) in the issue
 tracker. Pull Requests are very welcome as well.
 
@@ -45,57 +24,61 @@
 
 ```
 pip install datahugger
 ```
 
 ## Getting started
 
-### Download with Python
+### Datahugger with Python
 
 Load a dataset (or any digital asset) from a repository with the
-`datahugger.load_repository` function. The first argument is the DOI or URL
+`datahugger.get()` function. The first argument is the DOI or URL
 and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
+The following code loads dataset [10.5061/dryad.mj8m0](https://doi.org/10.5061/dryad.mj8m0) into
+the folder `data`. 
+
 ```python
 import datahugger
 
-# download the data to your device
-datahugger.get("10.5061/dryad.x3ffbg7m8", "data")
+# download the dataset to the folder "data"
+datahugger.get("10.5061/dryad.mj8m0", "data")
 ```
 
-The data from DOI [10.5061/dryad.x3ffbg7m8](https://doi.org/10.5061/dryad.x3ffbg7m8) is now stored in the folder `data`. The data can now be accessed and analyzed. For example:
-
-```python
-
-import pandas as pd
-
-df = pd.read_csv("data/Pfaller_Robinson_2022_Global_Sea_Turtle_Epibiont_Database.csv")
-print(df["Higher Taxon"].value_counts())
-```
+For an example how this can integrate with your work, see the 
+[example workflow notebook](https://github.com/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb) or 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb)
 
 
-### Download with command line
+### Datahugger with command line
 
 The command line function `datahugger` provides an easy interface to download data. The first
 argument is the DOI or URL and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
 ```bash
-datahugger 10.5061/dryad.31zcrjdm5 data
+datahugger 10.5061/dryad.mj8m0 data
 ```
 
 ```bash
-% datahugger 10.5061/dryad.x3ffbg7m8 data
-README_Pfaller_Robinson_20[...].txt: 100%|█████████████████████████████████████| 17.1k/17.1k [00:00<00:00, 2.62MB/s]
-Pfaller_Robinson_2022_Glob[...].csv: 100%|████████████████████████████████████████| 709k/709k [00:00<00:00, 904kB/s]
-Repository content successfully downloaded.
+% datahugger 10.5061/dryad.mj8m0 data
+Collecting...
+NestTemperatureData.csv            : 100%|████████████████████████████████████████| 607k/607k
+README_for_NestTemperatureData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+ExternalTemps.csv                  : 100%|██████████████████████████████████████| 1.06k/1.06k
+README_for_ExternalTemps.txt       : 100%|██████████████████████████████████████| 2.82k/2.82k
+InternalEggTempData.csv            : 100%|██████████████████████████████████████████| 664/664
+README_for_InternalEggTempData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+SoilSimulation_Output.csv          : 100%|████████████████████████████████████████| 229M/229M
+README_for_SoilSimulation_[...].txt: 100%|██████████████████████████████████████| 2.82k/2.82k
+Dataset successfully downloaded.
 ```
 
-**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.31zcrjdm5" data`. 
+**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.mj8m0" data`. 
 
 ## Tips and tricks
 
 - No need to struggle with DOIs versus DOI URLs. They both work (and more). Example: The values `10.5061/dryad.x3ffbg7m8`, `doi:10.5061/dryad.x3ffbg7m8`, [`https://doi.org/10.5061/dryad.x3ffbg7m8`](https://doi.org/10.5061/dryad.x3ffbg7m8), and [`https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8`](https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8) all point to the same dataset.
 - Do not republish the dataset when you are uploading your data to an scientific data repository. These storages resources can be used better :)
 
 ## License
```

### Comparing `datahugger-0.2.1/README.md` & `datahugger-0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,39 @@
+Metadata-Version: 2.1
+Name: datahugger
+Version: 0.3
+Summary: One downloader for many scientific data and code repositories!
+Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: docs
+License-File: LICENSE
+
 <p align="center">
   <img alt="Datahugger - Where DOI hugs Data" src="https://github.com/J535D165/datahugger/raw/main/datahugger_repocard_tagline.svg">
 </p>
 
 # Datahugger - Where DOI :open_hands: Data
 
 Datahugger is a tool to download scientific datasets, software, and code from a large number of repositories based on their DOI [(wiki)](https://en.wikipedia.org/wiki/Digital_object_identifier) or URL. With Datahugger, you can automate the downloading of data and improve the reproducibility of your research. Datahugger provides a straightforward [Python interface](#download-with-python) as well as an intuitive [Command Line Interface](#download-with-command-line) (CLI).
 
 ## Supported repositories
 
-Datahugger offers support for more than [<!-- count -->226<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
+Datahugger offers support for more than [<!-- count -->350<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
 
 [![Datahugger support Zenodo, Dataverse, DataOne, GitHub, FigShare, HuggingFace, Mendeley Data, Dryad, OSF, and many more](https://github.com/J535D165/datahugger/raw/main/docs/images/logos.png)](https://j535d165.github.io/datahugger/repositories)
 
 We are still expanding Datahugger with support for more repositories. You can
 help by [requesting support for a repository](https://github.com/J535D165/datahugger/issues/new/choose) in the issue
 tracker. Pull Requests are very welcome as well.
 
@@ -24,57 +45,61 @@
 
 ```
 pip install datahugger
 ```
 
 ## Getting started
 
-### Download with Python
+### Datahugger with Python
 
 Load a dataset (or any digital asset) from a repository with the
-`datahugger.load_repository` function. The first argument is the DOI or URL
+`datahugger.get()` function. The first argument is the DOI or URL
 and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
+The following code loads dataset [10.5061/dryad.mj8m0](https://doi.org/10.5061/dryad.mj8m0) into
+the folder `data`. 
+
 ```python
 import datahugger
 
-# download the data to your device
-datahugger.get("10.5061/dryad.x3ffbg7m8", "data")
+# download the dataset to the folder "data"
+datahugger.get("10.5061/dryad.mj8m0", "data")
 ```
 
-The data from DOI [10.5061/dryad.x3ffbg7m8](https://doi.org/10.5061/dryad.x3ffbg7m8) is now stored in the folder `data`. The data can now be accessed and analyzed. For example:
-
-```python
-
-import pandas as pd
-
-df = pd.read_csv("data/Pfaller_Robinson_2022_Global_Sea_Turtle_Epibiont_Database.csv")
-print(df["Higher Taxon"].value_counts())
-```
+For an example how this can integrate with your work, see the 
+[example workflow notebook](https://github.com/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb) or 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb)
 
 
-### Download with command line
+### Datahugger with command line
 
 The command line function `datahugger` provides an easy interface to download data. The first
 argument is the DOI or URL and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
 ```bash
-datahugger 10.5061/dryad.31zcrjdm5 data
+datahugger 10.5061/dryad.mj8m0 data
 ```
 
 ```bash
-% datahugger 10.5061/dryad.x3ffbg7m8 data
-README_Pfaller_Robinson_20[...].txt: 100%|█████████████████████████████████████| 17.1k/17.1k [00:00<00:00, 2.62MB/s]
-Pfaller_Robinson_2022_Glob[...].csv: 100%|████████████████████████████████████████| 709k/709k [00:00<00:00, 904kB/s]
-Repository content successfully downloaded.
+% datahugger 10.5061/dryad.mj8m0 data
+Collecting...
+NestTemperatureData.csv            : 100%|████████████████████████████████████████| 607k/607k
+README_for_NestTemperatureData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+ExternalTemps.csv                  : 100%|██████████████████████████████████████| 1.06k/1.06k
+README_for_ExternalTemps.txt       : 100%|██████████████████████████████████████| 2.82k/2.82k
+InternalEggTempData.csv            : 100%|██████████████████████████████████████████| 664/664
+README_for_InternalEggTempData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+SoilSimulation_Output.csv          : 100%|████████████████████████████████████████| 229M/229M
+README_for_SoilSimulation_[...].txt: 100%|██████████████████████████████████████| 2.82k/2.82k
+Dataset successfully downloaded.
 ```
 
-**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.31zcrjdm5" data`. 
+**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.mj8m0" data`. 
 
 ## Tips and tricks
 
 - No need to struggle with DOIs versus DOI URLs. They both work (and more). Example: The values `10.5061/dryad.x3ffbg7m8`, `doi:10.5061/dryad.x3ffbg7m8`, [`https://doi.org/10.5061/dryad.x3ffbg7m8`](https://doi.org/10.5061/dryad.x3ffbg7m8), and [`https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8`](https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8) all point to the same dataset.
 - Do not republish the dataset when you are uploading your data to an scientific data repository. These storages resources can be used better :)
 
 ## License
```

### Comparing `datahugger-0.2.1/datahugger/__main__.py` & `datahugger-0.3/datahugger/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     )
 
     # version
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version="%(prog)s {version}".format(version=__version__),
+        version=f"%(prog)s {__version__}",
     )
 
     args, _ = parser.parse_known_args()
 
     logging.basicConfig(level=args.log_level)
 
     if args.progress:
```

### Comparing `datahugger-0.2.1/datahugger/api.py` & `datahugger-0.3/datahugger/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import requests
 
 from datahugger.exceptions import DOIError
 from datahugger.services import DataDryadDataset
 from datahugger.services import DataOneDataset
 from datahugger.services import DataverseDataset
+from datahugger.services import Djehuty
+from datahugger.services import DSpaceDataset
 from datahugger.services import FigShareDataset
 from datahugger.services import GitHubDataset
 from datahugger.services import HuggingFaceDataset
 from datahugger.services import MendeleyDataset
 from datahugger.services import OSFDataset
 from datahugger.services import ZenodoDataset
 from datahugger.utils import _is_doi
@@ -29,15 +31,16 @@
     "github.com": GitHubDataset,
     "datadryad.org": DataDryadDataset,
     "huggingface.co": HuggingFaceDataset,
     "osf.io": OSFDataset,
     "data.mendeley.com": MendeleyDataset,
     # Figshare download
     "figshare.com": FigShareDataset,
-    "data.4tu.nl": FigShareDataset,
+    # Djehuty
+    "data.4tu.nl": Djehuty,
     # DataOne repositories
     "arcticdata.io": DataOneDataset,
     "knb.ecoinformatics.org": DataOneDataset,
     "data.pndb.fr": DataOneDataset,
     "opc.dataone.org": DataOneDataset,
     "portal.edirepository.org": DataOneDataset,
     "goa.nceas.ucsb.edu": DataOneDataset,
@@ -123,15 +126,18 @@
     "ssri.is": DataverseDataset,
     "trolling.uit.no": DataverseDataset,
     "www.sodha.be": DataverseDataset,
     "www.uni-hildesheim.de": DataverseDataset,
 }
 
 # regexp lookup
-SERVICES_NETLOC_REGEXP = {r".*\.figshare\.com": FigShareDataset}
+SERVICES_NETLOC_REGEXP = {
+    r".*\/articles\/.*\/.*\/\d+": FigShareDataset,
+    r".*\/handle\/\d+\/\d+": DSpaceDataset,
+}
 
 RE3DATA_SOFTWARE = {
     "DataVerse": DataverseDataset,  # Hits on re3data 2022-09-02: (145)
     # "DSpace": DSpaceDataset,  # Hits on re3data 2022-09-02: (115)
     # "CKAN": CKANDataset,  # Hits on re3data 2022-09-02: (89)
     # "MySQL": MySQLDataset,  # Hits on re3data 2022-09-02: (86)
     # "Fedora": FedoraDataset,  # Hits on re3data 2022-09-02: (43)
@@ -148,15 +154,14 @@
     url,
     doi=None,
     max_file_size=None,
     force_download=False,
     unzip=True,
     progress=True,
     print_only=False,
-    *args,
     **kwargs,
 ):
 
     # check if the url is a doi, if so, make a proper doi url out of it.
     if url.startswith("doi:"):
         url = url[4:]
 
@@ -170,32 +175,34 @@
     # is url
     uri = urlparse(url)
 
     # if netloc is doi.org, follow the redirect
     if uri.hostname in URL_RESOLVE:
 
         r = requests.head(url, allow_redirects=True)
-        if r.status_code == 404:
+        if r.status_code == 404 and r.url and r.url.startswith("https://doi.org"):
             raise DOIError(
                 f"DOI cannot be found in the DOI System, see https://doi.org/{doi}"
             )
-        if r.status_code != 200:
-            raise ValueError("Error")
+        elif r.status_code == 405:
+            # head request not allowed, try get request
+            r = requests.get(url, allow_redirects=True)
+        else:
+            r.raise_for_status()
 
         logging.info(f"Redirect from {url} to {r.url}")
 
         return _base_request(
             r.url,
             max_file_size=max_file_size,
             doi=doi,
             force_download=force_download,
             unzip=unzip,
             progress=progress,
             print_only=print_only,
-            *args,
             **kwargs,
         )
 
     service_class = _resolve_service(url, doi)
 
     if service_class is None:
         raise ValueError(f"Data service for {url} is not supported.")
@@ -206,29 +213,27 @@
         url,
         base_url=get_base_url(url),
         max_file_size=max_file_size,
         force_download=force_download,
         unzip=unzip,
         progress=progress,
         print_only=print_only,
-        *args,
         **kwargs,
     )
 
 
 def get(
     url,
     output_folder,
     doi=None,
     max_file_size=None,
     force_download=False,
     unzip=True,
     progress=True,
     print_only=False,
-    *args,
     **kwargs,
 ):
     """Get the content of repository.
 
     Download the content of the dataset to a local folder. Provide a
     URL or DOI to the dataset in the data repository.
 
@@ -262,23 +267,21 @@
         url,
         doi=doi,
         max_file_size=max_file_size,
         force_download=force_download,
         unzip=unzip,
         progress=progress,
         print_only=print_only,
-        *args,
         **kwargs,
     ).download(output_folder, doi=doi)
 
 
 def info(
     url,
     doi=None,
-    *args,
     **kwargs,
 ):
     """Get info on the content of the dataset.
 
     Arguments
     ---------
     url: str, pathlib.Path
@@ -289,15 +292,14 @@
 
     datahugger.base.DatasetDownloader
         The dataset download object for the specific service.
     """
     b = _base_request(
         url,
         doi=doi,
-        *args,
         **kwargs,
     )
 
     # collect the files
     logging.info(b.files)
 
     return b
@@ -327,15 +329,15 @@
     logging.debug(f"Resolve service: search netloc '{uri.hostname}'")
     if uri.hostname in SERVICES_NETLOC.keys():
         logging.debug("Service found: " + uri.hostname)
 
         return SERVICES_NETLOC[uri.hostname]
 
     for netloc_re, service in SERVICES_NETLOC_REGEXP.items():
-        if re.match(netloc_re, uri.hostname):
+        if re.match(netloc_re, url):
             return service
 
 
 def _resolve_service_with_re3data(doi):
 
     publisher = get_datapublisher_from_doi(doi)
     logging.debug(f"Publisher of dataset: {publisher}")
```

### Comparing `datahugger-0.2.1/datahugger/base.py` & `datahugger-0.3/datahugger/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import os
 import re
 import zipfile
 from pathlib import Path
 from typing import Union
 
-from jsonpath_ng import parse
 import natsort as ns
 import requests
+from jsonpath_ng import parse
 from scitree import scitree
 from tqdm import tqdm
 
 from datahugger.utils import _format_filename
 from datahugger.utils import _is_url
 
 FILE_RANKING = [
@@ -32,15 +32,15 @@
         prio = len(FILE_RANKING)
 
     x = (prio,) + ns.natsort_keygen(alg=alg)(f)
 
     return x
 
 
-class DatasetResult(object):
+class DatasetResult:
     """Result class after downloading the dataset."""
 
     def __str__(self):
 
         return f"<{self.__class__.__name__} n_files={len(self)} >"
 
     def __len__(self):
@@ -52,29 +52,31 @@
 
         Tree based on scientific sort.
         """
 
         return scitree(self.output_folder, **kwargs)
 
 
-class DatasetDownloader(object):
+class DatasetDownloader:
     """Base class for downloading resources from repositories."""
 
+    API_URL = None
+
     def __init__(
         self,
         url: Union[str, int],
         version=None,
         base_url=None,
         max_file_size=None,
         force_download=False,
         progress=True,
         unzip=True,
         print_only=False,
     ):
-        super(DatasetDownloader, self).__init__()
+        super().__init__()
         self.url = url
         self.version = version
         self.base_url = base_url
         self.max_file_size = max_file_size
         self.force_download = force_download
         self.progress = progress
         self.unzip = unzip
@@ -170,21 +172,21 @@
 
         """
         if (
             file_size is not None
             and self.max_file_size is not None
             and file_size >= self.max_file_size
         ):
-            logging.info("Skipping large file {}".format(file_link))
+            logging.info(f"Skipping large file {file_link}")
             if self.progress:
-                print("{}: SKIPPED".format(_format_filename(file_name)))
+                print(f"{_format_filename(file_name)}: SKIPPED")
             return
 
         if not self.print_only:
-            logging.info("Downloading file {}".format(file_link))
+            logging.info(f"Downloading file {file_link}")
             res = requests.get(file_link, stream=True)
 
             output_fp = Path(output_folder, file_name)
             Path(output_fp).parent.mkdir(parents=True, exist_ok=True)
 
             if not self.force_download and output_fp.exists():
                 print("File already exists:", file_name)
@@ -193,22 +195,23 @@
             if self.progress:
                 with tqdm.wrapattr(
                     open(output_fp, "wb"),
                     "write",
                     miniters=1,
                     desc=_format_filename(file_name),
                     total=int(res.headers.get("content-length", 0)),
+                    bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt}",
                 ) as fout:
                     for chunk in res.iter_content(chunk_size=4096):
                         fout.write(chunk)
             else:
                 with open(output_fp, "wb") as f:
                     f.write(res.content)
         else:
-            print("{}: COMPLETE".format(_format_filename(file_name)))
+            print(f"{_format_filename(file_name)}: COMPLETE")
 
     def _parse_url(self, url):
         if not isinstance(url, str) or not _is_url(url):
             raise ValueError("Not a valid URL.")
 
         # first try to parse with version number
         if hasattr(self, "REGEXP_ID_AND_VERSION"):
@@ -222,15 +225,15 @@
         # then try to parse without version number
         if hasattr(self, "REGEXP_ID"):
             match = re.search(self.REGEXP_ID, url)
 
             if match and match.group(1):
                 return match.group(1), None
 
-        return None, None
+        raise ValueError(f"Failed to parse record identifier from URL '{url}'")
 
     def _unpack_single_folder(self, zip_url, output_folder):
 
         r = requests.get(zip_url)
         z = zipfile.ZipFile(io.BytesIO(r.content))
 
         for zip_info in z.infolist():
@@ -253,63 +256,79 @@
         return self._api_record_id
 
     def _pre_files(self):
         pass
 
     def _get_files_recursive(self, url, folder_name=None):
 
+        if not isinstance(url, str):
+            ValueError(f"Expected url to be string type, got {type(url)}")
+
         result = []
 
         # get the data from URL
         res = requests.get(url)
+        reponse = res.json()
 
         # find path to raw files
         if hasattr(self, "META_FILES_JSONPATH"):
             jsonpath_expression = parse(self.META_FILES_JSONPATH)
-            files_raw = jsonpath_expression.find(res.json())[0].value
+            files_raw = jsonpath_expression.find(reponse)[0].value
         else:
-            files_raw = res.json()
+            files_raw = reponse
 
         for f in files_raw:
 
             # create the file or folder path
             if folder_name is None:
                 f_path = self._get_attr_name(f)
             else:
                 f_path = str(Path(folder_name, self._get_attr_name(f)))
 
             if self._get_attr_kind(f) == "folder":
 
                 result.extend(
-                    self._get_files_recursive(self._get_attr_link(f), folder_name=f_path)
+                    self._get_files_recursive(
+                        self._get_attr_link(f), folder_name=f_path)
                 )
             else:
 
                 result.append(
                     {
                         "link": self._get_attr_link(f),
                         "name": f_path,
                         "size": self._get_attr_size(f),
                         "hash": self._get_attr_hash(f),
                         "hash_type": self._get_attr_hash_type(f),
                     }
                 )
 
+        if hasattr(self, "PAGINATION_JSONPATH"):
+            jsonpath_expression = parse(self.PAGINATION_JSONPATH)
+            next_url = jsonpath_expression.find(reponse)[0].value
+
+            if next_url:
+                result.extend(
+                    self._get_files_recursive(
+                        next_url, folder_name=folder_name)
+                )
+
         return result
 
     @property
     def files(self):
 
         if hasattr(self, "_files"):
             return self._files
 
         self._pre_files()
 
         self._files = self._get_files_recursive(
             self.API_URL_META.format(
+                api_url=self.API_URL,
                 api_record_id=self.api_record_id,
                 version=self.version,
                 base_url=self.base_url,
             )
         )
 
         return self._files
```

### Comparing `datahugger-0.2.1/datahugger/deprecated.py` & `datahugger-0.3/datahugger/deprecated.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     output_folder,
     doi=None,
     max_file_size=None,
     force_download=False,
     unzip=True,
     progress=True,
     print_only=False,
-    *args,
     **kwargs,
 ):
     """Load repository is deprecated.
 
     Use datahugger.get() instead.
     """
     return get(
@@ -22,10 +21,9 @@
         output_folder,
         doi=doi,
         max_file_size=max_file_size,
         force_download=force_download,
         unzip=unzip,
         progress=progress,
         print_only=print_only,
-        *args,
         **kwargs,
     )
```

### Comparing `datahugger-0.2.1/datahugger/services.py` & `datahugger-0.3/datahugger/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import io
 import xml.etree.ElementTree as ET
 import zipfile
 from pathlib import Path
 from typing import Union
 from urllib.parse import quote
 
-from jsonpath_ng import parse
 import requests
+from jsonpath_ng import parse
 
 from datahugger.base import DatasetDownloader
 from datahugger.base import DatasetResult
 
 
 class ZenodoDataset(DatasetDownloader, DatasetResult):
     """Downloader for Zenodo repository.
@@ -20,15 +20,15 @@
 
     REGEXP_ID = r"zenodo\.org\/record\/(\d+).*"
 
     # the base entry point of the REST API
     API_URL = "https://zenodo.org/api/"
 
     # the files and metadata about the dataset
-    API_URL_META = API_URL + "records/{api_record_id}"
+    API_URL_META = "{api_url}records/{api_record_id}"
     META_FILES_JSONPATH = "files"
 
     # paths to file attributes
     ATTR_NAME_JSONPATH = "key"
     ATTR_FILE_LINK_JSONPATH = "links.self"
     ATTR_SIZE_JSONPATH = "size"
     ATTR_HASH_JSONPATH = "checksum"
@@ -67,43 +67,55 @@
             self.base_url, record["dataFile"]["id"]
         )
 
 
 class FigShareDataset(DatasetDownloader, DatasetResult):
     """Downloader for FigShare repository."""
 
-    REGEXP_ID_AND_VERSION = r"articles\/dataset\/.*\/(\d+)\/(\d+)"
-    REGEXP_ID = r"articles\/dataset\/.*\/(\d+)"
+    REGEXP_ID_AND_VERSION = r"articles\/.*\/.*\/(\d+)\/(\d+)"
+    REGEXP_ID = r"articles\/.*\/.*\/(\d+)"
 
     # the base entry point of the REST API
     API_URL = "https://api.figshare.com/v2"
 
     # the files and metadata about the dataset
-    API_URL_META = API_URL + "/articles/{api_record_id}/files"
+    API_URL_META = "{api_url}/articles/{api_record_id}/files"
 
     # paths to file attributes
     ATTR_FILE_LINK_JSONPATH = "download_url"
     ATTR_NAME_JSONPATH = "name"
     ATTR_SIZE_JSONPATH = "size"
     ATTR_HASH_JSONPATH = "computed_md5"
     ATTR_HASH_TYPE_VALUE = "md5"
 
 
+class Djehuty(FigShareDataset):
+    """Downloader for Djehuty repository."""
+
+    REGEXP_ID_AND_VERSION = r"articles\/.*\/(\d+)\/(\d+)"
+    REGEXP_ID = r"articles\/.*\/(\d+)"
+
+    # the base entry point of the REST API
+    API_URL = "https://data.4tu.nl/v2"
+
+
 class OSFDataset(DatasetDownloader, DatasetResult):
     """Downloader for OSF repository."""
 
     REGEXP_ID = r"osf\.io\/(.*)/"
 
     # the base entry point of the REST API
     API_URL = "https://api.osf.io/v2/registrations/"
 
     # the files and metadata about the dataset
-    API_URL_META = API_URL + "{api_record_id}/files/osfstorage/?format=jsonapi"
+    API_URL_META = "{api_url}{api_record_id}/files/osfstorage/?format=jsonapi"
     META_FILES_JSONPATH = "data"
 
+    PAGINATION_JSONPATH = "links.next"
+
     # paths to file attributes
     ATTR_KIND_JSONPATH = "attributes.kind"
 
     ATTR_FILE_LINK_JSONPATH = "links.download"
     ATTR_FOLDER_LINK_JSONPATH = "relationships.files.links.related.href"
 
     ATTR_NAME_JSONPATH = "attributes.name"
@@ -204,43 +216,75 @@
                     }
                 )
 
         self._files = x
         return self._files
 
 
+class DSpaceDataset(DatasetDownloader, DatasetResult):
+    """Downloader for DSpaceDataset repositories."""
+
+    REGEXP_ID = r"handle/(\d+\/\d+)"
+
+    # paths to file attributes
+    ATTR_KIND_JSONPATH = "attributes.kind"
+
+    ATTR_FILE_LINK_JSONPATH = "link"
+
+    ATTR_NAME_JSONPATH = "name"
+    ATTR_SIZE_JSONPATH = "sizeBytes"
+    ATTR_HASH_JSONPATH = "checkSum.checkSumAlgorithm"
+    ATTR_HASH_TYPE_VALUE = "checkSum.value"
+
+    def _get_attr_link(self, record):
+
+        return self.base_url + record["retrieveLink"]
+
+    def _pre_files(self):
+
+        handle_id_url = "{base_url}/rest/handle/{api_record_id}".format(
+            base_url=self.base_url, api_record_id=self.api_record_id
+        )
+        res = requests.get(handle_id_url)
+
+        # set the API_URL_META
+        self.API_URL_META = self.base_url + res.json()["link"] + "/bitstreams"
+
+
 class MendeleyDataset(DatasetDownloader, DatasetResult):
     """Downloader for Mendeley repository."""
 
     REGEXP_ID_WITH_VERSION = r"data\.mendeley\.com\/datasets\/([0-9a-z]+)\/(\d+)"
     REGEXP_ID = r"data\.mendeley\.com\/datasets\/([0-9a-z]+)"
 
     # the base entry point of the REST API
     API_URL = "https://data.mendeley.com/public-api/"
 
     # version url
-    API_URL_VERSION = API_URL + "datasets/{api_record_id}/versions"
+    API_URL_VERSION = "{api_url}datasets/{api_record_id}/versions"
 
     # the files and metadata about the dataset
     API_URL_META = (
-        API_URL + "datasets/{api_record_id}/files?folder_id=root&version={version}"
+        "{api_url}datasets/{api_record_id}/files?folder_id=root&version={version}"
     )
 
     # paths to file attributes
     ATTR_FILE_LINK_JSONPATH = "content_details.download_url"
     ATTR_NAME_JSONPATH = "filename"
     ATTR_SIZE_JSONPATH = "size"
     ATTR_HASH_JSONPATH = "content_details.sha256_hash"
     ATTR_HASH_TYPE_VALUE = "sha256"
 
     def _pre_files(self):
 
         if self.version is None:
             r_version = requests.get(
-                self.API_URL_VERSION.format(api_record_id=self.api_record_id)
+                self.API_URL_VERSION.format(
+                    api_url=self.API_URL,
+                    api_record_id=self.api_record_id)
             )
             self.version = r_version.json()[-1]["version"]
 
 
 class GitHubDataset(DatasetDownloader, DatasetResult):
     """Downloader for GitHub repository."""
 
@@ -265,14 +309,14 @@
         self,
         output_folder: Union[Path, str],
         **kwargs,
     ):
 
         try:
             from datasets import load_dataset
-        except ImportError:
+        except ImportError as err:
             raise ImportError(
                 "Install 'datasets' to use HuggingFace Datasets"
                 " or use 'pip install datahugger[all]'"
-            )
+            ) from err
 
         load_dataset(self.api_record_id, cache_dir=output_folder, **kwargs)
```

### Comparing `datahugger-0.2.1/datahugger/utils.py` & `datahugger-0.3/datahugger/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     return urlparse(s).netloc != ""
 
 
 def _format_filename(s, len_s=35) -> str:
 
     # README_Pfaller_Robinson_2022_Global_Sea_Turtle_Epibiont_Database.txt
 
+    if len_s is None:
+        return s
+
     s = str(s)
 
     if len(s) <= len_s:
         return s.ljust(len_s, " ")
 
     len_suffixes = len("".join(Path(s).suffixes))
```

### Comparing `datahugger-0.2.1/datahugger.egg-info/PKG-INFO` & `datahugger-0.3/datahugger.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahugger
-Version: 0.2.1
+Version: 0.3
 Summary: One downloader for many scientific data and code repositories!
 Author-email: Jonathan de Bruin <jonathandebruinos@gmail.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -25,15 +25,15 @@
 
 # Datahugger - Where DOI :open_hands: Data
 
 Datahugger is a tool to download scientific datasets, software, and code from a large number of repositories based on their DOI [(wiki)](https://en.wikipedia.org/wiki/Digital_object_identifier) or URL. With Datahugger, you can automate the downloading of data and improve the reproducibility of your research. Datahugger provides a straightforward [Python interface](#download-with-python) as well as an intuitive [Command Line Interface](#download-with-command-line) (CLI).
 
 ## Supported repositories
 
-Datahugger offers support for more than [<!-- count -->226<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
+Datahugger offers support for more than [<!-- count -->350<!-- count --> generic and specific (scientific) repositories](https://j535d165.github.io/datahugger/repositories) (and more to come!).
 
 [![Datahugger support Zenodo, Dataverse, DataOne, GitHub, FigShare, HuggingFace, Mendeley Data, Dryad, OSF, and many more](https://github.com/J535D165/datahugger/raw/main/docs/images/logos.png)](https://j535d165.github.io/datahugger/repositories)
 
 We are still expanding Datahugger with support for more repositories. You can
 help by [requesting support for a repository](https://github.com/J535D165/datahugger/issues/new/choose) in the issue
 tracker. Pull Requests are very welcome as well.
 
@@ -45,57 +45,61 @@
 
 ```
 pip install datahugger
 ```
 
 ## Getting started
 
-### Download with Python
+### Datahugger with Python
 
 Load a dataset (or any digital asset) from a repository with the
-`datahugger.load_repository` function. The first argument is the DOI or URL
+`datahugger.get()` function. The first argument is the DOI or URL
 and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
+The following code loads dataset [10.5061/dryad.mj8m0](https://doi.org/10.5061/dryad.mj8m0) into
+the folder `data`. 
+
 ```python
 import datahugger
 
-# download the data to your device
-datahugger.get("10.5061/dryad.x3ffbg7m8", "data")
+# download the dataset to the folder "data"
+datahugger.get("10.5061/dryad.mj8m0", "data")
 ```
 
-The data from DOI [10.5061/dryad.x3ffbg7m8](https://doi.org/10.5061/dryad.x3ffbg7m8) is now stored in the folder `data`. The data can now be accessed and analyzed. For example:
-
-```python
-
-import pandas as pd
-
-df = pd.read_csv("data/Pfaller_Robinson_2022_Global_Sea_Turtle_Epibiont_Database.csv")
-print(df["Higher Taxon"].value_counts())
-```
+For an example how this can integrate with your work, see the 
+[example workflow notebook](https://github.com/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb) or 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/J535D165/datahugger/blob/main/examples/example_datahugger_in_workflow.ipynb)
 
 
-### Download with command line
+### Datahugger with command line
 
 The command line function `datahugger` provides an easy interface to download data. The first
 argument is the DOI or URL and the second argument the name of the folder to store the dataset (will be
 created if it does not exist).
 
 ```bash
-datahugger 10.5061/dryad.31zcrjdm5 data
+datahugger 10.5061/dryad.mj8m0 data
 ```
 
 ```bash
-% datahugger 10.5061/dryad.x3ffbg7m8 data
-README_Pfaller_Robinson_20[...].txt: 100%|█████████████████████████████████████| 17.1k/17.1k [00:00<00:00, 2.62MB/s]
-Pfaller_Robinson_2022_Glob[...].csv: 100%|████████████████████████████████████████| 709k/709k [00:00<00:00, 904kB/s]
-Repository content successfully downloaded.
+% datahugger 10.5061/dryad.mj8m0 data
+Collecting...
+NestTemperatureData.csv            : 100%|████████████████████████████████████████| 607k/607k
+README_for_NestTemperatureData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+ExternalTemps.csv                  : 100%|██████████████████████████████████████| 1.06k/1.06k
+README_for_ExternalTemps.txt       : 100%|██████████████████████████████████████| 2.82k/2.82k
+InternalEggTempData.csv            : 100%|██████████████████████████████████████████| 664/664
+README_for_InternalEggTempData.txt : 100%|██████████████████████████████████████| 2.82k/2.82k
+SoilSimulation_Output.csv          : 100%|████████████████████████████████████████| 229M/229M
+README_for_SoilSimulation_[...].txt: 100%|██████████████████████████████████████| 2.82k/2.82k
+Dataset successfully downloaded.
 ```
 
-**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.31zcrjdm5" data`. 
+**Tip:** On some systems, you have to quote the DOI or URL. For example: `datahugger "10.5061/dryad.mj8m0" data`. 
 
 ## Tips and tricks
 
 - No need to struggle with DOIs versus DOI URLs. They both work (and more). Example: The values `10.5061/dryad.x3ffbg7m8`, `doi:10.5061/dryad.x3ffbg7m8`, [`https://doi.org/10.5061/dryad.x3ffbg7m8`](https://doi.org/10.5061/dryad.x3ffbg7m8), and [`https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8`](https://datadryad.org/stash/dataset/doi:10.5061/dryad.x3ffbg7m8) all point to the same dataset.
 - Do not republish the dataset when you are uploading your data to an scientific data repository. These storages resources can be used better :)
 
 ## License
```

### Comparing `datahugger-0.2.1/datahugger.egg-info/SOURCES.txt` & `datahugger-0.3/datahugger.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-.flake8
 .gitignore
+.pre-commit-config.yaml
 CITATION.cff
 LICENSE
 README.md
 datahugger_repocard_dark.svg
 datahugger_repocard_tagline.svg
 mkdocs.yml
 pyproject.toml
@@ -39,13 +39,14 @@
 docs/working.md
 docs/images/datahugger_architecture.drawio
 docs/images/datahugger_architecture.drawio.svg
 docs/images/datahugger_repo.svg
 docs/images/logos.ai
 docs/images/logos.png
 docs/stylesheets/extra.css
+examples/example_datahugger_in_workflow.ipynb
 scripts/datacite_clients.py
 scripts/estimate_repos_supported.py
 tests/test_dataset_result.py
 tests/test_repositories.py
 tests/test_resolver.py
 tests/test_utils.py
```

### Comparing `datahugger-0.2.1/datahugger_repocard_dark.svg` & `datahugger-0.3/datahugger_repocard_dark.svg`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/datahugger_repocard_tagline.svg` & `datahugger-0.3/datahugger_repocard_tagline.svg`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/development.md` & `datahugger-0.3/docs/development.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/download.md` & `datahugger-0.3/docs/download.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/images/datahugger_architecture.drawio` & `datahugger-0.3/docs/images/datahugger_architecture.drawio`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/images/datahugger_architecture.drawio.svg` & `datahugger-0.3/docs/images/datahugger_architecture.drawio.svg`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/images/datahugger_repo.svg` & `datahugger-0.3/docs/images/datahugger_repo.svg`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/images/logos.ai` & `datahugger-0.3/docs/images/logos.ai`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/images/logos.png` & `datahugger-0.3/docs/images/logos.png`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/index.md` & `datahugger-0.3/docs/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 <p align="center">
   <img alt="Datahugger - Where DOI hugs data" src="images/datahugger_repo.svg">
 </p>
 
 ## Alternatives
 
 Datahugger's main focus is on downloading datasets from arbitrary DOI's. As
-far as I know, there are alternatives for downloading datasets from arbitrary
+far as I know, there are no alternatives for downloading datasets from arbitrary
 DOI's. However, there are many libraries for downloading datasets from a
 repository right away. Usually they can also be used for uploading data to
-the respotory. Nice examples are:
+the repository. Nice examples are:
 
 - [https://guides.dataverse.org/en/latest/api/client-libraries.html](https://guides.dataverse.org/en/latest/api/client-libraries.html)
 - [https://pypi.org/project/pyzenodo3/](https://pypi.org/project/pyzenodo3/)
 - [https://osfclient.readthedocs.io/en/latest/](https://osfclient.readthedocs.io/en/latest/)
```

### Comparing `datahugger-0.2.1/docs/object.md` & `datahugger-0.3/docs/object.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/options.md` & `datahugger-0.3/docs/options.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/repositories.md` & `datahugger-0.3/docs/repositories.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/repositories_not_supported.md` & `datahugger-0.3/docs/repositories_not_supported.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/docs/reproducible.md` & `datahugger-0.3/docs/reproducible.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 scientific publications. Once you found the dataset, copy the DOI. If there
 is no DOI available, use the URL to the dataset.
 
 ### Instruct user to install datahugger
 
 If the user doesn't have datahugger installed on their device, it is required
 to install datahugger. Datahugger can be added to an existing Python
-installation file like `requirements.txt` of via documentation `pip install
+installation file like `requirements.txt` or via documentation `pip install
 datahugger`.
 
 ### Scenario 1: Standalone project setup
 
 In this scenario, you create a script or piece of documentation to setup the prerequirements for your project. This likely contains the installation dependencies and the download of the data with Datahugger. The following example shows an example for a Python project.
 
 ```bash
```

### Comparing `datahugger-0.2.1/docs/working.md` & `datahugger-0.3/docs/working.md`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/mkdocs.yml` & `datahugger-0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/pyproject.toml` & `datahugger-0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -32,7 +32,13 @@
 build-backend = 'setuptools.build_meta'
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 
 [tool.setuptools]
 packages = ["datahugger"]
 
 [tool.setuptools_scm]
+
+[tool.ruff]
+select = ["E", "F", "UP", "I", "B"]
+
+[tool.ruff.isort]
+force-single-line = true
```

### Comparing `datahugger-0.2.1/scripts/datacite_clients.py` & `datahugger-0.3/scripts/datacite_clients.py`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/scripts/estimate_repos_supported.py` & `datahugger-0.3/scripts/estimate_repos_supported.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,28 @@
 
 
 n_dataverse = get_count(
     "https://www.re3data.org/api/beta/repositories?software%5B%5D=DataVerse"
 )
 # print("DataVerse", n_dataverse)
 
+n_dspace = get_count(
+    "https://www.re3data.org/api/beta/repositories?software%5B%5D=DSpace"
+)
+# print("DSpace", n_dspace)
+
 n_figshare = get_count("https://www.re3data.org/api/beta/repositories?query=figshare")
 # print("FigShare", n_figshare)
 
 n_dataone = get_count("https://www.re3data.org/api/beta/repositories?query=dataone")
 # print("DataOne", n_dataone)
 
 single_instance_repos = ["zenodo", "mendeley", "osf", "dryad", "github", "huggingface"]
 
-n_total = n_dataverse + n_figshare + n_dataone + len(single_instance_repos)
+n_total = n_dataverse + n_figshare + n_dspace + n_dataone + len(single_instance_repos)
 print("Number of supported data repositories", n_total)
 
 
 if 1:
 
     with open("README.md") as f_read:
         readme = f_read.read()
```

### Comparing `datahugger-0.2.1/tests/test_dataset_result.py` & `datahugger-0.3/tests/test_dataset_result.py`

 * *Files identical despite different names*

### Comparing `datahugger-0.2.1/tests/test_repositories.py` & `datahugger-0.3/tests/test_repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     ("https://doi.org/10.7910/DVN/KBHLOD", "tutorial1.py"),
     # Figshare
     ("https://doi.org/10.6084/m9.figshare.8851784.v1", "cross_year_data2.csv"),
     (
         "https://figshare.com/articles/dataset/Long-term_behavioral_repeatability_in_wild_adult_and_captive_juvenile_turtles_implications_for_personality_development/8851784",
         "cross_year_data2.csv",
     ),
+    ("https://doi.org/10.15131/shef.data.22010159.v2",
+     "ScHARR QUIT evaluation statistical and health economic analysis plan.pdf"),
+    # Djehuty
     ("https://doi.org/10.4121/21989216.v1", "README.txt"),
     # Dryad
     (
         "https://datadryad.org/stash/dataset/doi:10.5061/dryad.31zcrjdm5",
         "ReadmeFile.txt",
     ),
     ("https://doi.org/10.5061/dryad.31zcrjdm5", "ReadmeFile.txt"),
@@ -35,14 +38,19 @@
     (
         "https://doi.org/10.17632/p6wmtv6t5g.2",
         "READMI Stranding Sea Turtle records.pdf",
     ),
     ("https://doi.org/10.17632/p6wmtv6t5g", "READMI Stranding Sea Turtle records.pdf"),
     # Dataone
     ("https://doi.org/10.18739/A2KH0DZ42", "2012F_Temperature_Data.csv"),
+
+    # DSpace
+    ("https://uhra.herts.ac.uk/handle/2299/26087", "pdf.pdf"),
+    ("https://repositorioinstitucional.ceu.es/handle/10637/2741",
+     "Aquaporin_1_JAMartin_et_al_MedSport_2009.pdf"),
 ]
 
 
 def test_url_checker():
 
     assert not _is_url("82949")
     assert _is_url("https://doi.org/10.5281/zenodo.6614829")
```

