# Comparing `tmp/ethpm-types-0.4.4.tar.gz` & `tmp/ethpm-types-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.4.4.tar", last modified: Fri Apr 28 13:25:23 2023, max compression
+gzip compressed data, was "ethpm-types-0.4.5.tar", last modified: Tue May  2 12:41:47 2023, max compression
```

## Comparing `ethpm-types-0.4.4.tar` & `ethpm-types-0.4.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.038358 ethpm-types-0.4.4/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 13:25:22.000000 ethpm-types-0.4.4/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.042358 ethpm-types-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:25:23.050359 ethpm-types-0.4.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/data/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-28 13:24:56.000000 ethpm-types-0.4.4/tests/test_sourcemap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.811100 ethpm-types-0.4.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.815101 ethpm-types-0.4.5/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 12:41:47.000000 ethpm-types-0.4.5/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.819101 ethpm-types-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:41:47.823101 ethpm-types-0.4.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  5214582 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/data/VyperContract.json
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-02 12:41:19.000000 ethpm-types-0.4.5/tests/test_sourcemap.py
```

### Comparing `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.4.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/.github/release-drafter.yml` & `ethpm-types-0.4.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/.github/workflows/commitlint.yaml` & `ethpm-types-0.4.5/.github/workflows/commitlint.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install -r cz-requirement.txt
 
         - name: Check commit history
```

### Comparing `ethpm-types-0.4.4/.github/workflows/docs.yaml` & `ethpm-types-0.4.5/.github/workflows/docs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[doc]
 
         - name: Build HTML artifact
```

### Comparing `ethpm-types-0.4.4/.github/workflows/prtitle.yaml` & `ethpm-types-0.4.5/.github/workflows/prtitle.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install -r cz-requirement.txt
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ethpm-types-0.4.4/.github/workflows/publish.yaml` & `ethpm-types-0.4.5/.github/workflows/publish.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
 
     - name: Build
```

### Comparing `ethpm-types-0.4.4/.github/workflows/test.yaml` & `ethpm-types-0.4.5/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10"]  # eventually add 3.11
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
@@ -90,14 +90,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ethpm-types-0.4.4/.gitignore` & `ethpm-types-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/.pre-commit-config.yaml` & `ethpm-types-0.4.5/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ethpm-types-0.4.4/CONTRIBUTING.md` & `ethpm-types-0.4.5/CONTRIBUTING.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
```

### Comparing `ethpm-types-0.4.4/LICENSE` & `ethpm-types-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/PKG-INFO` & `ethpm-types-0.4.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.4
+Version: 0.4.5
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
-        The library validates and serializes contract related data and provides JSON schemas.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ethpm-types
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ethpm-types.git
-        cd ethpm-types
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Starting with a dictionary of attribute data, such as a contract instance, you can build an EthPM typed object.
-        
-        ```python
-        from ethpm_types import ContractInstance
-        
-        contract = ContractInstance(contractType="ContractClassName", address="0x123...")
-        print(contract.contract_type)
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
+The library validates and serializes contract related data and provides JSON schemas.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ethpm-types
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ethpm-types.git
+cd ethpm-types
+python3 setup.py install
+```
+
+## Quick Usage
+
+Starting with a dictionary of attribute data, such as a contract instance, you can build an EthPM typed object.
+
+```python
+from ethpm_types import ContractInstance
+
+contract = ContractInstance(contractType="ContractClassName", address="0x123...")
+print(contract.contract_type)
+```
```

### Comparing `ethpm-types-0.4.4/README.md` & `ethpm-types-0.4.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
 The library validates and serializes contract related data and provides JSON schemas.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ethpm-types-0.4.4/build_docs.py` & `ethpm-types-0.4.5/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/_static/custom.css` & `ethpm-types-0.4.5/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/_static/custom.js` & `ethpm-types-0.4.5/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/_templates/layout.html` & `ethpm-types-0.4.5/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/conf.py` & `ethpm-types-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/favicon.ico` & `ethpm-types-0.4.5/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/docs/logo.gif` & `ethpm-types-0.4.5/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/__init__.py` & `ethpm-types-0.4.5/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/abi.py` & `ethpm-types-0.4.5/ethpm_types/abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/ast.py` & `ethpm-types-0.4.5/ethpm_types/ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/base.py` & `ethpm-types-0.4.5/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/contract_type.py` & `ethpm-types-0.4.5/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/manifest.py` & `ethpm-types-0.4.5/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/source.py` & `ethpm-types-0.4.5/ethpm_types/source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/sourcemap.py` & `ethpm-types-0.4.5/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types/utils.py` & `ethpm-types-0.4.5/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.4.5/ethpm_types.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.4.4
+Version: 0.4.5
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
-        The library validates and serializes contract related data and provides JSON schemas.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ethpm-types
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ethpm-types.git
-        cd ethpm-types
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Starting with a dictionary of attribute data, such as a contract instance, you can build an EthPM typed object.
-        
-        ```python
-        from ethpm_types import ContractInstance
-        
-        contract = ContractInstance(contractType="ContractClassName", address="0x123...")
-        print(contract.contract_type)
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+EthPM is an Ethereum package manifest containing data types for contracts, deployments, and source code using [EIP-2678](https://eips.ethereum.org/EIPS/eip-2678).
+The library validates and serializes contract related data and provides JSON schemas.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ethpm-types
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ethpm-types.git
+cd ethpm-types
+python3 setup.py install
+```
+
+## Quick Usage
+
+Starting with a dictionary of attribute data, such as a contract instance, you can build an EthPM typed object.
+
+```python
+from ethpm_types import ContractInstance
+
+contract = ContractInstance(contractType="ContractClassName", address="0x123...")
+print(contract.contract_type)
+```
```

### Comparing `ethpm-types-0.4.4/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.4.5/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.4.5/ethpm_types.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 hexbytes<1,>=0.3.0
-pydantic<2,>=1.10.1
-eth-utils<3,>=2.0.0
+pydantic<2,>=1.10.7
+eth-utils<3,>=2.1.0
 py-cid<0.4,>=0.3.0
-requests<3,>=2.28.1
+requests<3,>=2.29.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 PyGithub<2.0,>=1.54
 hypothesis-jsonschema==0.19.0
 pysha3<2.0.0,>=1.0.2
 black<24,>=23.3.0
 mypy<1,>=0.991
 types-setuptools
 types-requests
-flake8<6,>=5.0.4
+flake8<7,>=6.0.0
 flake8-breakpoint>=1.1.0
 flake8-print>=4.0.0
 isort<5.11,>=5.10.1
 setuptools
 wheel
 twine
 commitizen<2.41,>=2.40
@@ -37,15 +37,15 @@
 sphinxcontrib-napoleon>=0.7
 
 [lint]
 black<24,>=23.3.0
 mypy<1,>=0.991
 types-setuptools
 types-requests
-flake8<6,>=5.0.4
+flake8<7,>=6.0.0
 flake8-breakpoint>=1.1.0
 flake8-print>=4.0.0
 isort<5.11,>=5.10.1
 
 [release]
 setuptools
 wheel
```

### Comparing `ethpm-types-0.4.4/pyproject.toml` & `ethpm-types-0.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ethpm-types-0.4.4/setup.py` & `ethpm-types-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "pysha3>=1.0.2,<2.0.0",  # Backend for eth-hash
     ],
     "lint": [
         "black>=23.3.0,<24",  # auto-formatter and linter
         "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
         "types-requests",  # Needed due to mypy typeshed
-        "flake8>=5.0.4,<6",  # Style linter
+        "flake8>=6.0.0,<7",  # Style linter
         "flake8-breakpoint>=1.1.0",  # detect breakpoints left in code
         "flake8-print>=4.0.0",  # detect print statements left in code
         "isort>=5.10.1,<5.11",  # Import sorting linter
     ],
     "doc": [
         "myst-parser>=0.17.0,<0.18",  # Tools for parsing markdown files in the docs
         "sphinx-click>=3.1.0,<4.0",  # For documenting CLI
@@ -70,20 +70,20 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ethpm-types",
     include_package_data=True,
     install_requires=[
         "hexbytes>=0.3.0,<1",
-        "pydantic>=1.10.1,<2",
-        "eth-utils>=2.0.0,<3",
+        "pydantic>=1.10.7,<2",
+        "eth-utils>=2.1.0,<3",
         "py-cid>=0.3.0,<0.4",
-        "requests>=2.28.1,<3",
+        "requests>=2.29.0,<3",
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ethpm_types"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ethpm_types": ["py.typed"]},
@@ -94,9 +94,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ethpm-types-0.4.4/tests/conftest.py` & `ethpm-types-0.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/data/OpenZeppelinContracts.json` & `ethpm-types-0.4.5/tests/data/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/data/SolidityContract.json` & `ethpm-types-0.4.5/tests/data/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/data/TestStrategy.srcmap` & `ethpm-types-0.4.5/tests/data/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/data/VyperContract.json` & `ethpm-types-0.4.5/tests/data/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_ast.py` & `ethpm-types-0.4.5/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_cairo.py` & `ethpm-types-0.4.5/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_contract_type.py` & `ethpm-types-0.4.5/tests/test_contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_hexbytes.py` & `ethpm-types-0.4.5/tests/test_hexbytes.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_package_manifest.py` & `ethpm-types-0.4.5/tests/test_package_manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_pc_map.py` & `ethpm-types-0.4.5/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_schema_fuzzing.py` & `ethpm-types-0.4.5/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_source.py` & `ethpm-types-0.4.5/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.4.4/tests/test_sourcemap.py` & `ethpm-types-0.4.5/tests/test_sourcemap.py`

 * *Files identical despite different names*

