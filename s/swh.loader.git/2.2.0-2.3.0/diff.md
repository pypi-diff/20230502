# Comparing `tmp/swh.loader.git-2.2.0.tar.gz` & `tmp/swh.loader.git-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.git-2.2.0.tar", last modified: Mon Feb 20 15:28:47 2023, max compression
+gzip compressed data, was "dist/swh.loader.git-2.3.0.tar", last modified: Tue May  2 12:39:38 2023, max compression
```

## Comparing `swh.loader.git-2.2.0.tar` & `swh.loader.git-2.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1907 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/bin/dir-git-repo-meta.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/docs/attic/
--rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/attic/api-backend-protocol.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/attic/git-loading-design.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      108 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      101 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       34 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/resources/local-loader-git.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/resources/remote-loader-git.ini
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/resources/test/
--rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/resources/test/back.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/resources/test/db-manager.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/resources/updater.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2387 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/loader/git/
--rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9812 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7758 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/dumb.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15166 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26910 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/loader/git/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1134 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/loader/git/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh/loader/git/tests/data/git-repos/
--rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
--rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/data/testrepo.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/test_from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    36583 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2522 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4070 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/swh/loader/git/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-02-20 15:28:46.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-02-20 15:28:47.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-02-20 15:28:46.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      103 2023-02-20 15:28:46.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      240 2023-02-20 15:28:46.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-02-20 15:28:46.000000 swh.loader.git-2.2.0/swh.loader.git.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-02-20 15:28:45.000000 swh.loader.git-2.2.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1907 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/bin/dir-git-repo-meta.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/attic/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/attic/api-backend-protocol.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/attic/git-loading-design.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       34 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/local-loader-git.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/remote-loader-git.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/resources/test/
+-rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/test/back.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/test/db-manager.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/updater.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2387 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/
+-rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9812 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8043 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/dumb.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15166 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    28204 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1134 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
+-rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/testrepo.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    39895 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2522 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4070 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      103 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/tox.ini
```

### Comparing `swh.loader.git-2.2.0/.pre-commit-config.yaml` & `swh.loader.git-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/CODE_OF_CONDUCT.md` & `swh.loader.git-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/LICENSE` & `swh.loader.git-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/PKG-INFO` & `swh.loader.git-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.2.0
+Version: 2.3.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
```

### Comparing `swh.loader.git-2.2.0/README.md` & `swh.loader.git-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/bin/dir-git-repo-meta.sh` & `swh.loader.git-2.3.0/bin/dir-git-repo-meta.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/conftest.py` & `swh.loader.git-2.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/docs/attic/api-backend-protocol.txt` & `swh.loader.git-2.3.0/docs/attic/api-backend-protocol.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/docs/attic/git-loading-design.txt` & `swh.loader.git-2.3.0/docs/attic/git-loading-design.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/setup.py` & `swh.loader.git-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/__init__.py` & `swh.loader.git-2.3.0/swh/loader/git/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/base.py` & `swh.loader.git-2.3.0/swh/loader/git/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/converters.py` & `swh.loader.git-2.3.0/swh/loader/git/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/dumb.py` & `swh.loader.git-2.3.0/swh/loader/git/dumb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from __future__ import annotations
 
 from collections import defaultdict
@@ -13,15 +13,17 @@
 from typing import TYPE_CHECKING, Callable, Dict, Iterable, List, Set, cast
 import urllib.parse
 
 from dulwich.errors import NotGitRepository
 from dulwich.objects import S_IFGITLINK, Commit, ShaFile, Tree
 from dulwich.pack import Pack, PackData, PackIndex, load_pack_index_file
 import requests
+from tenacity.before_sleep import before_sleep_log
 
+from swh.core.retry import http_retry
 from swh.loader.git.utils import HexBytes
 
 if TYPE_CHECKING:
     from .loader import RepoRepresentation
 
 logger = logging.getLogger(__name__)
 
@@ -114,18 +116,22 @@
             object_type: Git object type, either b"blob", b"commit", b"tag" or b"tree"
 
         Returns:
             A generator fetching git objects on the fly.
         """
         return map(self._get_git_object, self.objects[object_type])
 
+    @http_retry(
+        before_sleep=before_sleep_log(logger, logging.WARNING),
+    )
     def _http_get(self, path: str) -> SpooledTemporaryFile:
         url = urllib.parse.urljoin(self.repo_url.rstrip("/") + "/", path)
         logger.debug("Fetching %s", url)
         response = self._session.get(url, headers=HEADERS)
+        response.raise_for_status()
         buffer = SpooledTemporaryFile(max_size=100 * 1024 * 1024)
         for chunk in response.iter_content(chunk_size=10 * 1024 * 1024):
             buffer.write(chunk)
         buffer.flush()
         buffer.seek(0)
         return buffer
 
@@ -176,17 +182,18 @@
     def _get_git_object(self, sha: bytes) -> ShaFile:
         # try to get the object from a pack file first to avoid flooding
         # git server with numerous HTTP requests
         for pack in list(self.packs):
             try:
                 if sha in pack:
                     return pack[sha]
-            except (NotGitRepository, struct.error):
-                # missing (dulwich http client raises NotGitRepository on 404)
-                # or invalid pack index/content, remove it from global packs list
+            except (NotGitRepository, struct.error, requests.HTTPError) as e:
+                if isinstance(e, requests.HTTPError) and e.response.status_code != 404:
+                    raise
+                # missing or invalid pack index/content, remove it from global packs list
                 logger.debug("A pack file is missing or its content is invalid")
                 self.packs.remove(pack)
         # fetch it from objects/ directory otherwise
         sha_hex = sha.decode()
         object_path = f"objects/{sha_hex[:2]}/{sha_hex[2:]}"
         return ShaFile.from_file(self._http_get(object_path))
```

### Comparing `swh.loader.git-2.2.0/swh/loader/git/from_disk.py` & `swh.loader.git-2.3.0/swh/loader/git/from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/loader.py` & `swh.loader.git-2.3.0/swh/loader/git/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
 from dataclasses import dataclass
 import datetime
+import json
 import logging
 import os
 import pickle
 import sys
 from tempfile import SpooledTemporaryFile
 from typing import (
     Any,
@@ -39,20 +40,22 @@
     release_git_object,
     revision_git_object,
 )
 from swh.model.model import (
     BaseContent,
     Content,
     Directory,
+    RawExtrinsicMetadata,
     Release,
     Revision,
     Snapshot,
     SnapshotBranch,
     TargetType,
 )
+from swh.model.swhids import ExtendedObjectType
 from swh.storage.algos.directory import directory_get
 from swh.storage.algos.snapshot import snapshot_get_latest
 from swh.storage.interface import StorageInterface
 
 from . import converters, dumb, utils
 from .base import BaseGitLoader
 from .utils import HexBytes
@@ -196,14 +199,15 @@
         self.pack_size_bytes = pack_size_bytes
         self.temp_file_cutoff = temp_file_cutoff
         # state initialized in fetch_data
         self.remote_refs: Dict[bytes, HexBytes] = {}
         self.symbolic_refs: Dict[bytes, HexBytes] = {}
         self.ref_object_types: Dict[bytes, Optional[TargetType]] = {}
         self.ext_refs: Dict[bytes, Optional[Tuple[int, bytes]]] = {}
+        self.repo_pack_size_bytes = 0
 
     def fetch_pack_from_origin(
         self,
         origin_url: str,
         base_repo: RepoRepresentation,
         do_activity: Callable[[bytes], None],
     ) -> FetchPackReturn:
@@ -262,14 +266,32 @@
             pack_buffer=pack_buffer,
             pack_size=pack_size,
         )
 
     def get_full_snapshot(self, origin_url) -> Optional[Snapshot]:
         return snapshot_get_latest(self.storage, origin_url)
 
+    def load_metadata_objects(
+        self, metadata_objects: List[RawExtrinsicMetadata]
+    ) -> None:
+        for metadata in metadata_objects:
+            if (
+                metadata.target.object_type == ExtendedObjectType.ORIGIN
+                and metadata.format == "application/vnd.github.v3+json"
+            ):
+                try:
+                    json_metadata = json.loads(metadata.metadata)
+                    self.repo_pack_size_bytes = json_metadata.get("size", 0) * 1024
+                except json.JSONDecodeError:
+                    logger.warning(
+                        "JSON metadata for origin %s could not be parsed.",
+                        self.origin.url,
+                    )
+        super().load_metadata_objects(metadata_objects)
+
     def prepare(self) -> None:
         assert self.origin is not None
 
         self.prev_snapshot = Snapshot(branches={})
         """Last snapshot of this origin if any; empty snapshot otherwise"""
         self.base_snapshots = []
         """Last snapshot of this origin and all its parents, if any."""
@@ -300,14 +322,21 @@
         # Increments a metric with full name 'swh_loader_git'; which is useful to
         # count how many runs of the loader are with each incremental mode
         self.statsd.increment("git_total", tags={})
 
     def fetch_data(self) -> bool:
         assert self.origin is not None
 
+        if not self.base_snapshots and self.repo_pack_size_bytes > self.pack_size_bytes:
+            raise IOError(
+                f"Pack file too big for repository {self.origin.url}, "
+                f"limit is {self.pack_size_bytes} bytes, "
+                f"current size is {self.repo_pack_size_bytes}"
+            )
+
         base_repo = self.repo_representation(
             storage=self.storage,
             base_snapshots=self.base_snapshots,
             incremental=self.incremental,
             statsd=self.statsd,
         )
 
@@ -321,19 +350,21 @@
             )
         except (dulwich.client.HTTPUnauthorized, NotGitRepository) as e:
             raise NotFound(e)
         except GitProtocolError as e:
             # unfortunately, that kind of error is not specific to a not found
             # scenario... It depends on the value of message within the exception.
             for msg in [
-                "Repository unavailable",  # e.g DMCA takedown
-                "Repository not found",
+                " unavailable",  # e.g DMCA takedown
+                " not found",
                 "unexpected http resp 401",
+                "unexpected http resp 403",
+                "unexpected http resp 410",
             ]:
-                if msg in e.args[0]:
+                if msg in str(e.args[0]):
                     raise NotFound(e)
             # otherwise transmit the error
             raise
         except (AttributeError, NotImplementedError, ValueError):
             # with old dulwich versions, those exceptions types can be raised
             # by the fetch_pack operation when encountering a repository with
             # dumb transfer protocol so we check if the repository supports it
```

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tasks.py` & `swh.loader.git-2.3.0/swh/loader/git/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/conftest.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle` & `swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/data/testrepo.tgz` & `swh.loader.git-2.3.0/swh/loader/git/tests/data/testrepo.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/test_converters.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/test_from_disk.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/test_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/test_loader.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/test_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2018-2022  The Software Heritage developers
+# Copyright (C) 2018-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 from functools import partial
 from http.server import HTTPServer, SimpleHTTPRequestHandler
@@ -18,38 +18,52 @@
 import attr
 from dulwich.errors import GitProtocolError, NotGitRepository, ObjectFormatException
 from dulwich.pack import REF_DELTA
 from dulwich.porcelain import push
 import dulwich.repo
 from dulwich.tests.utils import build_pack
 import pytest
+import requests_mock
 
 from swh.loader.git import converters, dumb
 from swh.loader.git.loader import FetchPackReturn, GitLoader
 from swh.loader.git.tests.test_from_disk import SNAPSHOT1, FullGitLoaderTests
 from swh.loader.tests import (
     assert_last_visit_matches,
     get_stats,
     prepare_repository_from_archive,
 )
-from swh.model.model import Origin, OriginVisit, OriginVisitStatus, Snapshot
+from swh.model.model import (
+    MetadataAuthority,
+    MetadataAuthorityType,
+    MetadataFetcher,
+    Origin,
+    OriginVisit,
+    OriginVisitStatus,
+    RawExtrinsicMetadata,
+    Snapshot,
+)
 
 
 class CommonGitLoaderNotFound:
     @pytest.fixture(autouse=True)
     def __inject_fixtures(self, mocker):
         """Inject required fixtures in unittest.TestCase class"""
         self.mocker = mocker
 
     @pytest.mark.parametrize(
         "failure_exception",
         [
             GitProtocolError("Repository unavailable"),  # e.g DMCA takedown
+            GitProtocolError("user/project.git unavailable"),
             GitProtocolError("Repository not found"),
+            GitProtocolError("user/project.git not found"),
             GitProtocolError("unexpected http resp 401"),
+            GitProtocolError("unexpected http resp 403"),
+            GitProtocolError("unexpected http resp 410"),
             NotGitRepository("not a git repo"),
         ],
     )
     def test_load_visit_not_found(self, failure_exception):
         """Ingesting an unknown url result in a visit with not_found status"""
         # simulate an initial communication error (e.g no repository found, ...)
         mock = self.mocker.patch(
@@ -67,30 +81,31 @@
             type="git",
             snapshot=None,
         )
 
     @pytest.mark.parametrize(
         "failure_exception",
         [
-            IOError,
-            ObjectFormatException,
-            OSError,
-            ValueError,
-            GitProtocolError,
+            IOError("failure"),
+            ObjectFormatException("failure"),
+            OSError("failure"),
+            ValueError("failure"),
+            GitProtocolError("failure"),
+            GitProtocolError(ConnectionResetError("Connection reset by peer")),
         ],
     )
     def test_load_visit_failure(self, failure_exception):
         """Failing during the fetch pack step result in failing visit"""
         # simulate a fetch communication error after the initial connection
         # server error (e.g IOError, ObjectFormatException, ...)
         mock = self.mocker.patch(
             "swh.loader.git.loader.GitLoader.fetch_pack_from_origin"
         )
 
-        mock.side_effect = failure_exception("failure")
+        mock.side_effect = failure_exception
 
         res = self.loader.load()
         assert res == {"status": "failed"}
 
         assert_last_visit_matches(
             self.loader.storage,
             self.repo_url,
@@ -844,14 +859,15 @@
 
                 return super().load()
 
         # bare repository with dumb protocol only URL
         self.repo_url = f"http://{httpd.server_name}:{httpd.server_port}/{repo_name}"
         self.loader = DumbGitLoaderTest(swh_storage, self.repo_url)
         self.repo = repo
+        self.bare_repo_path = bare_repo_path
 
         yield
 
         # shutdown HTTP server
         httpd.shutdown()
         thread.join()
 
@@ -944,12 +960,90 @@
 
         mocker.patch.object(dumb, "GitObjectsFetcher", GitObjectsFetcherMissingPack)
 
         res = self.loader.load()
 
         assert res == {"status": "eventful"}
 
+    def test_http_get_retry(self, mocker):
+        sleep = mocker.patch.object(dumb.GitObjectsFetcher._http_get.retry, "sleep")
+        with requests_mock.Mocker(real_http=True) as http_mocker:
+            # mock requests for getting packs data
+            for root, _, files in os.walk(
+                os.path.join(self.bare_repo_path, "objects/pack")
+            ):
+                nb_files = len(files)
+                for pack in files:
+                    with open(os.path.join(root, pack), "rb") as pack_data:
+                        http_mocker.get(
+                            f"{self.repo_url}/objects/pack/{pack}",
+                            [
+                                # first request fails
+                                {"status_code": 502},
+                                # next one succeeds
+                                {"status_code": 200, "content": pack_data.read()},
+                            ],
+                        )
+
+            res = self.loader.load()
+            assert res == {"status": "eventful"}
+            sleep.assert_has_calls([mocker.call(param) for param in [1] * nb_files])
+
 
 class TestDumbGitLoaderWithoutPack(DumbGitLoaderTestBase):
     @classmethod
     def setup_class(cls):
         cls.with_pack_files = False
+
+
+def test_loader_too_large_pack_file_for_github_origin(
+    swh_storage, datadir, tmp_path, mocker, sentry_events
+):
+    archive_name = "testrepo"
+    archive_path = os.path.join(datadir, f"{archive_name}.tgz")
+    repo_url = prepare_repository_from_archive(
+        archive_path, archive_name, tmp_path=tmp_path
+    )
+
+    big_size_kib = 100 * 1024 * 1024
+
+    metadata = RawExtrinsicMetadata(
+        target=Origin(url=repo_url).swhid(),
+        discovery_date=datetime.datetime.now(datetime.timezone.utc),
+        authority=MetadataAuthority(
+            type=MetadataAuthorityType.FORGE, url="https://github.com", metadata=None
+        ),
+        fetcher=MetadataFetcher(
+            name="swh.loader.metadata.github", version="1.1.0", metadata=None
+        ),
+        format="application/vnd.github.v3+json",
+        metadata=f'{{"size": {big_size_kib}}}'.encode(),
+        origin=None,
+        visit=None,
+        snapshot=None,
+        release=None,
+        revision=None,
+        path=None,
+        directory=None,
+    )
+
+    loader = GitLoader(
+        swh_storage,
+        repo_url,
+        lister_name="github",
+        lister_instance_name="github",
+    )
+
+    mocker.patch.object(
+        loader,
+        "build_extrinsic_origin_metadata",
+        return_value=[metadata],
+    )
+
+    assert loader.load() == {"status": "failed"}
+
+    assert sentry_events
+    assert sentry_events[0]["level"] == "error"
+    assert sentry_events[0]["exception"]["values"][0]["value"] == (
+        f"Pack file too big for repository {repo_url}, "
+        f"limit is {loader.pack_size_bytes} bytes, current size is {big_size_kib*1024}"
+    )
```

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/test_tasks.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/tests/test_utils.py` & `swh.loader.git-2.3.0/swh/loader/git/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh/loader/git/utils.py` & `swh.loader.git-2.3.0/swh/loader/git/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/swh.loader.git.egg-info/PKG-INFO` & `swh.loader.git-2.3.0/swh.loader.git.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.2.0
+Version: 2.3.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
```

### Comparing `swh.loader.git-2.2.0/swh.loader.git.egg-info/SOURCES.txt` & `swh.loader.git-2.3.0/swh.loader.git.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.2.0/tox.ini` & `swh.loader.git-2.3.0/tox.ini`

 * *Files identical despite different names*

