# Comparing `tmp/swh.loader.bzr-1.3.2.tar.gz` & `tmp/swh.loader.bzr-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.bzr-1.3.2.tar", last modified: Mon Oct 10 12:40:24 2022, max compression
+gzip compressed data, was "dist/swh.loader.bzr-1.3.3.tar", last modified: Tue May  2 11:55:48 2023, max compression
```

## Comparing `swh.loader.bzr-1.3.2.tar` & `swh.loader.bzr-1.3.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      122 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      847 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       26 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      179 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1215 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      291 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      571 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      291 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2044 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/how-bzr-works.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      208 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      361 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       96 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      344 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2704 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/
--rw-r--r--   0 jenkins    (115) docker     (999)      470 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26872 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)      768 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1140 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      191 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/broken-tags.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      980 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/broken-tags.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      275 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/does-not-support-tags.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     1049 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/does-not-support-tags.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      106 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/empty.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      962 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/empty.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      400 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/ghosts.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2451 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/ghosts.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      636 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/metadata-and-type-changes.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    13831 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/metadata-and-type-changes.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      139 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/needs-upgrade.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      880 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/needs-upgrade.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      213 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/no-branch.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      882 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/no-branch.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      829 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/nominal.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    11366 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/nominal.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/renames.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     5068 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/renames.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)    14359 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1972 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/swh/loader/bzr/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1215 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1716 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      118 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      199 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-10-10 12:40:24.000000 swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1471 2022-10-10 12:40:22.000000 swh.loader.bzr-1.3.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      122 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       26 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1215 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      291 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      291 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2044 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/how-bzr-works.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      257 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      361 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      364 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2704 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/
+-rw-r--r--   0 jenkins    (115) docker     (999)      470 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26805 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)      768 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1140 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      191 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/broken-tags.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      980 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/broken-tags.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      275 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/does-not-support-tags.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     1049 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/does-not-support-tags.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      106 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/empty.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      962 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/empty.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      400 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/ghosts.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2451 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/ghosts.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      636 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/metadata-and-type-changes.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    13831 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/metadata-and-type-changes.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      139 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/needs-upgrade.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      880 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/needs-upgrade.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      213 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/no-branch.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/no-branch.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      829 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/nominal.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    11366 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/nominal.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/renames.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     5068 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/renames.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)    14359 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1260 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/swh/loader/bzr/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1215 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1716 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      118 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      219 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-02 11:55:48.000000 swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1835 2023-05-02 11:55:45.000000 swh.loader.bzr-1.3.3/tox.ini
```

### Comparing `swh.loader.bzr-1.3.2/.pre-commit-config.yaml` & `swh.loader.bzr-1.3.3/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.3.0
     hooks:
       - id: trailing-whitespace
       - id: check-json
       - id: check-yaml
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8
+    rev: 5.0.4
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-bugbear==22.3.23]
+        additional_dependencies: [flake8-bugbear==22.9.23]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.2
     hooks:
       - id: codespell
         name: Check source code spelling
         stages: [commit]
 
   - repo: local
     hooks:
@@ -26,15 +26,15 @@
         entry: mypy
         args: [swh]
         pass_filenames: false
         language: system
         types: [python]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
 
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
       - id: black
```

### Comparing `swh.loader.bzr-1.3.2/CODE_OF_CONDUCT.md` & `swh.loader.bzr-1.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/LICENSE` & `swh.loader.bzr-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/PKG-INFO` & `swh.loader.bzr-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.bzr
-Version: 1.3.2
+Version: 1.3.3
 Summary: Software Heritage Bazaar/Breezy intent
 Home-page: https://forge.softwareheritage.org/diffusion/DLDBZR/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-bzr
```

### Comparing `swh.loader.bzr-1.3.2/conftest.py` & `swh.loader.bzr-1.3.3/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/docs/how-bzr-works.rst` & `swh.loader.bzr-1.3.3/docs/how-bzr-works.rst`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/setup.py` & `swh.loader.bzr-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/loader.py` & `swh.loader.bzr-1.3.3/swh/loader/bzr/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,25 @@
 from Bazaar or Breezy.
 """
 from datetime import datetime
 from functools import lru_cache, partial
 import itertools
 import os
 from tempfile import mkdtemp
-from typing import (
-    Any,
-    Dict,
-    Iterator,
-    List,
-    NewType,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, TypeVar, Union
 
 from breezy import errors as bzr_errors
 from breezy import repository, tsort
+from breezy.branch import Branch as BzrBranch
 from breezy.builtins import cmd_branch, cmd_upgrade
-from breezy.bzr import bzrdir
-from breezy.bzr.branch import Branch as BzrBranch
-from breezy.bzr.inventory import Inventory, InventoryEntry
-from breezy.bzr.inventorytree import InventoryTreeChange
+from breezy.controldir import ControlDir
 from breezy.revision import NULL_REVISION
 from breezy.revision import Revision as BzrRevision
-from breezy.tree import Tree
+from breezy.revision import RevisionID as BzrRevisionId
+from breezy.tree import Tree, TreeChange
 
 from swh.loader.core.loader import BaseLoader
 from swh.loader.core.utils import clean_dangling_folders, clone_with_timeout
 from swh.model import from_disk, swhids
 from swh.model.model import (
     Content,
     ExtID,
@@ -56,16 +44,14 @@
 from swh.storage.algos.snapshot import snapshot_get_latest
 from swh.storage.interface import StorageInterface
 
 TEMPORARY_DIR_PREFIX_PATTERN = "swh.loader.bzr.from_disk"
 EXTID_TYPE = "bzr-nodeid"
 EXTID_VERSION: int = 1
 
-BzrRevisionId = NewType("BzrRevisionId", bytes)
-
 T = TypeVar("T")
 
 # These are all the old Bazaar repository formats that we might encounter
 # in the wild. Bazaar's `clone` does not result in an upgrade, it needs to be
 # explicit.
 older_repository_formats = {
     b"Bazaar Knit Repository Format 3 (bzr 0.15)\n",
@@ -132,15 +118,15 @@
         # TODO move to swh.model.from_disk.Directory
         try:
             return self[path]
         except KeyError:
             return default
 
 
-def sort_changes(change: InventoryTreeChange) -> str:
+def sort_changes(change: TreeChange) -> str:
     """Key function for sorting the changes by path.
 
     Sorting allows us to group the folders together (for example "b", then "a/a",
     then "a/b"). Reversing this sort in the `sorted()` call will make it
     so the files appear before the folder ("a/a", then "a") if the folder has
     changed. This removes a bug where the order of operations is:
 
@@ -257,15 +243,15 @@
         return extids
 
     def cleanup(self) -> None:
         if self.repo is not None:
             self.repo.unlock()
 
     def get_repo_and_branch(self) -> Tuple[repository.Repository, BzrBranch]:
-        _, branch, repo, _ = bzrdir.BzrDir.open_containing_tree_branch_or_repository(
+        _, branch, repo, _ = ControlDir.open_containing_tree_branch_or_repository(
             self._repo_directory
         )
         return repo, branch
 
     def run_upgrade(self):
         """Upgrade both repository and branch to the most recent supported version
         to be compatible with the loader."""
@@ -302,15 +288,15 @@
         else:  # existing local repository
             # Allow to load on disk repository without cloning
             # for testing purpose.
             self.log.debug("Using local directory '%s'", self.directory)
             self._repo_directory = self.directory
 
         repo, branch = self.get_repo_and_branch()
-        repository_format = repo._format.as_string()  # lies about being a string
+        repository_format = repo._format.get_format_string()
 
         if not repository_format == expected_repository_format:
             if repository_format in older_repository_formats:
                 self.log.debug(
                     "Upgrading repository from format '%s'",
                     repository_format.decode("ascii").strip("\n"),
                 )
@@ -423,15 +409,19 @@
         timezone = round(int(bzr_rev.timezone) / 60)
         date = TimestampWithTimezone.from_numeric_offset(timestamp, timezone, False)
 
         # TODO (how) should we store multiple authors? (T3887)
         revision = Revision(
             author=Person.from_fullname(bzr_rev.get_apparent_authors()[0].encode()),
             date=date,
-            committer=Person.from_fullname(bzr_rev.committer.encode()),
+            committer=(
+                Person.from_fullname(bzr_rev.committer.encode())
+                if bzr_rev.committer
+                else None
+            ),
             committer_date=date,
             type=RevisionType.BAZAAR,
             directory=directory,
             message=bzr_rev.message.encode(),
             extra_headers=extra_headers,
             synthetic=False,
             parents=self._get_revision_parents(bzr_rev),
@@ -449,29 +439,27 @@
                     target=revision.swhid(),
                 )
             ]
         )
 
     def store_directories(self, bzr_rev: BzrRevision) -> Sha1Git:
         """Store a revision's directories."""
-        repo: repository.Repository = self.repo
-        inventory: Inventory = repo.get_inventory(bzr_rev.revision_id)
+        new_tree = self._get_revision_tree(bzr_rev.revision_id)
         if self._prev_revision is None:
-            self._store_directories_slow(bzr_rev, inventory)
+            self._store_directories_slow(bzr_rev, new_tree)
             return self._store_tree(bzr_rev)
 
         old_tree = self._get_revision_tree(self._prev_revision.revision_id)
-        new_tree = self._get_revision_tree(bzr_rev.revision_id)
 
         delta = new_tree.changes_from(old_tree)
 
         if delta.renamed or delta.copied:
             # Figuring out all nested and possibly conflicting renames is a lot
             # of effort for very few revisions, just go the slow way
-            self._store_directories_slow(bzr_rev, inventory)
+            self._store_directories_slow(bzr_rev, new_tree)
             return self._store_tree(bzr_rev)
 
         to_remove = sorted(
             delta.removed + delta.missing, key=sort_changes, reverse=True
         )
         for change in to_remove:
             if change.kind[0] == "directory":
@@ -481,16 +469,18 @@
             del self._last_root[path.encode()]
 
         # `delta.kind_changed` needs to happen before `delta.added` since a file
         # could be added under a node that changed from directory to file at the
         # same time, for example
         for change in itertools.chain(delta.kind_changed, delta.added, delta.modified):
             path = change.path[1]
-            entry = inventory.get_entry(change.file_id)
-            content = self.store_content(bzr_rev, path, entry)
+            (kind, size, executable, _sha1_or_link) = new_tree.path_content_summary(
+                path
+            )
+            content = self.store_content(bzr_rev, path, kind, executable, size)
             self._last_root[path.encode()] = content
 
         self._prev_revision = bzr_rev
         return self._store_tree(bzr_rev)
 
     def store_release(self, name: bytes, target: Sha1Git) -> Sha1Git:
         """Store a release given its name and its target.
@@ -514,50 +504,55 @@
         )
 
         self.storage.release_add([release])
 
         return release.id
 
     def store_content(
-        self, bzr_rev: BzrRevision, file_path: str, entry: InventoryEntry
+        self,
+        bzr_rev: BzrRevision,
+        file_path: str,
+        kind: str,
+        executable: bool,
+        size: int,
     ) -> from_disk.Content:
-        if entry.executable:
+        if executable:
             perms = from_disk.DentryPerms.executable_content
-        elif entry.kind == "directory":
+        elif kind == "directory":
             perms = from_disk.DentryPerms.directory
-        elif entry.kind == "symlink":
+        elif kind == "symlink":
             perms = from_disk.DentryPerms.symlink
-        elif entry.kind == "file":
+        elif kind == "file":
             perms = from_disk.DentryPerms.content
         else:  # pragma: no cover
             raise RuntimeError("Hit unreachable condition")
 
-        data = b""
-        if entry.has_text():
+        if kind == "file":
             rev_tree = self._get_revision_tree(bzr_rev.revision_id)
-            data = rev_tree.get_file(file_path).read()
-            assert len(data) == entry.text_size
+            with rev_tree.get_file(file_path) as f:
+                data = f.read()
+            assert len(data) == size
+        else:
+            data = b""
 
         content = Content.from_data(data)
 
         self.storage.content_add([content])
 
         return from_disk.Content({"sha1_git": content.sha1_git, "perms": perms})
 
-    def _get_bzr_revs_to_load(self) -> List[BzrRevision]:
+    def _get_bzr_revs_to_load(self) -> List[BzrRevisionId]:
         assert self.repo is not None
-        repo: repository.Repository = self.repo
         self.log.debug("Getting fully sorted revision tree")
         if self.head_revision_id == NULL_REVISION:
             return []
-        head_revision = repo.get_revision(self.head_revision_id)
         # bazaar's model doesn't allow it to iterate on its graph from
         # the bottom lazily, but basically all DAGs (especially bzr ones)
         # are small enough to fit in RAM.
-        ancestors_iter = self._iterate_ancestors(head_revision)
+        ancestors_iter = self._iterate_ancestors(self.head_revision_id)
         ancestry = []
         for rev, parents in ancestors_iter:
             if parents is None:
                 # Filter out ghosts, they scare the `TopoSorter`.
                 # Store them to later catch exceptions about missing parent revision
                 self._ghosts.add(rev)
                 continue
@@ -583,18 +578,20 @@
                 # everything
                 msg = "Previous head (%s) not found, loading all revisions"
                 self.log.debug(msg, self._latest_head)
                 return all_revisions
             return new_revisions
         return all_revisions
 
-    def _iterate_ancestors(self, rev: BzrRevision) -> Iterator[BzrRevisionId]:
+    def _iterate_ancestors(
+        self, revision_id: BzrRevisionId
+    ) -> Iterator[Tuple[BzrRevisionId, Tuple[BzrRevisionId]]]:
         """Return an iterator of this revision's ancestors"""
         assert self.repo is not None
-        return self.repo.get_graph().iter_ancestry([rev.revision_id])
+        return self.repo.get_graph().iter_ancestry([revision_id])
 
     # We want to cache at most the current revision and the last, no need to
     # take cache more than this.
     @lru_cache(maxsize=2)
     def _get_revision_tree(self, rev: BzrRevisionId) -> Tree:
         assert self.repo is not None
         return self.repo.revision_tree(rev)
@@ -611,33 +608,33 @@
                     for item in directory.values()
                     if isinstance(item, from_disk.Directory)
                 ]
             )
         self._prev_revision = bzr_rev
         return self._last_root.hash
 
-    def _store_directories_slow(
-        self, bzr_rev: BzrRevision, inventory: Inventory
-    ) -> None:
+    def _store_directories_slow(self, bzr_rev: BzrRevision, tree: Tree) -> None:
         """Store a revision's directories.
 
         This is the slow variant: it does not use a diff from the last revision
         but lists all the files. It is used for the first revision of a load
         (the null revision for a full run, the last recorded head for an
         incremental one) or for cases where the headaches of figuring out the
         delta from the breezy primitives is not worth it.
         """
         # Don't reuse the last root, we're listing everything anyway, and we
         # could be keeping around deleted files
         self._last_root = BzrDirectory()
-        for path, entry in inventory.iter_entries():
+        for path, entry in tree.iter_entries_by_dir():
             if path == "":
                 # root repo is created by default
                 continue
-            content = self.store_content(bzr_rev, path, entry)
+            content = self.store_content(
+                bzr_rev, path, entry.kind, entry.executable, entry.text_size
+            )
             self._last_root[path.encode()] = content
 
     def _get_revision_parents(self, bzr_rev: BzrRevision) -> Tuple[Sha1Git, ...]:
         parents = []
         for parent_id in bzr_rev.parent_ids:
             if parent_id == NULL_REVISION:
                 # Paranoid, don't think that actually happens
@@ -684,15 +681,15 @@
         self._branch = branches[0]
         return branches[0]
 
     @property
     def head_revision_id(self) -> BzrRevisionId:
         """Returns the Bazaar revision id of the branch's head.
 
-        Bazaar/Breezy branches do not have multiple heads."""
+        Bazaar branches do not have multiple heads."""
         assert self.repo is not None
         if self._head_revision_id is None:
             self._head_revision_id = self.branch.last_revision()
         assert self._head_revision_id is not None
         return BzrRevisionId(self._head_revision_id)
 
     @property
```

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tasks.py` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/conftest.py` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/broken-tags.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/broken-tags.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/does-not-support-tags.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/does-not-support-tags.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/empty.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/empty.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/ghosts.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/ghosts.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/metadata-and-type-changes.sh` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/metadata-and-type-changes.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/metadata-and-type-changes.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/metadata-and-type-changes.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/needs-upgrade.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/needs-upgrade.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/no-branch.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/no-branch.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/nominal.sh` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/nominal.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/nominal.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/nominal.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/data/renames.tgz` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/data/renames.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh/loader/bzr/tests/test_loader.py` & `swh.loader.bzr-1.3.3/swh/loader/bzr/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/PKG-INFO` & `swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.bzr
-Version: 1.3.2
+Version: 1.3.3
 Summary: Software Heritage Bazaar/Breezy intent
 Home-page: https://forge.softwareheritage.org/diffusion/DLDBZR/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-bzr
```

### Comparing `swh.loader.bzr-1.3.2/swh.loader.bzr.egg-info/SOURCES.txt` & `swh.loader.bzr-1.3.3/swh.loader.bzr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.bzr-1.3.2/tox.ini` & `swh.loader.bzr-1.3.3/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 [tox]
-envlist=black,flake8,mypy,py3
+requires =
+  tox>4
+envlist=black,flake8,mypy,py3,py3-breezy32
 
 [testenv]
 extras =
   testing
 deps =
   pytest-cov
 commands =
   pytest --doctest-modules \
          {envsitepackagesdir}/swh/loader/bzr \
          --cov={envsitepackagesdir}/swh/loader/bzr \
          --cov-branch {posargs}
 
+[testenv:py3-breezy32]
+# version 3.3.0 introduces Rust code, which requires rustc versions newer than available in Debian 11.
+# >=3.3.1 has wheels for most architecture, but some may be missing
+deps =
+  breezy < 3.3.0
+commands =
+  pytest --doctest-modules \
+         {envsitepackagesdir}/swh/loader/bzr
+
 [testenv:black]
 skip_install = true
 deps =
-  black==22.3.0
+  black==22.10.0
 commands =
   {envpython} -m black --check swh
 
 [testenv:flake8]
 skip_install = true
 deps =
-  flake8==4.0.1
-  flake8-bugbear==22.3.23
+  flake8==5.0.4
+  flake8-bugbear==22.9.23
+  pycodestyle==2.9.1
 commands =
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
 deps =
-  mypy==0.942
+  mypy==1.0.1
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

