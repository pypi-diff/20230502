# Comparing `tmp/hkpy-2.8.1.tar.gz` & `tmp/hkpy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkpy-2.8.1.tar", last modified: Thu Apr 13 19:22:34 2023, max compression
+gzip compressed data, was "hkpy-2.9.0.tar", last modified: Tue May  2 13:57:38 2023, max compression
```

## Comparing `hkpy-2.8.1.tar` & `hkpy-2.9.0.tar`

### file list

```diff
@@ -1,92 +1,98 @@
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:34.051376 hkpy-2.8.1/
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.758390 hkpy-2.8.1/.venv/
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.766920 hkpy-2.8.1/.venv/lib/
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.775477 hkpy-2.8.1/.venv/lib/python3.10/
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:28.824112 hkpy-2.8.1/.venv/lib/python3.10/site-packages/
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.532160 hkpy-2.8.1/.venv/lib/python3.10/site-packages/hkpy/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 18:41:08.000000 hkpy-2.8.1/.venv/lib/python3.10/site-packages/hkpy/py.typed
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.636512 hkpy-2.8.1/.venv/lib/python3.10/site-packages/pip/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      286 2023-04-13 18:34:18.000000 hkpy-2.8.1/.venv/lib/python3.10/site-packages/pip/py.typed
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1088 2023-04-13 14:26:29.000000 hkpy-2.8.1/LICENSE
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       45 2023-04-13 19:17:08.000000 hkpy-2.8.1/MANIFEST.in
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-04-13 19:22:34.044856 hkpy-2.8.1/PKG-INFO
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2538 2023-04-13 14:26:29.000000 hkpy-2.8.1/README.md
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:29.745329 hkpy-2.8.1/hkpy/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      218 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/__init__.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.137560 hkpy-2.8.1/hkpy/common/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      109 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/common/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2163 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/common/result_set.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.663862 hkpy-2.8.1/hkpy/hkbase/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      309 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6600 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkbase.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6160 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkobserverfactory.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    23414 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hkrepository.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1169 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/hktransaction.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.818390 hkpy-2.8.1/hkpy/hkbase/observer/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      162 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/__init__.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:31.281090 hkpy-2.8.1/hkpy/hkbase/observer/clients/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      331 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     5210 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/configurableobserverclient.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1691 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/observerclient.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6873 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     7990 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/clients/restobserverclient.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      599 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/observer/notification.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1859 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/query.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1600 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hkbase/query_management.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:31.891013 hkpy-2.8.1/hkpy/hklib/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2726 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1790 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/anchor.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2123 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/connector.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3321 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/entity.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.334190 hkpy-2.8.1/hkpy/hklib/fi/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      250 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2410 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/fi.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1875 2023-04-13 15:31:05.000000 hkpy-2.8.1/hkpy/hklib/fi/fianchor.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      193 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/fioperator.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4098 2023-04-13 15:31:05.000000 hkpy-2.8.1/hkpy/hklib/fi/fiparser.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1477 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/fi/grammar.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6927 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/graph.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3516 2023-04-13 14:26:29.000000 hkpy-2.8.1/hkpy/hklib/graphbuilder.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3738 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hklib/link.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     9768 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hklib/node.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.408228 hkpy-2.8.1/hkpy/hkpyo/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      177 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/__init__.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:32.818380 hkpy-2.8.1/hkpy/hkpyo/converters/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16080 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/HKOReaderHKG.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    19047 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/HKOWriterHKG.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      197 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      493 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/constants.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1533 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/converters/utils.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.067527 hkpy-2.8.1/hkpy/hkpyo/hkb/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      158 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2694 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2290 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo_simple.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.223279 hkpy-2.8.1/hkpy/hkpyo/model/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      135 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/model/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16316 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/model/hko_model.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.382840 hkpy-2.8.1/hkpy/hkpyo/reasoners/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      141 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/reasoners/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4855 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/hkpyo/reasoners/simple_reasoner.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.518031 hkpy-2.8.1/hkpy/oops/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      185 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/oops/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      775 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/oops/oops.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/py.typed
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.726486 hkpy-2.8.1/hkpy/utils/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      155 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/__init__.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1379 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/constants.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2234 2023-04-13 14:26:30.000000 hkpy-2.8.1/hkpy/utils/misc.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:30.003978 hkpy-2.8.1/hkpy.egg-info/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/PKG-INFO
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1828 2023-04-13 19:22:28.000000 hkpy-2.8.1/hkpy.egg-info/SOURCES.txt
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        1 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/dependency_links.txt
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       71 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/requires.txt
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-04-13 19:22:07.000000 hkpy-2.8.1/hkpy.egg-info/top_level.txt
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       38 2023-04-13 19:22:34.054394 hkpy-2.8.1/setup.cfg
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1976 2023-04-13 19:18:58.000000 hkpy-2.8.1/setup.py
-drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:22:33.988545 hkpy-2.8.1/tests/
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4004 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3454 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_context.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2092 2023-04-13 15:31:05.000000 hkpy-2.8.1/tests/test_fi.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      903 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_literal.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3764 2023-04-13 14:26:30.000000 hkpy-2.8.1/tests/test_simple_reasoner.py
--rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-04-13 19:20:59.000000 hkpy-2.8.1/version.txt
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.474639 hkpy-2.9.0/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.514754 hkpy-2.9.0/.venv/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.517843 hkpy-2.9.0/.venv/lib/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.522366 hkpy-2.9.0/.venv/lib/python3.10/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.580362 hkpy-2.9.0/.venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.829798 hkpy-2.9.0/.venv/lib/python3.10/site-packages/build/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:56:44.000000 hkpy-2.9.0/.venv/lib/python3.10/site-packages/build/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.888797 hkpy-2.9.0/.venv/lib/python3.10/site-packages/hkpy/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 19:25:46.000000 hkpy-2.9.0/.venv/lib/python3.10/site-packages/hkpy/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:35.958406 hkpy-2.9.0/.venv/lib/python3.10/site-packages/packaging/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:56:42.000000 hkpy-2.9.0/.venv/lib/python3.10/site-packages/packaging/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.020415 hkpy-2.9.0/.venv/lib/python3.10/site-packages/pip/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      286 2023-04-13 18:34:18.000000 hkpy-2.9.0/.venv/lib/python3.10/site-packages/pip/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.080924 hkpy-2.9.0/.venv/lib/python3.10/site-packages/tomli/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       26 2023-05-02 13:56:42.000000 hkpy-2.9.0/.venv/lib/python3.10/site-packages/tomli/py.typed
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1088 2023-04-13 14:26:29.000000 hkpy-2.9.0/LICENSE
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       45 2023-04-13 19:35:11.000000 hkpy-2.9.0/MANIFEST.in
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-05-02 13:57:38.469639 hkpy-2.9.0/PKG-INFO
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2538 2023-04-13 14:26:29.000000 hkpy-2.9.0/README.md
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.149659 hkpy-2.9.0/hkpy/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      218 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.319386 hkpy-2.9.0/hkpy/common/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      109 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/common/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2163 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/common/result_set.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.553847 hkpy-2.9.0/hkpy/hkbase/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      309 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6600 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/hkbase.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6160 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/hkobserverfactory.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    23438 2023-05-02 13:53:51.000000 hkpy-2.9.0/hkpy/hkbase/hkrepository.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1169 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/hktransaction.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.641052 hkpy-2.9.0/hkpy/hkbase/observer/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      162 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.931482 hkpy-2.9.0/hkpy/hkbase/observer/clients/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      331 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/clients/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     5210 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/clients/configurableobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1691 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/clients/observerclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6873 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     7990 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/clients/restobserverclient.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      599 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/observer/notification.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1859 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/query.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1600 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hkbase/query_management.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:37.273835 hkpy-2.9.0/hkpy/hklib/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2726 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1790 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/anchor.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2123 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/connector.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3321 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/entity.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:37.535957 hkpy-2.9.0/hkpy/hklib/fi/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      250 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/fi/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2410 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/fi/fi.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1875 2023-04-13 15:31:05.000000 hkpy-2.9.0/hkpy/hklib/fi/fianchor.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      193 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/fi/fioperator.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4098 2023-04-13 15:31:05.000000 hkpy-2.9.0/hkpy/hklib/fi/fiparser.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1477 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/fi/grammar.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     6927 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/graph.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3516 2023-04-13 14:26:29.000000 hkpy-2.9.0/hkpy/hklib/graphbuilder.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3738 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hklib/link.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     9768 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hklib/node.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:37.572484 hkpy-2.9.0/hkpy/hkpyo/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      177 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/__init__.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:37.782048 hkpy-2.9.0/hkpy/hkpyo/converters/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16080 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/converters/HKOReaderHKG.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    19047 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/converters/HKOWriterHKG.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      197 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/converters/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      493 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/converters/constants.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1533 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/converters/utils.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:37.920354 hkpy-2.9.0/hkpy/hkpyo/hkb/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      158 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/hkb/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2694 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/hkb/hkbo.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2290 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/hkb/hkbo_simple.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.013882 hkpy-2.9.0/hkpy/hkpyo/model/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      135 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/model/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)    16316 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/model/hko_model.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.112388 hkpy-2.9.0/hkpy/hkpyo/reasoners/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      141 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/reasoners/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4855 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/hkpyo/reasoners/simple_reasoner.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.190477 hkpy-2.9.0/hkpy/oops/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      185 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/oops/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      775 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/oops/oops.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        0 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/py.typed
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.301696 hkpy-2.9.0/hkpy/utils/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      155 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/utils/__init__.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1379 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/utils/constants.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2234 2023-04-13 14:26:30.000000 hkpy-2.9.0/hkpy/utils/misc.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:36.264760 hkpy-2.9.0/hkpy.egg-info/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      832 2023-05-02 13:57:23.000000 hkpy-2.9.0/hkpy.egg-info/PKG-INFO
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1982 2023-05-02 13:57:35.000000 hkpy-2.9.0/hkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        1 2023-05-02 13:57:23.000000 hkpy-2.9.0/hkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       71 2023-05-02 13:57:23.000000 hkpy-2.9.0/hkpy.egg-info/requires.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-05-02 13:57:23.000000 hkpy-2.9.0/hkpy.egg-info/top_level.txt
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)       38 2023-05-02 13:57:38.475639 hkpy-2.9.0/setup.cfg
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     1976 2023-04-13 19:35:12.000000 hkpy-2.9.0/setup.py
+drwxr-xr-x   0 srfiorini  (1000) srfiorini  (1000)        0 2023-05-02 13:57:38.441639 hkpy-2.9.0/tests/
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     4004 2023-04-13 14:26:30.000000 hkpy-2.9.0/tests/test.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3454 2023-04-13 14:26:30.000000 hkpy-2.9.0/tests/test_context.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     2092 2023-04-13 15:31:05.000000 hkpy-2.9.0/tests/test_fi.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)      903 2023-04-13 14:26:30.000000 hkpy-2.9.0/tests/test_literal.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)     3764 2023-04-13 14:26:30.000000 hkpy-2.9.0/tests/test_simple_reasoner.py
+-rw-r--r--   0 srfiorini  (1000) srfiorini  (1000)        5 2023-05-02 13:53:51.000000 hkpy-2.9.0/version.txt
```

### Comparing `hkpy-2.8.1/LICENSE` & `hkpy-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/PKG-INFO` & `hkpy-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkpy
-Version: 2.8.1
+Version: 2.9.0
 Summary: A Python module to create software abstraction for accessing hyperknowledge graphs
 Home-page: https://github.com/ibm-hyperknowledge/hkpy
 Author: IBM Research Brazil
 Author-email: mmoreno@br.ibm.com
 License: MIT
 Keywords: Hyperknowlede,Knowledge Engineering
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hkpy-2.8.1/README.md` & `hkpy-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/common/result_set.py` & `hkpy-2.9.0/hkpy/common/result_set.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/hkbase.py` & `hkpy-2.9.0/hkpy/hkbase/hkbase.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/hkobserverfactory.py` & `hkpy-2.9.0/hkpy/hkbase/hkobserverfactory.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/hkrepository.py` & `hkpy-2.9.0/hkpy/hkbase/hkrepository.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
             headers['transactionId'] = transaction_id
 
         response = requests.post(url=url, headers=headers, json=stored_query)
         _, data = response_validator(response=response)
 
         return HKStoredQuery.from_dict(data)
 
-    def run_stored_query(self, query_id: str, parameters: Optional[List[str]] = None,
+    def run_stored_query(self, query_id: str, parameters: Optional[Dict[str, Union[str, float, int]]] = None,
                          run_options: Optional[Dict] = None, transaction_id: Optional[str] = None,
                          mime_type: Optional[str] = None, proxy: Optional[bool] = False) -> Union[HKEntityResultSet,
                                                                                                   SPARQLResultSet]:
         run_configuration = dict()
         if parameters is not None:
             run_configuration['parameters'] = parameters
         if run_options is not None:
```

### Comparing `hkpy-2.8.1/hkpy/hkbase/hktransaction.py` & `hkpy-2.9.0/hkpy/hkbase/hktransaction.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/observer/clients/configurableobserverclient.py` & `hkpy-2.9.0/hkpy/hkbase/observer/clients/configurableobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/observer/clients/observerclient.py` & `hkpy-2.9.0/hkpy/hkbase/observer/clients/observerclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py` & `hkpy-2.9.0/hkpy/hkbase/observer/clients/rabbitmqobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/observer/clients/restobserverclient.py` & `hkpy-2.9.0/hkpy/hkbase/observer/clients/restobserverclient.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/observer/notification.py` & `hkpy-2.9.0/hkpy/hkbase/observer/notification.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/query.py` & `hkpy-2.9.0/hkpy/hkbase/query.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkbase/query_management.py` & `hkpy-2.9.0/hkpy/hkbase/query_management.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/__init__.py` & `hkpy-2.9.0/hkpy/hklib/__init__.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/anchor.py` & `hkpy-2.9.0/hkpy/hklib/anchor.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/connector.py` & `hkpy-2.9.0/hkpy/hklib/connector.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/entity.py` & `hkpy-2.9.0/hkpy/hklib/entity.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/fi/fi.py` & `hkpy-2.9.0/hkpy/hklib/fi/fi.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/fi/fianchor.py` & `hkpy-2.9.0/hkpy/hklib/fi/fianchor.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/fi/fiparser.py` & `hkpy-2.9.0/hkpy/hklib/fi/fiparser.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/fi/grammar.py` & `hkpy-2.9.0/hkpy/hklib/fi/grammar.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/graph.py` & `hkpy-2.9.0/hkpy/hklib/graph.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/graphbuilder.py` & `hkpy-2.9.0/hkpy/hklib/graphbuilder.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/link.py` & `hkpy-2.9.0/hkpy/hklib/link.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hklib/node.py` & `hkpy-2.9.0/hkpy/hklib/node.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/converters/HKOReaderHKG.py` & `hkpy-2.9.0/hkpy/hkpyo/converters/HKOReaderHKG.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/converters/HKOWriterHKG.py` & `hkpy-2.9.0/hkpy/hkpyo/converters/HKOWriterHKG.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/converters/utils.py` & `hkpy-2.9.0/hkpy/hkpyo/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo.py` & `hkpy-2.9.0/hkpy/hkpyo/hkb/hkbo.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/hkb/hkbo_simple.py` & `hkpy-2.9.0/hkpy/hkpyo/hkb/hkbo_simple.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/model/hko_model.py` & `hkpy-2.9.0/hkpy/hkpyo/model/hko_model.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/hkpyo/reasoners/simple_reasoner.py` & `hkpy-2.9.0/hkpy/hkpyo/reasoners/simple_reasoner.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/oops/oops.py` & `hkpy-2.9.0/hkpy/oops/oops.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/utils/constants.py` & `hkpy-2.9.0/hkpy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy/utils/misc.py` & `hkpy-2.9.0/hkpy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/hkpy.egg-info/PKG-INFO` & `hkpy-2.9.0/hkpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkpy
-Version: 2.8.1
+Version: 2.9.0
 Summary: A Python module to create software abstraction for accessing hyperknowledge graphs
 Home-page: https://github.com/ibm-hyperknowledge/hkpy
 Author: IBM Research Brazil
 Author-email: mmoreno@br.ibm.com
 License: MIT
 Keywords: Hyperknowlede,Knowledge Engineering
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hkpy-2.8.1/hkpy.egg-info/SOURCES.txt` & `hkpy-2.9.0/hkpy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./version.txt
+.venv/lib/python3.10/site-packages/build/py.typed
 .venv/lib/python3.10/site-packages/hkpy/py.typed
+.venv/lib/python3.10/site-packages/packaging/py.typed
 .venv/lib/python3.10/site-packages/pip/py.typed
+.venv/lib/python3.10/site-packages/tomli/py.typed
 hkpy/__init__.py
 hkpy/py.typed
 hkpy.egg-info/PKG-INFO
 hkpy.egg-info/SOURCES.txt
 hkpy.egg-info/dependency_links.txt
 hkpy.egg-info/requires.txt
 hkpy.egg-info/top_level.txt
```

### Comparing `hkpy-2.8.1/setup.py` & `hkpy-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/tests/test.py` & `hkpy-2.9.0/tests/test.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/tests/test_context.py` & `hkpy-2.9.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/tests/test_fi.py` & `hkpy-2.9.0/tests/test_fi.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/tests/test_literal.py` & `hkpy-2.9.0/tests/test_literal.py`

 * *Files identical despite different names*

### Comparing `hkpy-2.8.1/tests/test_simple_reasoner.py` & `hkpy-2.9.0/tests/test_simple_reasoner.py`

 * *Files identical despite different names*

