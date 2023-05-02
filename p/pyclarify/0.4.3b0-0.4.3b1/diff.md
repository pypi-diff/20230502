# Comparing `tmp/pyclarify-0.4.3b0.tar.gz` & `tmp/pyclarify-0.4.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclarify-0.4.3b0.tar", last modified: Thu Feb 23 12:00:21 2023, max compression
+gzip compressed data, was "/home/runner/work/pyclarify/pyclarify/dist/.tmp-csq9k27j/pyclarify-0.4.3b1.tar", last modified: Tue May  2 13:19:34 2023, max compression
```

## Comparing `pyclarify-0.4.3b0.tar` & `pyclarify-0.4.3b1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.576991 pyclarify-0.4.3b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.576991 pyclarify-0.4.3b0/src/pyclarify/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.576991 pyclarify-0.4.3b0/src/pyclarify/__utils__/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/stopping_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/__utils__/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    42269 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/src/pyclarify/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/fields/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/src/pyclarify/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/jsonrpc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/jsonrpc/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/src/pyclarify/query/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/query/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/src/pyclarify/views/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/views/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/views/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/views/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/src/pyclarify/views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.576991 pyclarify-0.4.3b0/src/pyclarify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-02-23 12:00:21.000000 pyclarify-0.4.3b0/src/pyclarify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-02-23 12:00:21.000000 pyclarify-0.4.3b0/src/pyclarify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 12:00:21.000000 pyclarify-0.4.3b0/src/pyclarify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-23 12:00:21.000000 pyclarify-0.4.3b0/src/pyclarify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-23 12:00:21.000000 pyclarify-0.4.3b0/src/pyclarify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 12:00:21.580992 pyclarify-0.4.3b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_publish_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_save_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_select_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_select_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-02-23 11:59:57.000000 pyclarify-0.4.3b0/tests/test_client_select_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/stopping_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42165 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_publish_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_save_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_signals.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyclarify-0.4.3b0/LICENSE` & `pyclarify-0.4.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/LICENSE.txt` & `pyclarify-0.4.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/PKG-INFO` & `pyclarify-0.4.3b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1
-Name: pyclarify
-Version: 0.4.3b0
-Summary: Python SDK for reading and writing signals to Clarify.
-Home-page: https://github.com/clarify/pyclarify
-Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar Aspaas
-Author-email: alexia@clarify.io, eliezer@clarify.io, odd.gunnar@clarify.io
-Project-URL: Bug Tracker, https://github.com/clarify/pyclarify/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
 <a href="https://www.clarify.io">
     <img src="https://raw.githubusercontent.com/clarify/data-science-tutorials/main/media/logo_dark.png" alt="Clarify logo" title="Clarify" align="right" height="80" />
 </a>
 
 # PyClarify
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-brightgreen)](https://pypi.org/project/pyclarify/)
 [![Version number](https://img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/project/pyclarify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclarify)](https://pypi.org/project/pyclarify/)
+[![Downloads](https://static.pepy.tech/badge/pyclarify)](https://pepy.tech/project/pyclarify)
+[![Downloads](https://static.pepy.tech/personalized-badge/pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/pyclarify)
 [![Actions Status](https://github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://github.com/clarify/pyclarify/actions)
 [![License](https://img.shields.io/github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <hr/>
 
+```python
+from pyclarify import Client
+
+data = {
+  "times": ["2022-10-10T00:00:00"],
+  "temperature": [19]
+}
+
+client = Client("credentials.json")
+client.insert(data)
+```
+
 PyClarify helps users of Clarify to easily read, write and manipulate data in Clarify.
 
-- Data scientists can easily filter data, convert it to pandas with our built in methods, and write results back.
+- Data scientists can easily filter data, convert it to `pandas` with our built in methods, and write results back.
 - System integrators can set up pipelines for automatic streaming of data, and update labels on the fly.
 
 # Useful tutorials and documentation
 
 - [PyClarify SDK](https://pypi.org/project/pyclarify/)
 - [PyClarify documentation](https://clarify.github.io/pyclarify/)
 - [Clarify Developer documentation](https://docs.clarify.io/developers/welcome)
```

#### html2text {}

```diff
@@ -1,60 +1,56 @@
-Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b0 Summary: Python SDK for
-reading and writing signals to Clarify. Home-page: https://github.com/clarify/
-pyclarify Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar
-Aspaas Author-email: alexia@clarify.io, eliezer@clarify.io,
-odd.gunnar@clarify.io Project-URL: Bug Tracker, https://github.com/clarify/
-pyclarify/issues Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE License-File: LICENSE.txt [Clarify_logo] # PyClarify [!
-[PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-
-brightgreen)](https://pypi.org/project/pyclarify/) [![Version number](https://
-img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/
-project/pyclarify/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
-pyclarify)](https://pypi.org/project/pyclarify/) [![Actions Status](https://
+[Clarify_logo] # PyClarify [![PyPI package](https://img.shields.io/badge/
+pip%20install-pyclarify-brightgreen)](https://pypi.org/project/pyclarify/) [!
+[Version number](https://img.shields.io/pypi/v/
+pyclarify?color=green&label=version)](https://pypi.org/project/pyclarify/) [!
+[Downloads](https://static.pepy.tech/badge/pyclarify)](https://pepy.tech/
+project/pyclarify) [![Downloads](https://static.pepy.tech/personalized-badge/
+pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/
+month)](https://pepy.tech/project/pyclarify) [![Actions Status](https://
 github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://
 github.com/clarify/pyclarify/actions) [![License](https://img.shields.io/
 github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/
 main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/ambv/black)
 ===============================================================================
-PyClarify helps users of Clarify to easily read, write and manipulate data in
-Clarify. - Data scientists can easily filter data, convert it to pandas with
-our built in methods, and write results back. - System integrators can set up
-pipelines for automatic streaming of data, and update labels on the fly. #
-Useful tutorials and documentation - [PyClarify SDK](https://pypi.org/project/
-pyclarify/) - [PyClarify documentation](https://clarify.github.io/pyclarify/) -
-[Clarify Developer documentation](https://docs.clarify.io/developers/welcome) -
-[Basic tutorial on using Python with Clarify](https://
-colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
-tutorials/Introduction.ipynb) # Prerequisites In order to start using the
-Python SDK, you need - To know a bit of Python. For a refresher, see the
-[Official Python tutorial](https://docs.python.org/tutorial/). - Python3 (>=
-3.7) and pip. - Credentials from a Clarify integration. See the [introduction
-notebook](https://colab.research.google.com/github/clarify/data-science-
-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete introduction.
-## Where to get it The source code is currently hosted on GitHub at: https://
-github.com/clarify/pyclarify Binary installers for the latest released version
-are available at the [Python Package Index (PyPI)](https://pypi.org/project/
-pyclarify). ```sh # PyPI install pip install pyclarify ``` ## Dependencies -
-[requests](https://requests.readthedocs.io/en/latest/) - The most used (and
-trusted) HTTP library. - [Pydantic](https://pydantic-docs.helpmanual.io) -
-Allowing for strict typing and data validation. - [Typing Extensions](https://
-typing.readthedocs.io) - Brings the typing use of new type system features on
-older Python versions, allowing us to support python 3.7+. # Interact with
-Clarify PyClarify provides a fast and easy way to interact with Clarify. The
-`Client` class takes as an argument the path of your credentials in string
-format, which should always be the first step when starting to interact with
-PyClarify. For information about the Clarify Developer documentation click
-[here](https://docs.clarify.io/developers/welcome). ## Quickstart We recommend
-using Google Colab to quickly learn how to interact with Clarify using Python.
-We have created an interactive introduction tutorial where you will learn all
-the basics to get you started. [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+```python from pyclarify import Client data = { "times": ["2022-10-10T00:00:
+00"], "temperature": [19] } client = Client("credentials.json") client.insert
+(data) ``` PyClarify helps users of Clarify to easily read, write and
+manipulate data in Clarify. - Data scientists can easily filter data, convert
+it to `pandas` with our built in methods, and write results back. - System
+integrators can set up pipelines for automatic streaming of data, and update
+labels on the fly. # Useful tutorials and documentation - [PyClarify SDK]
+(https://pypi.org/project/pyclarify/) - [PyClarify documentation](https://
+clarify.github.io/pyclarify/) - [Clarify Developer documentation](https://
+docs.clarify.io/developers/welcome) - [Basic tutorial on using Python with
+Clarify](https://colab.research.google.com/github/clarify/data-science-
+tutorials/blob/main/tutorials/Introduction.ipynb) # Prerequisites In order to
+start using the Python SDK, you need - To know a bit of Python. For a
+refresher, see the [Official Python tutorial](https://docs.python.org/tutorial/
+). - Python3 (>= 3.7) and pip. - Credentials from a Clarify integration. See
+the [introduction notebook](https://colab.research.google.com/github/clarify/
+data-science-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete
+introduction. ## Where to get it The source code is currently hosted on GitHub
+at: https://github.com/clarify/pyclarify Binary installers for the latest
+released version are available at the [Python Package Index (PyPI)](https://
+pypi.org/project/pyclarify). ```sh # PyPI install pip install pyclarify ``` ##
+Dependencies - [requests](https://requests.readthedocs.io/en/latest/) - The
+most used (and trusted) HTTP library. - [Pydantic](https://pydantic-
+docs.helpmanual.io) - Allowing for strict typing and data validation. - [Typing
+Extensions](https://typing.readthedocs.io) - Brings the typing use of new type
+system features on older Python versions, allowing us to support python 3.7+. #
+Interact with Clarify PyClarify provides a fast and easy way to interact with
+Clarify. The `Client` class takes as an argument the path of your credentials
+in string format, which should always be the first step when starting to
+interact with PyClarify. For information about the Clarify Developer
+documentation click [here](https://docs.clarify.io/developers/welcome). ##
+Quickstart We recommend using Google Colab to quickly learn how to interact
+with Clarify using Python. We have created an interactive introduction tutorial
+where you will learn all the basics to get you started. [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
 tutorials/Introduction.ipynb) ### Access you data with the _ClarifyClient_
 ```python from pyclarify import Client client = Client("clarify-
 credentials.json") ``` ### Create new _Signals_ ```python from pyclarify import
 Signal signal = Signal( name = "Home temperature", description = "Temperature
 in the bedroom", labels = {"data-source": ["Raspberry Pi"], "location":
 ["Home"]} ) response = client.save_signals( input_ids=["INPUT_ID"], signals=
```

### Comparing `pyclarify-0.4.3b0/README.md` & `pyclarify-0.4.3b1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,54 @@
+Metadata-Version: 2.1
+Name: pyclarify
+Version: 0.4.3b1
+Summary: Python SDK for reading and writing signals to Clarify.
+Home-page: https://github.com/clarify/pyclarify
+Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar Aspaas
+Author-email: alexia@clarify.io, eliezer@clarify.io, odd.gunnar@clarify.io
+Project-URL: Bug Tracker, https://github.com/clarify/pyclarify/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE.txt
+
 <a href="https://www.clarify.io">
     <img src="https://raw.githubusercontent.com/clarify/data-science-tutorials/main/media/logo_dark.png" alt="Clarify logo" title="Clarify" align="right" height="80" />
 </a>
 
 # PyClarify
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-brightgreen)](https://pypi.org/project/pyclarify/)
 [![Version number](https://img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/project/pyclarify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclarify)](https://pypi.org/project/pyclarify/)
+[![Downloads](https://static.pepy.tech/badge/pyclarify)](https://pepy.tech/project/pyclarify)
+[![Downloads](https://static.pepy.tech/personalized-badge/pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/pyclarify)
 [![Actions Status](https://github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://github.com/clarify/pyclarify/actions)
 [![License](https://img.shields.io/github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <hr/>
 
+```python
+from pyclarify import Client
+
+data = {
+  "times": ["2022-10-10T00:00:00"],
+  "temperature": [19]
+}
+
+client = Client("credentials.json")
+client.insert(data)
+```
+
 PyClarify helps users of Clarify to easily read, write and manipulate data in Clarify.
 
-- Data scientists can easily filter data, convert it to pandas with our built in methods, and write results back.
+- Data scientists can easily filter data, convert it to `pandas` with our built in methods, and write results back.
 - System integrators can set up pipelines for automatic streaming of data, and update labels on the fly.
 
 # Useful tutorials and documentation
 
 - [PyClarify SDK](https://pypi.org/project/pyclarify/)
 - [PyClarify documentation](https://clarify.github.io/pyclarify/)
 - [Clarify Developer documentation](https://docs.clarify.io/developers/welcome)
```

#### html2text {}

```diff
@@ -1,52 +1,65 @@
-[Clarify_logo] # PyClarify [![PyPI package](https://img.shields.io/badge/
-pip%20install-pyclarify-brightgreen)](https://pypi.org/project/pyclarify/) [!
-[Version number](https://img.shields.io/pypi/v/
-pyclarify?color=green&label=version)](https://pypi.org/project/pyclarify/) [!
-[PyPI - Downloads](https://img.shields.io/pypi/dm/pyclarify)](https://pypi.org/
-project/pyclarify/) [![Actions Status](https://github.com/clarify/pyclarify/
-workflows/Build%20status/badge.svg)](https://github.com/clarify/pyclarify/
-actions) [![License](https://img.shields.io/github/license/clarify/pyclarify)]
-(https://github.com/clarify/pyclarify/blob/main/LICENSE) [![Code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/ambv/black)
+Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b1 Summary: Python SDK for
+reading and writing signals to Clarify. Home-page: https://github.com/clarify/
+pyclarify Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar
+Aspaas Author-email: alexia@clarify.io, eliezer@clarify.io,
+odd.gunnar@clarify.io Project-URL: Bug Tracker, https://github.com/clarify/
+pyclarify/issues Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE License-File: LICENSE.txt [Clarify_logo] # PyClarify [!
+[PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-
+brightgreen)](https://pypi.org/project/pyclarify/) [![Version number](https://
+img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/
+project/pyclarify/) [![Downloads](https://static.pepy.tech/badge/pyclarify)]
+(https://pepy.tech/project/pyclarify) [![Downloads](https://static.pepy.tech/
+personalized-badge/
+pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/
+month)](https://pepy.tech/project/pyclarify) [![Actions Status](https://
+github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://
+github.com/clarify/pyclarify/actions) [![License](https://img.shields.io/
+github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/
+main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-
+black-000000.svg)](https://github.com/ambv/black)
 ===============================================================================
-PyClarify helps users of Clarify to easily read, write and manipulate data in
-Clarify. - Data scientists can easily filter data, convert it to pandas with
-our built in methods, and write results back. - System integrators can set up
-pipelines for automatic streaming of data, and update labels on the fly. #
-Useful tutorials and documentation - [PyClarify SDK](https://pypi.org/project/
-pyclarify/) - [PyClarify documentation](https://clarify.github.io/pyclarify/) -
-[Clarify Developer documentation](https://docs.clarify.io/developers/welcome) -
-[Basic tutorial on using Python with Clarify](https://
-colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
-tutorials/Introduction.ipynb) # Prerequisites In order to start using the
-Python SDK, you need - To know a bit of Python. For a refresher, see the
-[Official Python tutorial](https://docs.python.org/tutorial/). - Python3 (>=
-3.7) and pip. - Credentials from a Clarify integration. See the [introduction
-notebook](https://colab.research.google.com/github/clarify/data-science-
-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete introduction.
-## Where to get it The source code is currently hosted on GitHub at: https://
-github.com/clarify/pyclarify Binary installers for the latest released version
-are available at the [Python Package Index (PyPI)](https://pypi.org/project/
-pyclarify). ```sh # PyPI install pip install pyclarify ``` ## Dependencies -
-[requests](https://requests.readthedocs.io/en/latest/) - The most used (and
-trusted) HTTP library. - [Pydantic](https://pydantic-docs.helpmanual.io) -
-Allowing for strict typing and data validation. - [Typing Extensions](https://
-typing.readthedocs.io) - Brings the typing use of new type system features on
-older Python versions, allowing us to support python 3.7+. # Interact with
-Clarify PyClarify provides a fast and easy way to interact with Clarify. The
-`Client` class takes as an argument the path of your credentials in string
-format, which should always be the first step when starting to interact with
-PyClarify. For information about the Clarify Developer documentation click
-[here](https://docs.clarify.io/developers/welcome). ## Quickstart We recommend
-using Google Colab to quickly learn how to interact with Clarify using Python.
-We have created an interactive introduction tutorial where you will learn all
-the basics to get you started. [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+```python from pyclarify import Client data = { "times": ["2022-10-10T00:00:
+00"], "temperature": [19] } client = Client("credentials.json") client.insert
+(data) ``` PyClarify helps users of Clarify to easily read, write and
+manipulate data in Clarify. - Data scientists can easily filter data, convert
+it to `pandas` with our built in methods, and write results back. - System
+integrators can set up pipelines for automatic streaming of data, and update
+labels on the fly. # Useful tutorials and documentation - [PyClarify SDK]
+(https://pypi.org/project/pyclarify/) - [PyClarify documentation](https://
+clarify.github.io/pyclarify/) - [Clarify Developer documentation](https://
+docs.clarify.io/developers/welcome) - [Basic tutorial on using Python with
+Clarify](https://colab.research.google.com/github/clarify/data-science-
+tutorials/blob/main/tutorials/Introduction.ipynb) # Prerequisites In order to
+start using the Python SDK, you need - To know a bit of Python. For a
+refresher, see the [Official Python tutorial](https://docs.python.org/tutorial/
+). - Python3 (>= 3.7) and pip. - Credentials from a Clarify integration. See
+the [introduction notebook](https://colab.research.google.com/github/clarify/
+data-science-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete
+introduction. ## Where to get it The source code is currently hosted on GitHub
+at: https://github.com/clarify/pyclarify Binary installers for the latest
+released version are available at the [Python Package Index (PyPI)](https://
+pypi.org/project/pyclarify). ```sh # PyPI install pip install pyclarify ``` ##
+Dependencies - [requests](https://requests.readthedocs.io/en/latest/) - The
+most used (and trusted) HTTP library. - [Pydantic](https://pydantic-
+docs.helpmanual.io) - Allowing for strict typing and data validation. - [Typing
+Extensions](https://typing.readthedocs.io) - Brings the typing use of new type
+system features on older Python versions, allowing us to support python 3.7+. #
+Interact with Clarify PyClarify provides a fast and easy way to interact with
+Clarify. The `Client` class takes as an argument the path of your credentials
+in string format, which should always be the first step when starting to
+interact with PyClarify. For information about the Clarify Developer
+documentation click [here](https://docs.clarify.io/developers/welcome). ##
+Quickstart We recommend using Google Colab to quickly learn how to interact
+with Clarify using Python. We have created an interactive introduction tutorial
+where you will learn all the basics to get you started. [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
 tutorials/Introduction.ipynb) ### Access you data with the _ClarifyClient_
 ```python from pyclarify import Client client = Client("clarify-
 credentials.json") ``` ### Create new _Signals_ ```python from pyclarify import
 Signal signal = Signal( name = "Home temperature", description = "Temperature
 in the bedroom", labels = {"data-source": ["Raspberry Pi"], "location":
 ["Home"]} ) response = client.save_signals( input_ids=["INPUT_ID"], signals=
```

### Comparing `pyclarify-0.4.3b0/setup.cfg` & `pyclarify-0.4.3b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__init__.py` & `pyclarify-0.4.3b1/src/pyclarify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -14,9 +14,9 @@
 limitations under the License.
 """
 
 from pyclarify.client import Client
 from pyclarify.views import Signal, SignalInfo, Item, ItemInfo, DataFrame
 import pyclarify.query
 
-__version__ = "0.4.3b0"
+__version__ = "0.4.3b1"
 __API_version__ = "1.1beta2"
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/__init__.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/auxiliary.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/auxiliary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,8 +18,8 @@
 from .exceptions import ImportError
 
 
 def local_import(module: str):
     try:
         return importlib.import_module(module)
     except ImportError as e:
-        raise ImportError(module.split(".")[0]) from e
+        raise ImportError(modulue=module.split(".")[0]) from e
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/exceptions.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/pagination.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/payload.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/time.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/__utils__/warnings.py` & `pyclarify-0.4.3b1/src/pyclarify/__utils__/warnings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/client.py` & `pyclarify-0.4.3b1/src/pyclarify/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -53,20 +53,19 @@
         >>> client = Client("./clarify-credentials.json")
     """
 
     def __init__(self, clarify_credentials):
         super().__init__(None)
         self.update_headers({"X-API-Version": pyclarify.__API_version__})
         self.update_headers({"User-Agent": f"PyClarify/{pyclarify.__version__}"})
-        auth_success = self.authenticate(clarify_credentials)
-        if auth_success:
-            self.base_url = f"{self.authentication.api_url}rpc"
-            logging.debug("Successfully connected to Clarify!")
-            logging.debug(f"SDK version: {pyclarify.__version__}")
-            logging.debug(f"API version: {pyclarify.__API_version__}")
+        self.authenticate(clarify_credentials)
+        self.base_url = f"{self.authentication.api_url}rpc"
+        logging.debug("Successfully connected to Clarify!")
+        logging.debug(f"SDK version: {pyclarify.__version__}")
+        logging.debug(f"API version: {pyclarify.__API_version__}")
     
     def iterate_requests(self, request: Request, stopping_condition: Callable, window_size: timedelta = None):
         iterator = SelectIterator(request, window_size)
         responses = None
         for request in iterator:
             response = self.make_request(request.json())
             if responses is None:
@@ -173,15 +172,15 @@
             {"Authorization": f"Bearer {self.authentication.get_token()}"}
         )
         return self.make_request(request_data.json())
 
     @validate_arguments
     def select_items(
         self,
-        filter: Optional[Filter] = None,
+        filter = {},
         include: Optional[List] = [],
         skip: int = 0,
         limit: Optional[int] = 10,
         sort: List[str] = [],
         total: Optional[bool] = False,
     ) -> Response:
         """
@@ -312,15 +311,15 @@
                 ...         code = '-32602',
                 ...         message = 'Invalid params',
                 ...         data = ErrorData(trace = <trace_id>, params = {})
                 ... )
 
         """
         query = ResourceQuery(
-            filter=filter.to_query() if isinstance(filter, Filter) else {},
+            filter=filter.to_query() if isinstance(filter, Filter) else filter,
             sort=sort,
             limit=limit,
             skip=skip,
             total=total,
         )
         params = {"query": query, "include": include}
 
@@ -567,15 +566,15 @@
             {"Authorization": f"Bearer {self.authentication.get_token()}"}
         )
         return self.make_request(request_data.json())
 
     @validate_arguments
     def select_signals(
         self,
-        filter: Optional[Filter] = None,
+        filter = {},
         skip: int = 0,
         limit: Optional[int] = 20,
         sort: List[str] = [],
         total: Optional[bool] = False,
         include: Optional[List] = [],
         integration: str = None,
     ) -> Response:
@@ -740,15 +739,15 @@
                 ...         code = '-32602',
                 ...         message = 'Invalid params',
                 ...         data = ErrorData(trace = <trace_id>, params = {})
                 ... )
 
         """
         query = ResourceQuery(
-            filter=filter.to_query() if isinstance(filter, Filter) else {},
+            filter=filter.to_query() if isinstance(filter, Filter) else filter,
             sort=sort,
             limit=limit,
             skip=skip,
             total=total,
         )
         params = {"integration": integration, "query": query, "include": include}
 
@@ -762,15 +761,15 @@
             {"Authorization": f"Bearer {self.authentication.get_token()}"}
         )
         return self.iterate_requests(request_data, select_stopping_condition)
 
     @validate_arguments
     def data_frame(
         self,
-        filter: Optional[Filter] = None,
+        filter = {},
         sort: List[str] = [],
         limit: int = 20,
         skip: int = 0,
         total: bool = False,
         gte: Union[datetime, str] = None,
         lt: Union[datetime, str] = None,
         last: int = -1,
@@ -954,15 +953,15 @@
             ... 2022-09-05 11:32:11.432722+00:00                   6.0                   4.0  ...                   8.0                   9.0
             ... 2022-09-05 11:33:11.432720+00:00                   0.0                   7.0  ...                   9.0                   4.0
             ... 2022-09-05 11:34:11.432719+00:00                   8.0                   6.0  ...                   8.0                   5.0
 
         """
 
         query = ResourceQuery(
-            filter=filter.to_query() if isinstance(filter, Filter) else {},
+            filter=filter.to_query() if isinstance(filter, Filter) else filter,
             sort=sort,
             limit=limit,
             skip=skip,
             total=total,
         )
         data_filter = DataFilter(gte=gte, lt=lt)
         data_query = DataQuery(filter=data_filter.to_query(), last=last, rollup=rollup)
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/authentication.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/constraints.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/dataframe.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/error.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/query.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/fields/resource.py` & `pyclarify-0.4.3b1/src/pyclarify/fields/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/jsonrpc/client.py` & `pyclarify-0.4.3b1/src/pyclarify/jsonrpc/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -74,22 +74,18 @@
         ----------
         clarify_credentials : str/dict
             The path to the clarify_credentials.json downloaded from the Clarify app,
             or json/dictionary of the content in clarify_credentials.json.
 
         Returns
         -------
-        bool
-            True if valid credentials is passed otherwise False.
+        None
         """
-        try:
-            self.authentication = Authenticator(clarify_credentials)
-            return True
-        except AuthError:
-            return False
+        self.authentication = Authenticator(clarify_credentials)
+        
 
     def make_request(self, payload) -> Response:
         """
         Uses post request to send JSON RPC payload.
 
         Parameters
         ----------
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/jsonrpc/oauth2.py` & `pyclarify-0.4.3b1/src/pyclarify/jsonrpc/oauth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/query/__init__.py` & `pyclarify-0.4.3b1/src/pyclarify/query/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/query/filter.py` & `pyclarify-0.4.3b1/src/pyclarify/query/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/query/query.py` & `pyclarify-0.4.3b1/src/pyclarify/query/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/views/__init__.py` & `pyclarify-0.4.3b1/src/pyclarify/views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/views/dataframe.py` & `pyclarify-0.4.3b1/src/pyclarify/views/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -180,14 +180,15 @@
             if df.name is not None:
                 series =  {df.name : list(df.values)}
             else:
                 raise ValueError("The series you are converting does not have a name.")
 
         if time_col:
             times = df[time_col].values
+            series.pop(time_col)
         else:
             if is_datetime(df.index.values[0]):
                 times = df.index.values
             else:
                 import warnings
                 warnings.warn("No obvious time index! Attempting to select based on data.", stacklevel=2)
                 possible_indexes = [is_datetime(c) for c in df.values[0]]
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/views/generics.py` & `pyclarify-0.4.3b1/src/pyclarify/views/generics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/views/items.py` & `pyclarify-0.4.3b1/src/pyclarify/views/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify/views/signals.py` & `pyclarify-0.4.3b1/src/pyclarify/views/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2022 Searis AS
+Copyright 2023 Searis AS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify.egg-info/PKG-INFO` & `pyclarify-0.4.3b1/src/pyclarify.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclarify
-Version: 0.4.3b0
+Version: 0.4.3b1
 Summary: Python SDK for reading and writing signals to Clarify.
 Home-page: https://github.com/clarify/pyclarify
 Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar Aspaas
 Author-email: alexia@clarify.io, eliezer@clarify.io, odd.gunnar@clarify.io
 Project-URL: Bug Tracker, https://github.com/clarify/pyclarify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,24 +18,37 @@
     <img src="https://raw.githubusercontent.com/clarify/data-science-tutorials/main/media/logo_dark.png" alt="Clarify logo" title="Clarify" align="right" height="80" />
 </a>
 
 # PyClarify
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-brightgreen)](https://pypi.org/project/pyclarify/)
 [![Version number](https://img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/project/pyclarify/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclarify)](https://pypi.org/project/pyclarify/)
+[![Downloads](https://static.pepy.tech/badge/pyclarify)](https://pepy.tech/project/pyclarify)
+[![Downloads](https://static.pepy.tech/personalized-badge/pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/month)](https://pepy.tech/project/pyclarify)
 [![Actions Status](https://github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://github.com/clarify/pyclarify/actions)
 [![License](https://img.shields.io/github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 <hr/>
 
+```python
+from pyclarify import Client
+
+data = {
+  "times": ["2022-10-10T00:00:00"],
+  "temperature": [19]
+}
+
+client = Client("credentials.json")
+client.insert(data)
+```
+
 PyClarify helps users of Clarify to easily read, write and manipulate data in Clarify.
 
-- Data scientists can easily filter data, convert it to pandas with our built in methods, and write results back.
+- Data scientists can easily filter data, convert it to `pandas` with our built in methods, and write results back.
 - System integrators can set up pipelines for automatic streaming of data, and update labels on the fly.
 
 # Useful tutorials and documentation
 
 - [PyClarify SDK](https://pypi.org/project/pyclarify/)
 - [PyClarify documentation](https://clarify.github.io/pyclarify/)
 - [Clarify Developer documentation](https://docs.clarify.io/developers/welcome)
```

#### html2text {}

```diff
@@ -1,60 +1,65 @@
-Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b1 Summary: Python SDK for
 reading and writing signals to Clarify. Home-page: https://github.com/clarify/
 pyclarify Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar
 Aspaas Author-email: alexia@clarify.io, eliezer@clarify.io,
 odd.gunnar@clarify.io Project-URL: Bug Tracker, https://github.com/clarify/
 pyclarify/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE License-File: LICENSE.txt [Clarify_logo] # PyClarify [!
 [PyPI package](https://img.shields.io/badge/pip%20install-pyclarify-
 brightgreen)](https://pypi.org/project/pyclarify/) [![Version number](https://
 img.shields.io/pypi/v/pyclarify?color=green&label=version)](https://pypi.org/
-project/pyclarify/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
-pyclarify)](https://pypi.org/project/pyclarify/) [![Actions Status](https://
+project/pyclarify/) [![Downloads](https://static.pepy.tech/badge/pyclarify)]
+(https://pepy.tech/project/pyclarify) [![Downloads](https://static.pepy.tech/
+personalized-badge/
+pyclarify?period=month&units=none&left_color=grey&right_color=blue&left_text=downloads/
+month)](https://pepy.tech/project/pyclarify) [![Actions Status](https://
 github.com/clarify/pyclarify/workflows/Build%20status/badge.svg)](https://
 github.com/clarify/pyclarify/actions) [![License](https://img.shields.io/
 github/license/clarify/pyclarify)](https://github.com/clarify/pyclarify/blob/
 main/LICENSE) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/ambv/black)
 ===============================================================================
-PyClarify helps users of Clarify to easily read, write and manipulate data in
-Clarify. - Data scientists can easily filter data, convert it to pandas with
-our built in methods, and write results back. - System integrators can set up
-pipelines for automatic streaming of data, and update labels on the fly. #
-Useful tutorials and documentation - [PyClarify SDK](https://pypi.org/project/
-pyclarify/) - [PyClarify documentation](https://clarify.github.io/pyclarify/) -
-[Clarify Developer documentation](https://docs.clarify.io/developers/welcome) -
-[Basic tutorial on using Python with Clarify](https://
-colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
-tutorials/Introduction.ipynb) # Prerequisites In order to start using the
-Python SDK, you need - To know a bit of Python. For a refresher, see the
-[Official Python tutorial](https://docs.python.org/tutorial/). - Python3 (>=
-3.7) and pip. - Credentials from a Clarify integration. See the [introduction
-notebook](https://colab.research.google.com/github/clarify/data-science-
-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete introduction.
-## Where to get it The source code is currently hosted on GitHub at: https://
-github.com/clarify/pyclarify Binary installers for the latest released version
-are available at the [Python Package Index (PyPI)](https://pypi.org/project/
-pyclarify). ```sh # PyPI install pip install pyclarify ``` ## Dependencies -
-[requests](https://requests.readthedocs.io/en/latest/) - The most used (and
-trusted) HTTP library. - [Pydantic](https://pydantic-docs.helpmanual.io) -
-Allowing for strict typing and data validation. - [Typing Extensions](https://
-typing.readthedocs.io) - Brings the typing use of new type system features on
-older Python versions, allowing us to support python 3.7+. # Interact with
-Clarify PyClarify provides a fast and easy way to interact with Clarify. The
-`Client` class takes as an argument the path of your credentials in string
-format, which should always be the first step when starting to interact with
-PyClarify. For information about the Clarify Developer documentation click
-[here](https://docs.clarify.io/developers/welcome). ## Quickstart We recommend
-using Google Colab to quickly learn how to interact with Clarify using Python.
-We have created an interactive introduction tutorial where you will learn all
-the basics to get you started. [![Open In Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+```python from pyclarify import Client data = { "times": ["2022-10-10T00:00:
+00"], "temperature": [19] } client = Client("credentials.json") client.insert
+(data) ``` PyClarify helps users of Clarify to easily read, write and
+manipulate data in Clarify. - Data scientists can easily filter data, convert
+it to `pandas` with our built in methods, and write results back. - System
+integrators can set up pipelines for automatic streaming of data, and update
+labels on the fly. # Useful tutorials and documentation - [PyClarify SDK]
+(https://pypi.org/project/pyclarify/) - [PyClarify documentation](https://
+clarify.github.io/pyclarify/) - [Clarify Developer documentation](https://
+docs.clarify.io/developers/welcome) - [Basic tutorial on using Python with
+Clarify](https://colab.research.google.com/github/clarify/data-science-
+tutorials/blob/main/tutorials/Introduction.ipynb) # Prerequisites In order to
+start using the Python SDK, you need - To know a bit of Python. For a
+refresher, see the [Official Python tutorial](https://docs.python.org/tutorial/
+). - Python3 (>= 3.7) and pip. - Credentials from a Clarify integration. See
+the [introduction notebook](https://colab.research.google.com/github/clarify/
+data-science-tutorials/blob/main/tutorials/Introduction.ipynb) for a complete
+introduction. ## Where to get it The source code is currently hosted on GitHub
+at: https://github.com/clarify/pyclarify Binary installers for the latest
+released version are available at the [Python Package Index (PyPI)](https://
+pypi.org/project/pyclarify). ```sh # PyPI install pip install pyclarify ``` ##
+Dependencies - [requests](https://requests.readthedocs.io/en/latest/) - The
+most used (and trusted) HTTP library. - [Pydantic](https://pydantic-
+docs.helpmanual.io) - Allowing for strict typing and data validation. - [Typing
+Extensions](https://typing.readthedocs.io) - Brings the typing use of new type
+system features on older Python versions, allowing us to support python 3.7+. #
+Interact with Clarify PyClarify provides a fast and easy way to interact with
+Clarify. The `Client` class takes as an argument the path of your credentials
+in string format, which should always be the first step when starting to
+interact with PyClarify. For information about the Clarify Developer
+documentation click [here](https://docs.clarify.io/developers/welcome). ##
+Quickstart We recommend using Google Colab to quickly learn how to interact
+with Clarify using Python. We have created an interactive introduction tutorial
+where you will learn all the basics to get you started. [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/clarify/data-science-tutorials/blob/main/
 tutorials/Introduction.ipynb) ### Access you data with the _ClarifyClient_
 ```python from pyclarify import Client client = Client("clarify-
 credentials.json") ``` ### Create new _Signals_ ```python from pyclarify import
 Signal signal = Signal( name = "Home temperature", description = "Temperature
 in the bedroom", labels = {"data-source": ["Raspberry Pi"], "location":
 ["Home"]} ) response = client.save_signals( input_ids=["INPUT_ID"], signals=
```

### Comparing `pyclarify-0.4.3b0/src/pyclarify.egg-info/SOURCES.txt` & `pyclarify-0.4.3b1/src/pyclarify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_insert.py` & `pyclarify-0.4.3b1/tests/test_client_insert.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_publish_signals.py` & `pyclarify-0.4.3b1/tests/test_client_publish_signals.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_save_signals.py` & `pyclarify-0.4.3b1/tests/test_client_save_signals.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_select_dataframe.py` & `pyclarify-0.4.3b1/tests/test_client_select_dataframe.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_select_items.py` & `pyclarify-0.4.3b1/tests/test_client_select_items.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b0/tests/test_client_select_signals.py` & `pyclarify-0.4.3b1/tests/test_client_select_signals.py`

 * *Files identical despite different names*

