# Comparing `tmp/riot-0.8.1.tar.gz` & `tmp/riot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riot-0.8.1.tar", last modified: Wed Oct 13 15:08:00 2021, max compression
+gzip compressed data, was "riot-0.9.0.tar", last modified: Fri Oct 15 18:52:18 2021, max compression
```

## Comparing `riot-0.8.1.tar` & `riot-0.9.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.539502 riot-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.523501 riot-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-13 15:07:51.000000 riot-0.8.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.523501 riot-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-10-13 15:07:51.000000 riot-0.8.1/.github/workflows/build_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-10-13 15:07:51.000000 riot-0.8.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-10-13 15:07:51.000000 riot-0.8.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-10-13 15:07:51.000000 riot-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-10-13 15:07:51.000000 riot-0.8.1/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-10-13 15:07:51.000000 riot-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2021-10-13 15:07:51.000000 riot-0.8.1/LICENSE.apache2
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-13 15:07:51.000000 riot-0.8.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-10-13 15:08:00.539502 riot-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      855 2021-10-13 15:07:51.000000 riot-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.527501 riot-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-13 15:07:51.000000 riot-0.8.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      712 2021-10-13 15:07:51.000000 riot-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-10-13 15:07:51.000000 riot-0.8.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-10-13 15:07:51.000000 riot-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-10-13 15:07:51.000000 riot-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-10-13 15:07:51.000000 riot-0.8.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-13 15:07:51.000000 riot-0.8.1/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-13 15:07:51.000000 riot-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-13 15:07:51.000000 riot-0.8.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-13 15:07:51.000000 riot-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.511501 riot-0.8.1/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.535502 riot-0.8.1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/add-exitfirst-option-to-run-7bd06dedf87c3180.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/add-version-info-405c35d8f62c7909.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/feat-create-95b0d328d14440e5.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/feature-skip-missing-a032464fbeafdc52.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/fix-parent-py-7de74544797e4d4d.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/fix-sitepkgs-3ef98bad9dc20f70.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/fix-spaces-cmdargs-16399f428692f9c4.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/inherit-pythonpath-from-parent-2f40e6c984d8e95a.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/passenv-always-some-var-27f2a854ab7f7752.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/shell-fix-d6fc7eb1127473e6.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-10-13 15:07:51.000000 riot-0.8.1/releasenotes/notes/use-system-shell-222f6711f7b17dd4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.535502 riot-0.8.1/riot/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-10-13 15:07:51.000000 riot-0.8.1/riot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-13 15:07:51.000000 riot-0.8.1/riot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3798 2021-10-13 15:07:51.000000 riot-0.8.1/riot/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 15:07:51.000000 riot-0.8.1/riot/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    29325 2021-10-13 15:07:51.000000 riot-0.8.1/riot/riot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.539502 riot-0.8.1/riot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2021-10-13 15:08:00.000000 riot-0.8.1/riot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-13 15:07:59.000000 riot-0.8.1/riot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-10-13 15:07:51.000000 riot-0.8.1/riotfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.539502 riot-0.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      918 2021-10-13 15:07:51.000000 riot-0.8.1/scripts/check-releasenotes
--rw-r--r--   0 runner    (1001) docker     (121)      750 2021-10-13 15:08:00.539502 riot-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2021-10-13 15:07:51.000000 riot-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.539502 riot-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 15:07:51.000000 riot-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-13 15:08:00.539502 riot-0.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-13 15:07:51.000000 riot-0.8.1/tests/data/empty_riotfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-10-13 15:07:51.000000 riot-0.8.1/tests/data/simple_riotfile.py
--rw-r--r--   0 runner    (1001) docker     (121)    16889 2021-10-13 15:07:51.000000 riot-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    17683 2021-10-13 15:07:51.000000 riot-0.8.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-10-13 15:07:51.000000 riot-0.8.1/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.452637 riot-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.444637 riot-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-15 18:52:08.000000 riot-0.9.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.444637 riot-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2021-10-15 18:52:08.000000 riot-0.9.0/.github/workflows/build_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2021-10-15 18:52:08.000000 riot-0.9.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1833 2021-10-15 18:52:08.000000 riot-0.9.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-10-15 18:52:08.000000 riot-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2021-10-15 18:52:08.000000 riot-0.9.0/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-10-15 18:52:08.000000 riot-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    11342 2021-10-15 18:52:08.000000 riot-0.9.0/LICENSE.apache2
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-10-15 18:52:08.000000 riot-0.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-10-15 18:52:18.452637 riot-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      855 2021-10-15 18:52:08.000000 riot-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.448637 riot-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-15 18:52:08.000000 riot-0.9.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2021-10-15 18:52:08.000000 riot-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-10-15 18:52:08.000000 riot-0.9.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2021-10-15 18:52:08.000000 riot-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2021-10-15 18:52:08.000000 riot-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-10-15 18:52:08.000000 riot-0.9.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-15 18:52:08.000000 riot-0.9.0/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-10-15 18:52:08.000000 riot-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-15 18:52:08.000000 riot-0.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-15 18:52:08.000000 riot-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.440637 riot-0.9.0/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.448637 riot-0.9.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/add-exitfirst-option-to-run-7bd06dedf87c3180.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/add-version-info-405c35d8f62c7909.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/feat-create-95b0d328d14440e5.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/feat-shell-command-5ec238da2ca192ad.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/feature-skip-missing-a032464fbeafdc52.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/fix-parent-py-7de74544797e4d4d.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/fix-sitepkgs-3ef98bad9dc20f70.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/fix-spaces-cmdargs-16399f428692f9c4.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/inherit-pythonpath-from-parent-2f40e6c984d8e95a.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/passenv-always-some-var-27f2a854ab7f7752.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/shell-fix-d6fc7eb1127473e6.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-10-15 18:52:08.000000 riot-0.9.0/releasenotes/notes/use-system-shell-222f6711f7b17dd4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.448637 riot-0.9.0/riot/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-10-15 18:52:08.000000 riot-0.9.0/riot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-15 18:52:08.000000 riot-0.9.0/riot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4686 2021-10-15 18:52:08.000000 riot-0.9.0/riot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:08.000000 riot-0.9.0/riot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    33422 2021-10-15 18:52:08.000000 riot-0.9.0/riot/riot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.452637 riot-0.9.0/riot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1555 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-15 18:52:18.000000 riot-0.9.0/riot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-10-15 18:52:08.000000 riot-0.9.0/riotfile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.452637 riot-0.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      918 2021-10-15 18:52:08.000000 riot-0.9.0/scripts/check-releasenotes
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2021-10-15 18:52:18.452637 riot-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2021-10-15 18:52:08.000000 riot-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.452637 riot-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:08.000000 riot-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:18.452637 riot-0.9.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-15 18:52:08.000000 riot-0.9.0/tests/data/empty_riotfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-10-15 18:52:08.000000 riot-0.9.0/tests/data/simple_riotfile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16973 2021-10-15 18:52:08.000000 riot-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18740 2021-10-15 18:52:08.000000 riot-0.9.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2021-10-15 18:52:08.000000 riot-0.9.0/tests/test_unit.py
```

### Comparing `riot-0.8.1/.github/workflows/build_deploy.yml` & `riot-0.9.0/.github/workflows/build_deploy.yml`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/.github/workflows/changelog.yml` & `riot-0.9.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/.github/workflows/main.yml` & `riot-0.9.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/.gitignore` & `riot-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/LICENSE.apache2` & `riot-0.9.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/PKG-INFO` & `riot-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riot
-Version: 0.8.1
+Version: 0.9.0
 Summary: A simple Python test runner runner.
 Home-page: https://github.com/DataDog/riot
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 License: Apache 2
 Description: # riot
```

### Comparing `riot-0.8.1/README.md` & `riot-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/docs/conf.py` & `riot-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/docs/configuration.rst` & `riot-0.9.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/docs/contributing.rst` & `riot-0.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/docs/index.rst` & `riot-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/docs/quickstart.rst` & `riot-0.9.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/riot/cli.py` & `riot-0.9.0/riot/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 __all__ = ["main"]
 
 import logging
 import re
 import sys
 
-
 import click
 import pkg_resources
+from rich.console import Console
+from rich.logging import RichHandler
 
 from .riot import Interpreter, Session
 
+FORMAT = "%(message)s"
+
 
 try:
     __version__ = pkg_resources.get_distribution("riot").version
 except pkg_resources.DistributionNotFound:
     # package is not installed
     __version__ = "dev"
 
@@ -49,36 +52,56 @@
     "riotfile",
     default="riotfile.py",
     show_default=True,
     type=click.Path(exists=True),
 )
 @click.option("-v", "--verbose", "log_level", flag_value=logging.INFO)
 @click.option("-d", "--debug", "log_level", flag_value=logging.DEBUG)
+@click.option(
+    "-P",
+    "--pipe",
+    "pipe_mode",
+    is_flag=True,
+    default=False,
+    help="Pipe mode. Makes riot emit plain output.",
+)
 @click.version_option(__version__)
 @click.pass_context
-def main(ctx, riotfile, log_level):
-    if log_level:
-        logging.basicConfig(level=log_level)
+def main(ctx, riotfile, log_level, pipe_mode):
+    if pipe_mode:
+        if log_level:
+            logging.basicConfig(level=log_level)
+    else:
+        logging.basicConfig(
+            level=log_level or logging.WARNING,
+            format=FORMAT,
+            datefmt="[%X]",
+            handlers=[RichHandler(console=Console(stderr=True))],
+        )
 
     ctx.ensure_object(dict)
+    ctx.obj["pipe"] = pipe_mode
     try:
         ctx.obj["session"] = Session.from_config_file(riotfile)
     except Exception as e:
         click.echo(f"Failed to construct config file:\n{str(e)}", err=True)
         sys.exit(1)
 
 
 @main.command("list", help="""List all virtual env instances matching a pattern.""")
 @PYTHON_VERSIONS_ARG
 @PATTERN_ARG
 @VENV_PATTERN_ARG
 @click.pass_context
 def list_venvs(ctx, pythons, pattern, venv_pattern):
     ctx.obj["session"].list_venvs(
-        re.compile(pattern), re.compile(venv_pattern), pythons=pythons
+        re.compile(pattern),
+        re.compile(venv_pattern),
+        pythons=pythons,
+        pipe_mode=ctx.obj["pipe"],
     )
 
 
 @main.command(
     help="""Generate base virtual environments.
 
 A base virtual environment is a virtual environment with the local package
@@ -135,7 +158,18 @@
         skip_base_install=skip_base_install,
         pass_env=pass_env,
         cmdargs=ctx.args,
         pythons=pythons,
         skip_missing=skip_missing,
         exit_first=exit_first,
     )
+
+
+@main.command("shell", help="""Launch a shell inside a venv.""")
+@click.argument("ident", type=str)
+@click.option("--pass-env", "pass_env", is_flag=True, default=False)
+@click.pass_context
+def shell(ctx, ident, pass_env):
+    ctx.obj["session"].shell(
+        ident=ident,
+        pass_env=pass_env,
+    )
```

### Comparing `riot-0.8.1/riot/riot.py` & `riot-0.9.0/riot/riot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 from contextlib import contextmanager
 import dataclasses
 import functools
+from hashlib import sha256
 import importlib.abc
 import importlib.util
 import itertools
 import logging
 import os
 import shutil
 import subprocess
 import sys
+import tempfile
 import traceback
 import typing as t
 
 import click
+from rich import print as rich_print
+from rich.pretty import Pretty
+from rich.status import Status
+from rich.table import Table
 
 logger = logging.getLogger(__name__)
 
 SHELL = os.getenv("SHELL", "/bin/bash")
 ENCODING = sys.getdefaultencoding()
+SHELL_RCFILE = """
+if [ -f ~/.bashrc ]; then . ~/.bashrc; fi
+source {venv_path}/bin/activate
+echo -e "\e[31;1m"
+echo "                 )  "
+echo " (   (        ( /(  "
+echo " )(  )\   (   )\()) "
+echo "(()\((_)  )\ (_))/  "
+echo " ((_)(_) ((_)| |_   "
+echo "| '_|| |/ _ \|  _|  "
+echo "|_|  |_|\___/ \__|  "
+echo -e "\e[0m"
+echo -e "\e[33;1mInteractive shell\e[0m"
+echo ""
+echo -e "* Venv name   : \e[1m{name}\e[0m"
+echo -e "* Venv path   : \e[1m{venv_path}\e[0m"
+echo -e "* Interpreter : \e[1m$( python -V )\e[0m"
+PS1="\n(\e[31;1mriot\e[0m@\e[33;1m`basename {venv_path}`\e[0m) \e[36;1m\h\e[0m:\e[32;1m\w\e[0m\n🔥 "
+"""
 
 
 if t.TYPE_CHECKING or sys.version_info[:2] >= (3, 9):
     _T_CompletedProcess = subprocess.CompletedProcess[str]
 else:
     _T_CompletedProcess = subprocess.CompletedProcess
 
@@ -345,15 +370,18 @@
 
     @property
     def ident(self) -> t.Optional[str]:
         """Return prefix identifier string based on packages."""
         if not self.pkgs:
             return None
         return "_".join(
-            (f"{n}{rmchars('<=>.,', v)}" for n, v in sorted(self.pkgs.items()))
+            (
+                f"{rmchars('<=>.,:+@/', n)}{rmchars('<=>.,:+@/', v)}"
+                for n, v in self.pkgs.items()
+            )
         )
 
     @property
     def pkg_str(self) -> str:
         """Return pip friendly install string from defined packages."""
         return pip_deps(self.pkgs)
 
@@ -368,14 +396,21 @@
 
         pkgs: t.Dict[str, str] = {}
         for inst in chain:
             pkgs.update(dict(inst.pkgs))
 
         return pip_deps(pkgs)
 
+    def __hash__(self):
+        """Compute a hash for the venv instance."""
+        h = sha256()
+        h.update(repr(self).encode())
+        h.update(self.full_pkg_str.encode())
+        return int(h.hexdigest(), 16)
+
     @property
     def bin_path(self) -> t.Optional[str]:
         prefix = self.prefix
         if prefix is None:
             return None
         return os.path.join(prefix, "bin")
 
@@ -712,28 +747,56 @@
 
         s_num = f"{num_passed} passed with {num_warnings} warnings, {num_failed} failed"
         click.echo(click.style(s_num, fg="blue", bold=True))
 
         if any(True for r in results if r.code != 0):
             sys.exit(1)
 
-    def list_venvs(self, pattern, venv_pattern, pythons=None, out=sys.stdout):
-        for inst in self.venv.instances():
+    def list_venvs(
+        self, pattern, venv_pattern, pythons=None, out=sys.stdout, pipe_mode=False
+    ):
+        table = None
+        if not pipe_mode:
+            table = Table(
+                "No.",
+                "Hash",
+                "Name",
+                "Interpreter",
+                "Environment",
+                "Packages",
+                box=None,
+            )
+
+        for n, inst in enumerate(self.venv.instances()):
             if not inst.name or not pattern.match(inst.name):
                 continue
 
             if pythons and inst.py not in pythons:
                 continue
 
             if not inst.match_venv_pattern(venv_pattern):
                 continue
             pkgs_str = inst.full_pkg_str
             env_str = env_to_str(inst.env)
-            py_str = f"Python {inst.py}"
-            click.echo(f"{inst.name} {env_str} {py_str} {pkgs_str}")
+            if pipe_mode:
+                print(
+                    f"[#{n}]  {hex(hash(inst))[2:9]}  {inst.name:12} {env_str} {inst.py} Packages({pkgs_str})"
+                )
+            else:
+                table.add_row(
+                    f"[cyan]#{n}[/cyan]",
+                    f"[bold cyan]{hex(hash(inst))[2:9]}[/bold cyan]",
+                    f"[bold]{inst.name}[/bold]",
+                    Pretty(inst.py),
+                    env_str or "--",
+                    f"[italic]{pkgs_str}[/italic]",
+                )
+
+        if table:
+            rich_print(table)
 
     def generate_base_venvs(
         self,
         pattern: t.Pattern[str],
         recreate: bool,
         skip_deps: bool,
         pythons: t.Optional[t.Set[Interpreter]],
@@ -767,14 +830,77 @@
                 if skip_deps:
                     logger.info("Skipping global deps install.")
                     continue
 
                 # Install the dev package into the base venv.
                 install_dev_pkg(venv_path)
 
+    def _generate_shell_rcfile(self):
+        with tempfile.NamedTemporaryFile() as rcfile:
+            rcfile.write()
+            rcfile.flush()
+
+    def shell(self, ident, pass_env):
+        for n, inst in enumerate(self.venv.instances()):
+            if ident != f"#{n}" and not hex(hash(inst))[2:].startswith(ident):
+                continue
+
+            assert inst.py is not None, inst
+            try:
+                venv_path = inst.py.venv_path
+            except FileNotFoundError:
+                raise RuntimeError("%s not available" % inst.py)
+
+            logger.info("Launching shell inside venv instance %s", inst)
+
+            # Generate the environment for the instance.
+            if pass_env:
+                env = os.environ.copy()
+                env.update(dict(inst.env))
+            else:
+                env = dict(inst.env)
+
+            # Should we expect the venv to be ready?
+            with Status("Preparing shell virtual environment"):
+                inst.py.create_venv(False)
+                inst.prepare(env)
+
+            pythonpath = inst.pythonpath
+            if pythonpath:
+                env["PYTHONPATH"] = (
+                    f"{pythonpath}:{env['PYTHONPATH']}"
+                    if "PYTHONPATH" in env
+                    else pythonpath
+                )
+            script_path = inst.scriptpath
+            if script_path:
+                env["PATH"] = ":".join(
+                    (script_path, env.get("PATH", os.environ["PATH"]))
+                )
+
+            with nspkgs(inst):
+                pid = os.fork()
+                if pid == 0:
+                    with tempfile.NamedTemporaryFile() as rcfile:
+                        rcfile.write(
+                            SHELL_RCFILE.format(
+                                venv_path=venv_path, name=inst.name
+                            ).encode()
+                        )
+                        rcfile.flush()
+                        os.execvpe("bash", ["bash", "--rcfile", rcfile.name], env)
+                os.wait()
+
+            break
+        else:
+            logger.error(
+                "No venv instance found for %s. Use 'riot list' to get a list of valid numbers.",
+                ident,
+            )
+
     @classmethod
     def run_cmd_venv(
         cls,
         venv: str,
         args: str,
         stdout: _T_stdio = subprocess.PIPE,
         executable: t.Optional[str] = None,
```

### Comparing `riot-0.8.1/riot.egg-info/PKG-INFO` & `riot-0.9.0/riot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riot
-Version: 0.8.1
+Version: 0.9.0
 Summary: A simple Python test runner runner.
 Home-page: https://github.com/DataDog/riot
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 License: Apache 2
 Description: # riot
```

### Comparing `riot-0.8.1/riot.egg-info/SOURCES.txt` & `riot-0.9.0/riot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/quickstart.rst
 docs/release_notes.rst
 docs/requirements.txt
 docs/usage.rst
 releasenotes/notes/add-exitfirst-option-to-run-7bd06dedf87c3180.yaml
 releasenotes/notes/add-version-info-405c35d8f62c7909.yaml
 releasenotes/notes/feat-create-95b0d328d14440e5.yaml
+releasenotes/notes/feat-shell-command-5ec238da2ca192ad.yaml
 releasenotes/notes/feature-skip-missing-a032464fbeafdc52.yaml
 releasenotes/notes/fix-parent-py-7de74544797e4d4d.yaml
 releasenotes/notes/fix-sitepkgs-3ef98bad9dc20f70.yaml
 releasenotes/notes/fix-spaces-cmdargs-16399f428692f9c4.yaml
 releasenotes/notes/inherit-pythonpath-from-parent-2f40e6c984d8e95a.yaml
 releasenotes/notes/passenv-always-some-var-27f2a854ab7f7752.yaml
 releasenotes/notes/shell-fix-d6fc7eb1127473e6.yaml
```

### Comparing `riot-0.8.1/riotfile.py` & `riot-0.9.0/riotfile.py`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/scripts/check-releasenotes` & `riot-0.9.0/scripts/check-releasenotes`

 * *Files identical despite different names*

### Comparing `riot-0.8.1/setup.cfg` & `riot-0.9.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 application-import-name = riot
 exclude = 
 	.riot,
 	.git,
 	__pycache__,
 	*.eggs*,
 	build,
-ignore = E501,W503,E231,G201,D100,D101,D102,D103,D104,D107,B902
+ignore = E501,W503,E231,G201,D100,D101,D102,D103,D104,D107,B902,W605
 enable-extensions = G
 import-order-style = google
 
 [mypy]
 ignore_missing_imports = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
```

### Comparing `riot-0.8.1/setup.py` & `riot-0.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     packages=find_packages(exclude=["tests*"]),
     package_data={"riot": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
         "dataclasses; python_version<'3.7'",
         "click>=7,<8",
         "virtualenv",
+        "rich",
     ],
     setup_requires=["setuptools_scm"],
     use_scm_version=True,
     # Required for mypy compatibility, see
     # https://mypy.readthedocs.io/en/stable/installed_packages.html#making-pep-561-compatible-packages
     zip_safe=False,
 )
```

### Comparing `riot-0.8.1/tests/test_cli.py` & `riot-0.9.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,24 +57,28 @@
 
 def test_list_with_venv_pattern(cli: click.testing.CliRunner) -> None:
     """Running list with a venv pattern passes."""
     with with_riotfile(cli, "simple_riotfile.py"):
         result = cli.invoke(
             riot.cli.main,
             [
+                "-P",
                 "list",
                 "test",
                 "--venv-pattern",
                 "pytest543$",
             ],
         )
         if result.exception:
             raise result.exception
         assert result.exit_code == 0, result.stdout
-        assert result.stdout == "test  Python Interpreter(_hint='3') 'pytest==5.4.3'\n"
+        assert (
+            result.stdout
+            == "[#0]  4375064  test          Interpreter(_hint='3') Packages('pytest==5.4.3')\n"
+        )
 
 
 def test_list_with_python(cli: click.testing.CliRunner) -> None:
     """Running list with a python passes through the python."""
     with mock.patch("riot.cli.Session.list_venvs") as list_venvs:
         with with_riotfile(cli, "empty_riotfile.py"):
             result = cli.invoke(riot.cli.main, ["list", "--python", "3.6"])
```

### Comparing `riot-0.8.1/tests/test_integration.py` & `riot-0.9.0/tests/test_integration.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,27 +59,29 @@
         == """
 Usage: riot [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -f, --file PATH  [default: riotfile.py]
   -v, --verbose
   -d, --debug
+  -P, --pipe       Pipe mode. Makes riot emit plain output.
   --version        Show the version and exit.
   --help           Show this message and exit.
 
 Commands:
   generate  Generate base virtual environments.
   list      List all virtual env instances matching a pattern.
   run       Run virtualenv instances with names matching a pattern.
+  shell     Launch a shell inside a venv.
 """.lstrip()
     )
     assert result.stderr == ""
     assert result.returncode == 0
 
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert (
         result.stderr
         == """
 Usage: riot [OPTIONS] COMMAND [ARGS]...
 Try 'riot --help' for help.
 
 Error: Invalid value for '-f' / '--file': Path 'riotfile.py' does not exist.
@@ -150,36 +152,38 @@
         == """
 Usage: riot [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -f, --file PATH  [default: riotfile.py]
   -v, --verbose
   -d, --debug
+  -P, --pipe       Pipe mode. Makes riot emit plain output.
   --version        Show the version and exit.
   --help           Show this message and exit.
 
 Commands:
   generate  Generate base virtual environments.
   list      List all virtual env instances matching a pattern.
   run       Run virtualenv instances with names matching a pattern.
+  shell     Launch a shell inside a venv.
 """.lstrip()
     )
     assert result.stderr == ""
     assert result.returncode == 0
 
 
 def test_version(tmp_run: _T_TmpRun) -> None:
     result = tmp_run("riot --version")
     assert result.stdout.startswith("riot, version ")
     assert result.stderr == ""
     assert result.returncode == 0
 
 
 def test_list_no_file_empty_file(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert (
         result.stderr
         == """
 Usage: riot [OPTIONS] COMMAND [ARGS]...
 Try 'riot --help' for help.
 
 Error: Invalid value for '-f' / '--file': Path 'riotfile.py' does not exist.
@@ -189,15 +193,15 @@
 
     rf_path = tmp_path / "riotfile.py"
     rf_path.write_text(
         """
 from riot import Venv
 """,
     )
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert result.stderr == ""
     assert result.stdout == ""
     assert result.returncode == 0
 
 
 def test_list_configurations(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
     rf_path = tmp_path / "riotfile.py"
@@ -207,17 +211,20 @@
 venv = Venv(
     name="test",
     pys=[3],
     command="echo hi",
 )
 """,
     )
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert result.stderr == ""
-    assert result.stdout == "test  Python Interpreter(_hint='3') \n"
+    assert (
+        result.stdout
+        == "[#0]  1c31170  test          Interpreter(_hint='3') Packages()\n"
+    )
     assert result.returncode == 0
 
     rf_path.write_text(
         """
 from riot import Venv
 venv = Venv(
     name="test",
@@ -225,20 +232,20 @@
     command="echo hi",
     pkgs={
         "pkg1": ["==1.0", "==2.0"],
     }
 )
 """,
     )
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert result.stderr == ""
     assert re.search(
         r"""
-test  .* 'pkg1==1.0'
-test  .* 'pkg1==2.0'
+\[\#0\]  [0-9a-f]{7}  test  .* Packages\('pkg1==1.0'\)
+\[\#1\]  [0-9a-f]{7}  test  .* Packages\('pkg1==2.0'\)
 """.lstrip(),
         result.stdout,
     )
     assert result.returncode == 0
 
     rf_path.write_text(
         """
@@ -250,22 +257,22 @@
     pkgs={
         "pkg1": ["==1.0", "==2.0"],
         "pkg2": ["==2.0", "==3.0"],
     }
 )
 """,
     )
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert result.stderr == ""
     assert re.search(
         r"""
-test  .* 'pkg1==1.0' 'pkg2==2.0'
-test  .* 'pkg1==1.0' 'pkg2==3.0'
-test  .* 'pkg1==2.0' 'pkg2==2.0'
-test  .* 'pkg1==2.0' 'pkg2==3.0'
+\[\#0\]  [0-9a-f]{7}  test  .* Packages\('pkg1==1.0' 'pkg2==2.0'\)
+\[\#1\]  [0-9a-f]{7}  test  .* Packages\('pkg1==1.0' 'pkg2==3.0'\)
+\[\#2\]  [0-9a-f]{7}  test  .* Packages\('pkg1==2.0' 'pkg2==2.0'\)
+\[\#3\]  [0-9a-f]{7}  test  .* Packages\('pkg1==2.0' 'pkg2==3.0'\)
 """.lstrip(),
         result.stdout,
     )
     assert result.returncode == 0
 
     rf_path.write_text(
         """
@@ -289,26 +296,26 @@
                 "pkg2": ["==3.0", "==4.0"],
             }
         ),
     ]
 )
 """,
     )
-    result = tmp_run("riot list")
+    result = tmp_run("riot -P list")
     assert result.stderr == ""
     assert re.search(
         r"""
-test1  .* 'pkg1==1.0' 'pkg2==3.0'
-test1  .* 'pkg1==1.0' 'pkg2==4.0'
-test1  .* 'pkg1==2.0' 'pkg2==3.0'
-test1  .* 'pkg1==2.0' 'pkg2==4.0'
-test2  .* 'pkg1==1.0' 'pkg2==3.0'
-test2  .* 'pkg1==1.0' 'pkg2==4.0'
-test2  .* 'pkg1==2.0' 'pkg2==3.0'
-test2  .* 'pkg1==2.0' 'pkg2==4.0'
+\[\#0\]  [0-9a-f]{7}  test1  .* Packages\('pkg1==1.0' 'pkg2==3.0'\)
+\[\#1\]  [0-9a-f]{7}  test1  .* Packages\('pkg1==1.0' 'pkg2==4.0'\)
+\[\#2\]  [0-9a-f]{7}  test1  .* Packages\('pkg1==2.0' 'pkg2==3.0'\)
+\[\#3\]  [0-9a-f]{7}  test1  .* Packages\('pkg1==2.0' 'pkg2==4.0'\)
+\[\#4\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==1.0' 'pkg2==3.0'\)
+\[\#5\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==1.0' 'pkg2==4.0'\)
+\[\#6\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==2.0' 'pkg2==3.0'\)
+\[\#7\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==2.0' 'pkg2==4.0'\)
 """.lstrip(),
         result.stdout,
     )
     assert result.returncode == 0
 
 
 def test_list_filter(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
@@ -319,15 +326,15 @@
 venv = Venv(
     name="test",
     pys=[3],
     command="echo hi",
 )
 """,
     )
-    result = tmp_run("riot list test")
+    result = tmp_run("riot -P list test")
     assert result.stderr == ""
     assert re.search(r"test .*", result.stdout)
     assert result.returncode == 0
 
     rf_path.write_text(
         """
 from riot import Venv
@@ -338,22 +345,22 @@
     pkgs={
         "pkg1": ["==1.0", "==2.0"],
         "pkg2": ["==2.0", "==3.0"],
     }
 )
 """,
     )
-    result = tmp_run("riot list test")
+    result = tmp_run("riot -P list test")
     assert result.stderr == ""
     assert re.search(
         r"""
-test  .* 'pkg1==1.0' 'pkg2==2.0'
-test  .* 'pkg1==1.0' 'pkg2==3.0'
-test  .* 'pkg1==2.0' 'pkg2==2.0'
-test  .* 'pkg1==2.0' 'pkg2==3.0'
+\[\#0\]  [0-9a-f]{7}  test  .* Packages\('pkg1==1.0' 'pkg2==2.0'\)
+\[\#1\]  [0-9a-f]{7}  test  .* Packages\('pkg1==1.0' 'pkg2==3.0'\)
+\[\#2\]  [0-9a-f]{7}  test  .* Packages\('pkg1==2.0' 'pkg2==2.0'\)
+\[\#3\]  [0-9a-f]{7}  test  .* Packages\('pkg1==2.0' 'pkg2==3.0'\)
 """.lstrip(),
         result.stdout,
     )
     assert result.returncode == 0
 
     rf_path.write_text(
         """
@@ -377,22 +384,22 @@
                 "pkg2": ["==3.0", "==4.0"],
             }
         ),
     ]
 )
 """,
     )
-    result = tmp_run("riot list test2")
+    result = tmp_run("riot -P list test2")
     assert result.stderr == ""
     assert re.search(
         r"""
-test2  .* 'pkg1==1.0' 'pkg2==3.0'
-test2  .* 'pkg1==1.0' 'pkg2==4.0'
-test2  .* 'pkg1==2.0' 'pkg2==3.0'
-test2  .* 'pkg1==2.0' 'pkg2==4.0'
+\[\#4\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==1.0' 'pkg2==3.0'\)
+\[\#5\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==1.0' 'pkg2==4.0'\)
+\[\#6\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==2.0' 'pkg2==3.0'\)
+\[\#7\]  [0-9a-f]{7}  test2  .* Packages\('pkg1==2.0' 'pkg2==4.0'\)
 """.lstrip(),
         result.stdout,
     )
     assert result.returncode == 0
 
 
 def test_run(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
@@ -502,17 +509,16 @@
     pys=3,
     name="test",
     command="echo hello",
 )
 """,
     )
     result = tmp_run("riot run test")
-    assert 'ERROR: File "setup.py"' in result.stderr
-    assert "Dev install failed, aborting!" in result.stderr
-    assert result.stdout == ""
+    assert 'File "setup.py"' in result.stderr, result.stderr
+    assert "Dev install failed, aborting!" in result.stderr, result.stderr
     assert result.returncode == 1
 
 
 def test_bad_interpreter(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
     rf_path = tmp_path / "riotfile.py"
     rf_path.write_text(
         """
@@ -527,15 +533,14 @@
     result = tmp_run("riot run -s -pDNE test")
     assert (
         """
 FileNotFoundError: Python interpreter DNE not found
 """.strip()
         in result.stderr
     )
-    assert result.stdout == ""
     assert result.returncode == 1
 
 
 def test_interpreter_pythonpath(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
     rf_path = tmp_path / "riotfile.py"
     rf_path.write_text(
         """
@@ -720,20 +725,22 @@
             create=True,
             command="echo $PYTHONPATH",
         ),
     ],
 )
 """,
     )
-    result = tmp_run("riot -v run -s child")
-    venv_path = tmp_path / ".riot/venv_py{}_pip_pytest".format(
+    result = tmp_run("riot -Pv run -s child")
+    venv_path = tmp_path / ".riot/venv_py{}_pytest_pip".format(
         "".join((str(_) for _ in sys.version_info[:3]))
     )
-    assert f"Creating virtualenv '{venv_path}'" in result.stderr
-    assert f"Running command 'echo $PYTHONPATH' in venv '{venv_path}'"
+    assert f"Creating virtualenv '{venv_path}'" in result.stderr, result.stderr
+    assert (
+        f"Running command 'echo $PYTHONPATH' in venv '{venv_path}'" in result.stderr
+    ), result.stderr
     assert result.stdout.startswith(":".join(("", str(tmp_path))))
     assert result.returncode == 0
 
 
 def test_extras(tmp_path: pathlib.Path, tmp_run: _T_TmpRun) -> None:
     rf_path = tmp_path / "riotfile.py"
     rf_path.write_text(
```

### Comparing `riot-0.8.1/tests/test_unit.py` & `riot-0.9.0/tests/test_unit.py`

 * *Files identical despite different names*

