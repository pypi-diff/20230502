# Comparing `tmp/trade-republic-api-0.0.0.tar.gz` & `tmp/trade-republic-api-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trade-republic-api-0.0.0.tar", last modified: Mon May  1 21:39:18 2023, max compression
+gzip compressed data, was "trade-republic-api-0.0.1.tar", last modified: Mon May  1 22:54:02 2023, max compression
```

## Comparing `trade-republic-api-0.0.0.tar` & `trade-republic-api-0.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.366816 trade-republic-api-0.0.0/
--rw-r--r--   0 unimun     (502) staff       (20)      638 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.bumpversion.cfg
--rw-r--r--   0 unimun     (502) staff       (20)     2084 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.cookiecutterrc
--rw-r--r--   0 unimun     (502) staff       (20)      186 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.coveragerc
--rw-r--r--   0 unimun     (502) staff       (20)      353 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.editorconfig
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.348307 trade-republic-api-0.0.0/.github/
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.355426 trade-republic-api-0.0.0/.github/workflows/
--rw-r--r--   0 unimun     (502) staff       (20)     5793 2023-05-01 20:32:06.000000 trade-republic-api-0.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 unimun     (502) staff       (20)      684 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0 unimun     (502) staff       (20)      231 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/.readthedocs.yml
--rw-r--r--   0 unimun     (502) staff       (20)       55 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/AUTHORS.rst
--rw-r--r--   0 unimun     (502) staff       (20)       86 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/CHANGELOG.rst
--rw-r--r--   0 unimun     (502) staff       (20)     2392 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/CONTRIBUTING.rst
--rw-r--r--   0 unimun     (502) staff       (20)     1320 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/LICENSE
--rw-r--r--   0 unimun     (502) staff       (20)      443 2023-05-01 21:14:16.000000 trade-republic-api-0.0.0/MANIFEST.in
--rw-r--r--   0 unimun     (502) staff       (20)     2215 2023-05-01 21:39:18.366530 trade-republic-api-0.0.0/PKG-INFO
--rw-r--r--   0 unimun     (502) staff       (20)      178 2023-05-01 20:42:37.000000 trade-republic-api-0.0.0/Pipfile
--rw-r--r--   0 unimun     (502) staff       (20)     2547 2023-05-01 21:17:18.000000 trade-republic-api-0.0.0/README.rst
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.356532 trade-republic-api-0.0.0/ci/
--rwxr-xr-x   0 unimun     (502) staff       (20)     2861 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/ci/bootstrap.py
--rw-r--r--   0 unimun     (502) staff       (20)       72 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/ci/requirements.txt
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.348704 trade-republic-api-0.0.0/ci/templates/
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.348801 trade-republic-api-0.0.0/ci/templates/.github/
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.357080 trade-republic-api-0.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 unimun     (502) staff       (20)     2145 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.361400 trade-republic-api-0.0.0/docs/
--rw-r--r--   0 unimun     (502) staff       (20)       28 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/authors.rst
--rw-r--r--   0 unimun     (502) staff       (20)       30 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/changelog.rst
--rw-r--r--   0 unimun     (502) staff       (20)     1163 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/conf.py
--rw-r--r--   0 unimun     (502) staff       (20)       33 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/contributing.rst
--rw-r--r--   0 unimun     (502) staff       (20)      244 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/index.rst
--rw-r--r--   0 unimun     (502) staff       (20)       98 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/installation.rst
--rw-r--r--   0 unimun     (502) staff       (20)       27 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/readme.rst
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.362283 trade-republic-api-0.0.0/docs/reference/
--rw-r--r--   0 unimun     (502) staff       (20)       70 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/reference/index.rst
--rw-r--r--   0 unimun     (502) staff       (20)      142 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/reference/trade_republic_api.rst
--rw-r--r--   0 unimun     (502) staff       (20)       29 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/requirements.txt
--rw-r--r--   0 unimun     (502) staff       (20)      109 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 unimun     (502) staff       (20)       88 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/docs/usage.rst
--rw-r--r--   0 unimun     (502) staff       (20)     1207 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/pyproject.toml
--rw-r--r--   0 unimun     (502) staff       (20)      783 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/pytest.ini
--rw-r--r--   0 unimun     (502) staff       (20)       38 2023-05-01 21:39:18.366898 trade-republic-api-0.0.0/setup.cfg
--rwxr-xr-x   0 unimun     (502) staff       (20)     2888 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/setup.py
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.349447 trade-republic-api-0.0.0/src/
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.363413 trade-republic-api-0.0.0/src/trade_republic_api/
--rw-r--r--   0 unimun     (502) staff       (20)       22 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/src/trade_republic_api/__init__.py
--rw-r--r--   0 unimun     (502) staff       (20)      383 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/src/trade_republic_api/__main__.py
--rw-r--r--   0 unimun     (502) staff       (20)      768 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/src/trade_republic_api/cli.py
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.365806 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/
--rw-r--r--   0 unimun     (502) staff       (20)     2215 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/PKG-INFO
--rw-r--r--   0 unimun     (502) staff       (20)     1054 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/SOURCES.txt
--rw-r--r--   0 unimun     (502) staff       (20)        1 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/dependency_links.txt
--rw-r--r--   0 unimun     (502) staff       (20)       67 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/entry_points.txt
--rw-r--r--   0 unimun     (502) staff       (20)        1 2023-05-01 20:43:31.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/not-zip-safe
--rw-r--r--   0 unimun     (502) staff       (20)        6 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/requires.txt
--rw-r--r--   0 unimun     (502) staff       (20)       19 2023-05-01 21:39:18.000000 trade-republic-api-0.0.0/src/trade_republic_api.egg-info/top_level.txt
-drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 21:39:18.366125 trade-republic-api-0.0.0/tests/
--rw-r--r--   0 unimun     (502) staff       (20)      227 2023-05-01 21:14:38.000000 trade-republic-api-0.0.0/tests/test_trade_republic_api.py
--rw-r--r--   0 unimun     (502) staff       (20)     1674 2023-05-01 20:32:00.000000 trade-republic-api-0.0.0/tox.ini
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.328472 trade-republic-api-0.0.1/
+-rw-r--r--   0 unimun     (502) staff       (20)      638 2023-05-01 22:38:29.000000 trade-republic-api-0.0.1/.bumpversion.cfg
+-rw-r--r--   0 unimun     (502) staff       (20)     2084 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/.cookiecutterrc
+-rw-r--r--   0 unimun     (502) staff       (20)      186 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/.coveragerc
+-rw-r--r--   0 unimun     (502) staff       (20)      353 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/.editorconfig
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.310036 trade-republic-api-0.0.1/.github/
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.317320 trade-republic-api-0.0.1/.github/workflows/
+-rw-r--r--   0 unimun     (502) staff       (20)     5704 2023-05-01 22:14:08.000000 trade-republic-api-0.0.1/.github/workflows/github-actions.yml
+-rw-r--r--   0 unimun     (502) staff       (20)      684 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 unimun     (502) staff       (20)      231 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/.readthedocs.yml
+-rw-r--r--   0 unimun     (502) staff       (20)       55 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/AUTHORS.rst
+-rw-r--r--   0 unimun     (502) staff       (20)       86 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/CHANGELOG.rst
+-rw-r--r--   0 unimun     (502) staff       (20)     2392 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 unimun     (502) staff       (20)     1320 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/LICENSE
+-rw-r--r--   0 unimun     (502) staff       (20)      443 2023-05-01 21:14:16.000000 trade-republic-api-0.0.1/MANIFEST.in
+-rw-r--r--   0 unimun     (502) staff       (20)     2215 2023-05-01 22:54:02.328179 trade-republic-api-0.0.1/PKG-INFO
+-rw-r--r--   0 unimun     (502) staff       (20)      178 2023-05-01 20:42:37.000000 trade-republic-api-0.0.1/Pipfile
+-rw-r--r--   0 unimun     (502) staff       (20)     2547 2023-05-01 22:38:29.000000 trade-republic-api-0.0.1/README.rst
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.318063 trade-republic-api-0.0.1/ci/
+-rwxr-xr-x   0 unimun     (502) staff       (20)     2861 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/ci/bootstrap.py
+-rw-r--r--   0 unimun     (502) staff       (20)       72 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/ci/requirements.txt
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.310429 trade-republic-api-0.0.1/ci/templates/
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.310526 trade-republic-api-0.0.1/ci/templates/.github/
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.318412 trade-republic-api-0.0.1/ci/templates/.github/workflows/
+-rw-r--r--   0 unimun     (502) staff       (20)     2145 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.323443 trade-republic-api-0.0.1/docs/
+-rw-r--r--   0 unimun     (502) staff       (20)       28 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/authors.rst
+-rw-r--r--   0 unimun     (502) staff       (20)       30 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/changelog.rst
+-rw-r--r--   0 unimun     (502) staff       (20)     1163 2023-05-01 22:38:29.000000 trade-republic-api-0.0.1/docs/conf.py
+-rw-r--r--   0 unimun     (502) staff       (20)       33 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/contributing.rst
+-rw-r--r--   0 unimun     (502) staff       (20)      244 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/index.rst
+-rw-r--r--   0 unimun     (502) staff       (20)       98 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/installation.rst
+-rw-r--r--   0 unimun     (502) staff       (20)       27 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/readme.rst
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.324150 trade-republic-api-0.0.1/docs/reference/
+-rw-r--r--   0 unimun     (502) staff       (20)       70 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/reference/index.rst
+-rw-r--r--   0 unimun     (502) staff       (20)      142 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/reference/trade_republic_api.rst
+-rw-r--r--   0 unimun     (502) staff       (20)       29 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/requirements.txt
+-rw-r--r--   0 unimun     (502) staff       (20)      109 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 unimun     (502) staff       (20)       88 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/docs/usage.rst
+-rw-r--r--   0 unimun     (502) staff       (20)     1207 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/pyproject.toml
+-rw-r--r--   0 unimun     (502) staff       (20)      783 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/pytest.ini
+-rw-r--r--   0 unimun     (502) staff       (20)       38 2023-05-01 22:54:02.328558 trade-republic-api-0.0.1/setup.cfg
+-rwxr-xr-x   0 unimun     (502) staff       (20)     2888 2023-05-01 22:38:29.000000 trade-republic-api-0.0.1/setup.py
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.311153 trade-republic-api-0.0.1/src/
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.325157 trade-republic-api-0.0.1/src/trade_republic_api/
+-rw-r--r--   0 unimun     (502) staff       (20)       22 2023-05-01 22:38:29.000000 trade-republic-api-0.0.1/src/trade_republic_api/__init__.py
+-rw-r--r--   0 unimun     (502) staff       (20)      383 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/src/trade_republic_api/__main__.py
+-rw-r--r--   0 unimun     (502) staff       (20)      768 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/src/trade_republic_api/cli.py
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.327526 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/
+-rw-r--r--   0 unimun     (502) staff       (20)     2215 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/PKG-INFO
+-rw-r--r--   0 unimun     (502) staff       (20)     1054 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 unimun     (502) staff       (20)        1 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 unimun     (502) staff       (20)       67 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/entry_points.txt
+-rw-r--r--   0 unimun     (502) staff       (20)        1 2023-05-01 20:43:31.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/not-zip-safe
+-rw-r--r--   0 unimun     (502) staff       (20)        6 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/requires.txt
+-rw-r--r--   0 unimun     (502) staff       (20)       19 2023-05-01 22:54:02.000000 trade-republic-api-0.0.1/src/trade_republic_api.egg-info/top_level.txt
+drwxr-xr-x   0 unimun     (502) staff       (20)        0 2023-05-01 22:54:02.327801 trade-republic-api-0.0.1/tests/
+-rw-r--r--   0 unimun     (502) staff       (20)      227 2023-05-01 21:14:38.000000 trade-republic-api-0.0.1/tests/test_trade_republic_api.py
+-rw-r--r--   0 unimun     (502) staff       (20)     1674 2023-05-01 20:32:00.000000 trade-republic-api-0.0.1/tox.ini
```

### Comparing `trade-republic-api-0.0.0/.bumpversion.cfg` & `trade-republic-api-0.0.1/.bumpversion.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [bumpversion]
-current_version = 0.0.0
+current_version = 0.0.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
-search = version='{current_version}'
-replace = version='{new_version}'
+search = version="{current_version}"
+replace = version="{new_version}"
 
 [bumpversion:file (badge):README.rst]
 search = /v{current_version}.svg
 replace = /v{new_version}.svg
 
 [bumpversion:file (link):README.rst]
 search = /v{current_version}...main
 replace = /v{new_version}...main
 
 [bumpversion:file:docs/conf.py]
-search = version = release = '{current_version}'
-replace = version = release = '{new_version}'
+search = version = release = "{current_version}"
+replace = version = release = "{new_version}"
 
 [bumpversion:file:src/trade_republic_api/__init__.py]
-search = __version__ = '{current_version}'
-replace = __version__ = '{new_version}'
+search = __version__ = "{current_version}"
+replace = __version__ = "{new_version}"
```

### Comparing `trade-republic-api-0.0.0/.cookiecutterrc` & `trade-republic-api-0.0.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/.github/workflows/github-actions.yml` & `trade-republic-api-0.0.1/.github/workflows/github-actions.yml`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,9 @@
         tox --version
         pip list --format=freeze
     - name: test
       env:
         TOXPYTHON: '${{ matrix.toxpython }}'
       run: >
         tox -e ${{ matrix.tox_env }} -v
-  finish:
-    needs: test
-    if: ${{ always() }}
-    runs-on: ubuntu-latest
-    steps:
-    - uses: coverallsapp/github-action@v2
-      with:
-        parallel-finished: true
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v3
```

### Comparing `trade-republic-api-0.0.0/.pre-commit-config.yaml` & `trade-republic-api-0.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/CONTRIBUTING.rst` & `trade-republic-api-0.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/LICENSE` & `trade-republic-api-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/PKG-INFO` & `trade-republic-api-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trade-republic-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: Trade Republic API (Unofficial)
 Home-page: https://github.com/unimun/trade-republic-api
 Author: Dongbin Han
 Author-email: unimunity@gmail.com
 License: BSD-2-Clause
 Project-URL: Documentation, https://trade-republic-api.readthedocs.io/
 Project-URL: Changelog, https://trade-republic-api.readthedocs.io/en/latest/changelog.html
```

### Comparing `trade-republic-api-0.0.0/README.rst` & `trade-republic-api-0.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/trade-republic-api
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/trade-republic-api.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/trade-republic-api
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/unimun/trade-republic-api/v0.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/unimun/trade-republic-api/v0.0.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/unimun/trade-republic-api/compare/v0.0.0...main
+    :target: https://github.com/unimun/trade-republic-api/compare/v0.0.1...main
 
 
 
 .. end-badges
 
 Trade Republic API (Unofficial)
```

### Comparing `trade-republic-api-0.0.0/ci/bootstrap.py` & `trade-republic-api-0.0.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `trade-republic-api-0.0.1/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/docs/conf.py` & `trade-republic-api-0.0.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "trade-republic-api"
 year = "2023"
 author = "Dongbin Han"
 copyright = f"{year}, {author}"
-version = release = "0.0.0"
+version = release = "0.0.1"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/unimun/trade-republic-api/issues/%s", "#"),
     "pr": ("https://github.com/unimun/trade-republic-api/pull/%s", "PR #"),
 }
```

### Comparing `trade-republic-api-0.0.0/pyproject.toml` & `trade-republic-api-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/pytest.ini` & `trade-republic-api-0.0.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/setup.py` & `trade-republic-api-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="trade-republic-api",
-    version="0.0.0",
+    version="0.0.1",
     license="BSD-2-Clause",
     description="Trade Republic API (Unofficial)",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Dongbin Han",
```

### Comparing `trade-republic-api-0.0.0/src/trade_republic_api/cli.py` & `trade-republic-api-0.0.1/src/trade_republic_api/cli.py`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/src/trade_republic_api.egg-info/PKG-INFO` & `trade-republic-api-0.0.1/src/trade_republic_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trade-republic-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: Trade Republic API (Unofficial)
 Home-page: https://github.com/unimun/trade-republic-api
 Author: Dongbin Han
 Author-email: unimunity@gmail.com
 License: BSD-2-Clause
 Project-URL: Documentation, https://trade-republic-api.readthedocs.io/
 Project-URL: Changelog, https://trade-republic-api.readthedocs.io/en/latest/changelog.html
```

### Comparing `trade-republic-api-0.0.0/src/trade_republic_api.egg-info/SOURCES.txt` & `trade-republic-api-0.0.1/src/trade_republic_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trade-republic-api-0.0.0/tox.ini` & `trade-republic-api-0.0.1/tox.ini`

 * *Files identical despite different names*

