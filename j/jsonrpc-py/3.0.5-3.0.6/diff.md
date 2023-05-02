# Comparing `tmp/jsonrpc-py-3.0.5.tar.gz` & `tmp/jsonrpc-py-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.5.tar", last modified: Wed Apr 26 12:25:48 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.6.tar", last modified: Tue May  2 09:55:03 2023, max compression
```

## Comparing `jsonrpc-py-3.0.5.tar` & `jsonrpc-py-3.0.6.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.470396 jsonrpc-py-3.0.5/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.flake8
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/Makefile
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-26 12:25:48.469396 jsonrpc-py-3.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.449395 jsonrpc-py-3.0.5/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.442394 jsonrpc-py-3.0.5/docs/changelog/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.451395 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.1.0.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.459395 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.1.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.2.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.3.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.7.rst
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.8.rst
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.4.9.rst
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.5.1.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.461395 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.2.rst
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.5.rst
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/deployment.rst
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1861 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/docs/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.465396 jsonrpc-py-3.0.5/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5994 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.466396 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2852 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1922 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 12:25:48.000000 jsonrpc-py-3.0.5/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:25:48.470396 jsonrpc-py-3.0.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:25:48.469396 jsonrpc-py-3.0.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13819 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-26 12:25:26.000000 jsonrpc-py-3.0.5/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.775499 jsonrpc-py-3.0.6/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.769499 jsonrpc-py-3.0.6/docs/changelog/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.778499 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.1.0.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.785500 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      421 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.1.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      397 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.2.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.3.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.8.rst
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.4.9.rst
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.5.1.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.788500 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2623 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/deployment.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1861 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/docs/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.791500 jsonrpc-py-3.0.6/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9423 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5994 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3240 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.793501 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 09:55:03.000000 jsonrpc-py-3.0.6/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 09:55:03.797501 jsonrpc-py-3.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:55:03.796501 jsonrpc-py-3.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13819 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5140 2023-05-02 09:54:40.000000 jsonrpc-py-3.0.6/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.5/.gitlab-ci.yml` & `jsonrpc-py-3.0.6/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ---
 image: python:3.11-bullseye
 
 variables:
   PIP_CACHE_DIR: "$CI_PROJECT_DIR/.pip_cache"
-  PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_PROGRESS_BAR: "off"
   PIP_TIMEOUT: "300"
   PYTHONDONTWRITEBYTECODE: "1"
 
 cache:
   paths:
     - .pip_cache
@@ -16,15 +15,15 @@
 stages:
   - testing
   - building
   - publishing
 
 before_script:
   - python -VV
-  - python -m venv --copies .venv
+  - python -m venv --copies --upgrade-deps .venv
   - source .venv/bin/activate
 
 code quality:
   stage: testing
   script:
     - time make install
     - time make linting
```

### Comparing `jsonrpc-py-3.0.5/LICENSE` & `jsonrpc-py-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/Makefile` & `jsonrpc-py-3.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/PKG-INFO` & `jsonrpc-py-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.5
+Version: 3.0.6
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.5/README.md` & `jsonrpc-py-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/changelog/v1.x.x/v1.1.0.rst` & `jsonrpc-py-3.0.6/docs/changelog/v1.x.x/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.0.1.rst` & `jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.0.1.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/changelog/v2.x.x/v2.3.0.rst` & `jsonrpc-py-3.0.6/docs/changelog/v2.x.x/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/changelog/v3.x.x/v3.0.0.rst` & `jsonrpc-py-3.0.6/docs/changelog/v3.x.x/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/changelog.rst` & `jsonrpc-py-3.0.6/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/conf.py` & `jsonrpc-py-3.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/deployment.rst` & `jsonrpc-py-3.0.6/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/index.rst` & `jsonrpc-py-3.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/quickstart.rst` & `jsonrpc-py-3.0.6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/docs/reference.rst` & `jsonrpc-py-3.0.6/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/__init__.py` & `jsonrpc-py-3.0.6/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/asgi.py` & `jsonrpc-py-3.0.6/jsonrpc/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import re
-from asyncio import CancelledError, Task, create_task, gather, wait_for
+from asyncio import CancelledError, Task, create_task, shield
 from collections import UserDict
 from collections.abc import Generator, MutableSequence
 from http import HTTPMethod, HTTPStatus
 from io import DEFAULT_BUFFER_SIZE, BytesIO
 from typing import Any, ClassVar, Final, TypeAlias
 
 from .dispatcher import AsyncDispatcher
 from .errors import Error
 from .request import BatchRequest, Request
 from .response import BatchResponse, Response
 from .serializer import JSONSerializer
 from .typedefs import ASGIReceiveCallable, ASGISendCallable, HTTPConnectionScope, Scope
+from .utilities import multiple_coroutines
 
 __all__: Final[tuple[str, ...]] = ("ASGIHandler",)
 
 AnyTask: TypeAlias = Task[Any]
 AnyRequest: TypeAlias = Request | Error | BatchRequest
 AnyResponse: TypeAlias = Response | BatchResponse | None
 
@@ -190,22 +191,21 @@
             task.add_done_callback(self.background_tasks.discard)
             if request.is_notification:
                 #: ---
                 #: Mark exception retrieved:
                 task.add_done_callback(lambda task: task.cancelled() or task.exception() is None)
                 return None
             try:
-                result: Any = await wait_for(task, 3600.0)  # 1 hour.
+                result: Any = await shield(task)
                 return Response(body=result, response_id=request.request_id)
             except Error as error:
                 return Response(error=error, response_id=request.request_id)
 
         async def on_batch_request(request: BatchRequest) -> BatchResponse:
-            tasks: frozenset[AnyTask] = frozenset({create_task(self.process_request(item)) for item in request})
-            responses: list[AnyResponse] = await gather(*tasks)
+            responses: list[AnyResponse] = await multiple_coroutines(map(self.process_request, request))
             return BatchResponse([response for response in responses if isinstance(response, Response)])
 
         if isinstance(obj, Error):
             return on_error(obj)
         elif isinstance(obj, Request):
             return await on_request(obj)
         else:
```

### Comparing `jsonrpc-py-3.0.5/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.6/jsonrpc/dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/errors.py` & `jsonrpc-py-3.0.6/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/request.py` & `jsonrpc-py-3.0.6/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/response.py` & `jsonrpc-py-3.0.6/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/serializer.py` & `jsonrpc-py-3.0.6/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.6/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.6/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.5
+Version: 3.0.6
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Author-email: Andrew Malchuk <andrew.malchuk@yandex.ru>
 Maintainer-email: JSON-RPC Development Group <dev@jsonrpc.ru>
 License: BSD-3-Clause
 Project-URL: Source Code, https://gitlab.com/jsonrpc/jsonrpc-py
 Project-URL: Documentation, https://docs.jsonrpc.ru
 Project-URL: Change Log, https://docs.jsonrpc.ru/changelog.html
```

### Comparing `jsonrpc-py-3.0.5/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.6/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 docs/changelog/v3.x.x/index.rst
 docs/changelog/v3.x.x/v3.0.0.rst
 docs/changelog/v3.x.x/v3.0.1.rst
 docs/changelog/v3.x.x/v3.0.2.rst
 docs/changelog/v3.x.x/v3.0.3.rst
 docs/changelog/v3.x.x/v3.0.4.rst
 docs/changelog/v3.x.x/v3.0.5.rst
+docs/changelog/v3.x.x/v3.0.6.rst
 jsonrpc/__init__.py
 jsonrpc/asgi.py
 jsonrpc/dispatcher.py
 jsonrpc/errors.py
 jsonrpc/py.typed
 jsonrpc/request.py
 jsonrpc/response.py
```

### Comparing `jsonrpc-py-3.0.5/pyproject.toml` & `jsonrpc-py-3.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_asgi.py` & `jsonrpc-py-3.0.6/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_dispatcher.py` & `jsonrpc-py-3.0.6/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_errors.py` & `jsonrpc-py-3.0.6/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_request.py` & `jsonrpc-py-3.0.6/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_response.py` & `jsonrpc-py-3.0.6/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.5/tests/test_serializer.py` & `jsonrpc-py-3.0.6/tests/test_serializer.py`

 * *Files identical despite different names*

