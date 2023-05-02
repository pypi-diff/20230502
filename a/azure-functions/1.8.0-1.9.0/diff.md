# Comparing `tmp/azure-functions-1.8.0.tar.gz` & `tmp/azure-functions-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-functions-1.8.0.tar", last modified: Sat Nov 13 01:58:59 2021, max compression
+gzip compressed data, was "azure-functions-1.9.0.tar", last modified: Sat Feb 12 20:08:09 2022, max compression
```

## Comparing `azure-functions-1.8.0.tar` & `azure-functions-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.459502 azure-functions-1.8.0/
--rw-r--r--   0 varadmeru   (501) staff       (20)     1162 2020-04-02 21:14:02.000000 azure-functions-1.8.0/LICENSE
--rw-r--r--   0 varadmeru   (501) staff       (20)       90 2020-04-02 21:14:02.000000 azure-functions-1.8.0/MANIFEST.in
--rw-r--r--   0 varadmeru   (501) staff       (20)     5617 2021-11-13 01:58:59.459708 azure-functions-1.8.0/PKG-INFO
--rw-r--r--   0 varadmeru   (501) staff       (20)     4735 2020-12-19 09:35:17.000000 azure-functions-1.8.0/README.md
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.108451 azure-functions-1.8.0/azure/
--rw-r--r--   0 varadmeru   (501) staff       (20)      160 2020-12-19 09:35:17.000000 azure-functions-1.8.0/azure/__init__.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.235101 azure-functions-1.8.0/azure/functions/
--rw-r--r--   0 varadmeru   (501) staff       (20)     1881 2021-11-13 01:53:13.000000 azure-functions-1.8.0/azure/functions/__init__.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     8738 2021-11-13 01:53:13.000000 azure-functions-1.8.0/azure/functions/_abc.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     1400 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/_cosmosdb.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     3720 2020-09-30 21:29:35.000000 azure-functions-1.8.0/azure/functions/_durable_functions.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     2861 2020-07-01 18:44:48.000000 azure-functions-1.8.0/azure/functions/_eventgrid.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     3107 2020-07-01 18:46:33.000000 azure-functions-1.8.0/azure/functions/_eventhub.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     6114 2021-10-21 04:54:02.000000 azure-functions-1.8.0/azure/functions/_http.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     5767 2021-11-13 01:53:13.000000 azure-functions-1.8.0/azure/functions/_http_asgi.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     7786 2021-11-13 01:53:13.000000 azure-functions-1.8.0/azure/functions/_http_wsgi.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      720 2020-07-01 18:46:08.000000 azure-functions-1.8.0/azure/functions/_kafka.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     2702 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/_queue.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    11060 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_servicebus.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.254002 azure-functions-1.8.0/azure/functions/_thirdparty/
--rw-r--r--   0 varadmeru   (501) staff       (20)        0 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/_thirdparty/__init__.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    12456 2020-07-01 18:42:29.000000 azure-functions-1.8.0/azure/functions/_thirdparty/typing_inspect.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.268820 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/
--rw-r--r--   0 varadmeru   (501) staff       (20)        0 2020-04-02 21:14:02.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/__init__.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     6431 2020-04-02 21:14:02.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/_compat.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    14054 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/_internal.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    91402 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/datastructures.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    22906 2020-04-02 21:14:02.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/exceptions.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    21790 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/formparser.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    41398 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/http.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    39261 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/urls.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    24410 2020-04-02 21:14:02.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/utils.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    34368 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/wsgi.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     3167 2020-12-07 20:27:16.000000 azure-functions-1.8.0/azure/functions/_utils.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     4305 2020-12-19 09:35:17.000000 azure-functions-1.8.0/azure/functions/blob.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     2262 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/cosmosdb.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     4335 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/durable_functions.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     4227 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/eventgrid.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     9338 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/eventhub.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.368976 azure-functions-1.8.0/azure/functions/extension/
--rw-r--r--   0 varadmeru   (501) staff       (20)      329 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/__init__.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     5328 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/extension/app_extension_base.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      699 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/app_extension_hooks.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      517 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/extension_hook_meta.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     7631 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/extension_meta.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      782 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/extension_scope.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     6207 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/func_extension_base.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      673 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/func_extension_hooks.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      228 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/extension/function_extension_exception.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     4534 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/http.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     9256 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/kafka.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    12299 2021-11-13 01:53:13.000000 azure-functions-1.8.0/azure/functions/meta.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     4931 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/queue.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    19000 2021-08-09 03:35:40.000000 azure-functions-1.8.0/azure/functions/servicebus.py
--rw-r--r--   0 varadmeru   (501) staff       (20)      921 2021-08-03 20:18:12.000000 azure-functions-1.8.0/azure/functions/timer.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.374658 azure-functions-1.8.0/azure_functions.egg-info/
--rw-r--r--   0 varadmeru   (501) staff       (20)     5617 2021-11-13 01:58:58.000000 azure-functions-1.8.0/azure_functions.egg-info/PKG-INFO
--rw-r--r--   0 varadmeru   (501) staff       (20)     2292 2021-11-13 01:58:58.000000 azure-functions-1.8.0/azure_functions.egg-info/SOURCES.txt
--rw-r--r--   0 varadmeru   (501) staff       (20)        1 2021-11-13 01:58:58.000000 azure-functions-1.8.0/azure_functions.egg-info/dependency_links.txt
--rw-r--r--   0 varadmeru   (501) staff       (20)       67 2021-11-13 01:58:58.000000 azure-functions-1.8.0/azure_functions.egg-info/requires.txt
--rw-r--r--   0 varadmeru   (501) staff       (20)        6 2021-11-13 01:58:58.000000 azure-functions-1.8.0/azure_functions.egg-info/top_level.txt
--rw-r--r--   0 varadmeru   (501) staff       (20)      434 2021-11-13 01:58:59.462988 azure-functions-1.8.0/setup.cfg
--rw-r--r--   0 varadmeru   (501) staff       (20)     1579 2021-08-09 03:35:40.000000 azure-functions-1.8.0/setup.py
-drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2021-11-13 01:58:59.458581 azure-functions-1.8.0/tests/
--rw-r--r--   0 varadmeru   (501) staff       (20)      508 2020-07-01 18:48:20.000000 azure-functions-1.8.0/tests/__init__.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     9153 2021-08-03 20:18:12.000000 azure-functions-1.8.0/tests/test_blob.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     2091 2021-11-13 01:53:13.000000 azure-functions-1.8.0/tests/test_code_quality.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     3705 2020-07-01 18:48:27.000000 azure-functions-1.8.0/tests/test_cosmosdb.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     7565 2020-12-19 09:51:09.000000 azure-functions-1.8.0/tests/test_durable_functions.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     6589 2020-07-01 18:48:36.000000 azure-functions-1.8.0/tests/test_eventgrid.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    13634 2021-08-09 03:35:40.000000 azure-functions-1.8.0/tests/test_eventhub.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    28782 2021-08-03 20:18:12.000000 azure-functions-1.8.0/tests/test_extension.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     3237 2020-07-01 18:48:44.000000 azure-functions-1.8.0/tests/test_http.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     6515 2021-11-13 01:53:13.000000 azure-functions-1.8.0/tests/test_http_asgi.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    11301 2021-11-13 01:53:13.000000 azure-functions-1.8.0/tests/test_http_wsgi.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    10556 2021-08-09 03:35:40.000000 azure-functions-1.8.0/tests/test_kafka.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    10033 2021-11-13 01:53:13.000000 azure-functions-1.8.0/tests/test_meta.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     2204 2021-08-03 20:18:12.000000 azure-functions-1.8.0/tests/test_queue.py
--rw-r--r--   0 varadmeru   (501) staff       (20)    22030 2021-08-03 20:18:12.000000 azure-functions-1.8.0/tests/test_servicebus.py
--rw-r--r--   0 varadmeru   (501) staff       (20)     1083 2020-12-07 20:27:16.000000 azure-functions-1.8.0/tests/testutils.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.887057 azure-functions-1.9.0/
+-rw-r--r--   0 varadmeru   (501) staff       (20)     1162 2022-01-20 09:30:37.000000 azure-functions-1.9.0/LICENSE
+-rw-r--r--   0 varadmeru   (501) staff       (20)       90 2022-01-20 09:30:37.000000 azure-functions-1.9.0/MANIFEST.in
+-rw-r--r--   0 varadmeru   (501) staff       (20)     5665 2022-02-12 20:08:09.887181 azure-functions-1.9.0/PKG-INFO
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4783 2022-01-20 09:30:37.000000 azure-functions-1.9.0/README.md
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.793213 azure-functions-1.9.0/azure/
+-rw-r--r--   0 varadmeru   (501) staff       (20)      160 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/__init__.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.815003 azure-functions-1.9.0/azure/functions/
+-rw-r--r--   0 varadmeru   (501) staff       (20)     1881 2022-02-12 20:05:00.000000 azure-functions-1.9.0/azure/functions/__init__.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     8738 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_abc.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     1400 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_cosmosdb.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     3720 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_durable_functions.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2861 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_eventgrid.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     3107 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_eventhub.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     6114 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_http.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     5799 2022-02-12 20:03:33.000000 azure-functions-1.9.0/azure/functions/_http_asgi.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     7786 2022-02-09 15:32:50.000000 azure-functions-1.9.0/azure/functions/_http_wsgi.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      720 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_kafka.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2702 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_queue.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    11060 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_servicebus.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.816114 azure-functions-1.9.0/azure/functions/_thirdparty/
+-rw-r--r--   0 varadmeru   (501) staff       (20)        0 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/__init__.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    12456 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/typing_inspect.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.830063 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/
+-rw-r--r--   0 varadmeru   (501) staff       (20)        0 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/__init__.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     6431 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/_compat.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    14054 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/_internal.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    91402 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/datastructures.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    22906 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/exceptions.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    21790 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/formparser.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    41398 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/http.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    39261 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/urls.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    24410 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/utils.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    34368 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/wsgi.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     3167 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/_utils.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4305 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/blob.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2262 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/cosmosdb.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4335 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/durable_functions.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4227 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/eventgrid.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     9338 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/eventhub.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.836205 azure-functions-1.9.0/azure/functions/extension/
+-rw-r--r--   0 varadmeru   (501) staff       (20)      329 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/__init__.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     5328 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/app_extension_base.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      699 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/app_extension_hooks.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      517 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/extension_hook_meta.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     7592 2022-02-12 20:03:33.000000 azure-functions-1.9.0/azure/functions/extension/extension_meta.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      782 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/extension_scope.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     6207 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/func_extension_base.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      673 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/func_extension_hooks.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      228 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/extension/function_extension_exception.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4534 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/http.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     9950 2022-02-12 20:03:33.000000 azure-functions-1.9.0/azure/functions/kafka.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    12299 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/meta.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     4931 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/queue.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    19000 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/servicebus.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)      921 2022-01-20 09:30:37.000000 azure-functions-1.9.0/azure/functions/timer.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.839836 azure-functions-1.9.0/azure_functions.egg-info/
+-rw-r--r--   0 varadmeru   (501) staff       (20)     5665 2022-02-12 20:08:09.000000 azure-functions-1.9.0/azure_functions.egg-info/PKG-INFO
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2292 2022-02-12 20:08:09.000000 azure-functions-1.9.0/azure_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 varadmeru   (501) staff       (20)        1 2022-02-12 20:08:09.000000 azure-functions-1.9.0/azure_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 varadmeru   (501) staff       (20)       67 2022-02-12 20:08:09.000000 azure-functions-1.9.0/azure_functions.egg-info/requires.txt
+-rw-r--r--   0 varadmeru   (501) staff       (20)       12 2022-02-12 20:08:09.000000 azure-functions-1.9.0/azure_functions.egg-info/top_level.txt
+-rw-r--r--   0 varadmeru   (501) staff       (20)      434 2022-02-12 20:08:09.888707 azure-functions-1.9.0/setup.cfg
+-rw-r--r--   0 varadmeru   (501) staff       (20)     1531 2022-01-20 09:30:37.000000 azure-functions-1.9.0/setup.py
+drwxr-xr-x   0 varadmeru   (501) staff       (20)        0 2022-02-12 20:08:09.886628 azure-functions-1.9.0/tests/
+-rw-r--r--   0 varadmeru   (501) staff       (20)      508 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/__init__.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     9153 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_blob.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2091 2022-02-09 13:50:05.000000 azure-functions-1.9.0/tests/test_code_quality.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     3705 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_cosmosdb.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     7565 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_durable_functions.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     6589 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_eventgrid.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    13634 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_eventhub.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    28782 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_extension.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     3237 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_http.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     6515 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_http_asgi.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    11301 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_http_wsgi.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    11080 2022-02-12 20:03:33.000000 azure-functions-1.9.0/tests/test_kafka.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    10033 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_meta.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     2204 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_queue.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)    22030 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/test_servicebus.py
+-rw-r--r--   0 varadmeru   (501) staff       (20)     1083 2022-01-20 09:30:37.000000 azure-functions-1.9.0/tests/testutils.py
```

### Comparing `azure-functions-1.8.0/LICENSE` & `azure-functions-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/PKG-INFO` & `azure-functions-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions
-Version: 1.8.0
+Version: 1.9.0
 Summary: Azure Functions for Python
 Home-page: UNKNOWN
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -28,24 +28,26 @@
 |Branch|Status|Coverage|CodeCov|
 |---|---|---|---|
 |master|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=master)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=master)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/master)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/master/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 |dev|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=dev)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=dev)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/dev)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/dev/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 
 ## Overview
 
-Python support for Azure Functions is based on Python 3.6/3.7/3.8 and 3.9 (coming soon), serverless hosting on Linux and the Functions 2.0 runtime.
+Python support for Azure Functions is based on Python 3.6/3.7/3.8/3.9 and 3.10 (coming soon), serverless hosting on Linux and the Functions 2.0, 3.0
+and 4.0 runtime.
 
 Here is the current status of Python in Azure Functions:
 
 _What are the supported Python versions?_
 
 |Azure Functions Runtime|Python 3.6|Python 3.7|Python 3.8|Python 3.9|
 |---|---|---|---|---|
 |Azure Functions 2.0|✔|✔|-|-|
-|Azure Functions 3.0|✔|✔|✔|(preview)|
+|Azure Functions 3.0|✔|✔|✔|✔|
+|Azure Functions 4.0|-|✔|✔|✔|
 
 _What's available?_
 - Build, test, debug and publish using Azure Functions Core Tools (CLI) or Visual Studio Code
 - Triggers / Bindings : HTTP, Blob, Queue, Timer, Cosmos DB, Event Grid, Event Hubs and Service Bus
 - Create a Python Function on Linux using a custom docker image
 - Triggers / Bindings : Custom binding support
```

### Comparing `azure-functions-1.8.0/README.md` & `azure-functions-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 |Branch|Status|Coverage|CodeCov|
 |---|---|---|---|
 |master|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=master)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=master)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/master)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/master/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 |dev|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=dev)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=dev)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/dev)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/dev/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 
 ## Overview
 
-Python support for Azure Functions is based on Python 3.6/3.7/3.8 and 3.9 (coming soon), serverless hosting on Linux and the Functions 2.0 runtime.
+Python support for Azure Functions is based on Python 3.6/3.7/3.8/3.9 and 3.10 (coming soon), serverless hosting on Linux and the Functions 2.0, 3.0
+and 4.0 runtime.
 
 Here is the current status of Python in Azure Functions:
 
 _What are the supported Python versions?_
 
 |Azure Functions Runtime|Python 3.6|Python 3.7|Python 3.8|Python 3.9|
 |---|---|---|---|---|
 |Azure Functions 2.0|✔|✔|-|-|
-|Azure Functions 3.0|✔|✔|✔|(preview)|
+|Azure Functions 3.0|✔|✔|✔|✔|
+|Azure Functions 4.0|-|✔|✔|✔|
 
 _What's available?_
 - Build, test, debug and publish using Azure Functions Core Tools (CLI) or Visual Studio Code
 - Triggers / Bindings : HTTP, Blob, Queue, Timer, Cosmos DB, Event Grid, Event Hubs and Service Bus
 - Create a Python Function on Linux using a custom docker image
 - Triggers / Bindings : Custom binding support
```

### Comparing `azure-functions-1.8.0/azure/functions/__init__.py` & `azure-functions-1.9.0/azure/functions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,8 +63,8 @@
     # Extensions
     'AppExtensionBase',
     'FuncExtensionBase',
     'ExtensionMeta',
     'FunctionExtensionException'
 )
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
```

### Comparing `azure-functions-1.8.0/azure/functions/_abc.py` & `azure-functions-1.9.0/azure/functions/_abc.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_cosmosdb.py` & `azure-functions-1.9.0/azure/functions/_cosmosdb.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_durable_functions.py` & `azure-functions-1.9.0/azure/functions/_durable_functions.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_eventgrid.py` & `azure-functions-1.9.0/azure/functions/_eventgrid.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_eventhub.py` & `azure-functions-1.9.0/azure/functions/_eventhub.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_http.py` & `azure-functions-1.9.0/azure/functions/_http.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_http_asgi.py` & `azure-functions-1.9.0/azure/functions/_http_asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
             "type": "http",
             "asgi.version": self.asgi_version,
             "asgi.spec_version": self.asgi_spec_version,
             "http_version": "1.1",
             "method": self.request_method,
             "scheme": "https",
             "path": self.path_info,
-            "raw_path": self.path_info.encode("utf-8"),
-            "query_string": self.query_string.encode("utf-8"),
+            "raw_path": self.path_info.encode("utf-8"),  # type: ignore
+            "query_string": self.query_string.encode("utf-8"),  # type: ignore
             "root_path": self.script_name,
             "headers": self._get_encoded_http_headers(),
             "server": self._get_server_address(),
             "client": None,
             "azure_functions.function_directory": self.af_function_directory,
             "azure_functions.function_name": self.af_function_name,
             "azure_functions.invocation_id": self.af_invocation_id,
```

### Comparing `azure-functions-1.8.0/azure/functions/_http_wsgi.py` & `azure-functions-1.9.0/azure/functions/_http_wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_kafka.py` & `azure-functions-1.9.0/azure/functions/_kafka.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_queue.py` & `azure-functions-1.9.0/azure/functions/_queue.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_servicebus.py` & `azure-functions-1.9.0/azure/functions/_servicebus.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/typing_inspect.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/typing_inspect.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/_compat.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/_compat.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/_internal.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/_internal.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/datastructures.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/datastructures.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/exceptions.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/formparser.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/formparser.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/http.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/http.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/urls.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/urls.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/utils.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/utils.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_thirdparty/werkzeug/wsgi.py` & `azure-functions-1.9.0/azure/functions/_thirdparty/werkzeug/wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/_utils.py` & `azure-functions-1.9.0/azure/functions/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/blob.py` & `azure-functions-1.9.0/azure/functions/blob.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/cosmosdb.py` & `azure-functions-1.9.0/azure/functions/cosmosdb.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/durable_functions.py` & `azure-functions-1.9.0/azure/functions/durable_functions.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/eventgrid.py` & `azure-functions-1.9.0/azure/functions/eventgrid.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/eventhub.py` & `azure-functions-1.9.0/azure/functions/eventhub.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/app_extension_base.py` & `azure-functions-1.9.0/azure/functions/extension/app_extension_base.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/app_extension_hooks.py` & `azure-functions-1.9.0/azure/functions/extension/app_extension_hooks.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/extension_hook_meta.py` & `azure-functions-1.9.0/azure/functions/extension/extension_hook_meta.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/extension_meta.py` & `azure-functions-1.9.0/azure/functions/extension/extension_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,15 @@
             }
         """
         return json.dumps(cls._info)
 
     @classmethod
     def _get_extension_scope(cls, extension) -> ExtensionScope:
         """Return the scope of an extension"""
-        return getattr(extension, '_scope',  # type: ignore
-                       ExtensionScope.UNKNOWN)
+        return getattr(extension, '_scope', ExtensionScope.UNKNOWN)
 
     @classmethod
     def _set_hooks_for_function(cls, trigger_name: str, ext):
         ext_hooks = cls._func_exts.setdefault(
             trigger_name.lower(),
             cls._create_default_function_hook()
         )
```

### Comparing `azure-functions-1.8.0/azure/functions/extension/extension_scope.py` & `azure-functions-1.9.0/azure/functions/extension/extension_scope.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/func_extension_base.py` & `azure-functions-1.9.0/azure/functions/extension/func_extension_base.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/extension/func_extension_hooks.py` & `azure-functions-1.9.0/azure/functions/extension/func_extension_hooks.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/http.py` & `azure-functions-1.9.0/azure/functions/http.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/kafka.py` & `azure-functions-1.9.0/azure/functions/kafka.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,24 @@
     def __init__(self, *,
                  body: bytes,
                  trigger_metadata: typing.Mapping[str, meta.Datum] = None,
                  key: typing.Optional[str] = None,
                  offset: typing.Optional[int] = None,
                  partition: typing.Optional[int] = None,
                  topic: typing.Optional[str] = None,
-                 timestamp: typing.Optional[str] = None) -> None:
+                 timestamp: typing.Optional[str] = None,
+                 headers: typing.Optional[list] = None) -> None:
         self.__body = body
         self.__trigger_metadata = trigger_metadata
         self.__key = key
         self.__offset = offset
         self.__partition = partition
         self.__topic = topic
         self.__timestamp = timestamp
+        self.__headers = headers
 
         # Cache for trigger metadata after Python object conversion
         self._trigger_metadata_pyobj: typing.Optional[
             typing.Mapping[str, typing.Any]] = None
 
     def get_body(self) -> bytes:
         return self.__body
@@ -54,14 +56,18 @@
         return self.__topic
 
     @property
     def timestamp(self) -> typing.Optional[str]:
         return self.__timestamp
 
     @property
+    def headers(self) -> typing.Optional[list]:
+        return self.__headers
+
+    @property
     def metadata(self) -> typing.Optional[typing.Mapping[str, typing.Any]]:
         if self.__trigger_metadata is None:
             return None
 
         if self._trigger_metadata_pyobj is None:
             self._trigger_metadata_pyobj = {}
 
@@ -195,14 +201,16 @@
                 trigger_metadata, 'Key', python_type=str),
             partition=cls._decode_trigger_metadata_field(
                 trigger_metadata, 'Partition', python_type=int),
             offset=cls._decode_trigger_metadata_field(
                 trigger_metadata, 'Offset', python_type=int),
             topic=cls._decode_trigger_metadata_field(
                 trigger_metadata, 'Topic', python_type=str),
+            headers=cls._decode_trigger_metadata_field(
+                trigger_metadata, 'Headers', python_type=list),
             trigger_metadata=trigger_metadata
         )
 
     @classmethod
     def decode_multiple_events(cls, data: meta.Datum,
                                trigger_metadata) -> typing.List[KafkaEvent]:
         parsed_data: List[bytes] = []
@@ -216,14 +224,15 @@
             ]
 
         timestamp_props = trigger_metadata.get('TimestampArray')
         key_props = trigger_metadata.get('KeyArray')
         partition_props = trigger_metadata.get('PartitionArray')
         offset_props = trigger_metadata.get('OffsetArray')
         topic_props = trigger_metadata.get('TopicArray')
+        header_props = trigger_metadata.get('HeadersArray')
 
         parsed_timestamp_props: List[Any] = cls.get_parsed_props(
             timestamp_props, parsed_data)
 
         parsed_key_props = cls.get_parsed_props(
             key_props, parsed_data)
 
@@ -237,25 +246,32 @@
                 raise AssertionError(
                     'Number of bodies and metadata mismatched')
 
         parsed_topic_props: List[Any]
         if topic_props is not None:
             parsed_topic_props = [v for v in topic_props.value.string]
 
+        parsed_headers_props: List[Any]
+        if header_props is not None:
+            parsed_headers_list = cls.get_parsed_props(header_props,
+                                                       parsed_data)
+            parsed_headers_props = [v for v in parsed_headers_list]
+
         events = []
 
         for i in range(len(parsed_data)):
             event = KafkaEvent(
                 body=parsed_data[i],
                 timestamp=parsed_timestamp_props[i],
                 key=cls._decode_typed_data(
                     parsed_key_props[i], python_type=str),
                 partition=parsed_partition_props[i],
                 offset=parsed_offset_props[i],
                 topic=parsed_topic_props[i],
+                headers=parsed_headers_props[i],
                 trigger_metadata=trigger_metadata
             )
             events.append(event)
 
         return events
 
     @classmethod
```

### Comparing `azure-functions-1.8.0/azure/functions/meta.py` & `azure-functions-1.9.0/azure/functions/meta.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/queue.py` & `azure-functions-1.9.0/azure/functions/queue.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/servicebus.py` & `azure-functions-1.9.0/azure/functions/servicebus.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure/functions/timer.py` & `azure-functions-1.9.0/azure/functions/timer.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/azure_functions.egg-info/PKG-INFO` & `azure-functions-1.9.0/azure_functions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-functions
-Version: 1.8.0
+Version: 1.9.0
 Summary: Azure Functions for Python
 Home-page: UNKNOWN
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -28,24 +28,26 @@
 |Branch|Status|Coverage|CodeCov|
 |---|---|---|---|
 |master|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=master)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=master)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/master)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/master/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 |dev|[![Build Status](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_apis/build/status/Azure%20Functions%20Python-CI?branchName=dev)](https://azfunc.visualstudio.com/Azure%20Functions%20Python/_build/latest?definitionId=19&branchName=dev)|![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/azfunc/Azure%20Functions%20Python/19/dev)|[![codecov](https://codecov.io/gh/Azure/azure-functions-python-library/branch/dev/graph/badge.svg)](https://codecov.io/gh/Azure/azure-functions-python-library)
 
 ## Overview
 
-Python support for Azure Functions is based on Python 3.6/3.7/3.8 and 3.9 (coming soon), serverless hosting on Linux and the Functions 2.0 runtime.
+Python support for Azure Functions is based on Python 3.6/3.7/3.8/3.9 and 3.10 (coming soon), serverless hosting on Linux and the Functions 2.0, 3.0
+and 4.0 runtime.
 
 Here is the current status of Python in Azure Functions:
 
 _What are the supported Python versions?_
 
 |Azure Functions Runtime|Python 3.6|Python 3.7|Python 3.8|Python 3.9|
 |---|---|---|---|---|
 |Azure Functions 2.0|✔|✔|-|-|
-|Azure Functions 3.0|✔|✔|✔|(preview)|
+|Azure Functions 3.0|✔|✔|✔|✔|
+|Azure Functions 4.0|-|✔|✔|✔|
 
 _What's available?_
 - Build, test, debug and publish using Azure Functions Core Tools (CLI) or Visual Studio Code
 - Triggers / Bindings : HTTP, Blob, Queue, Timer, Cosmos DB, Event Grid, Event Hubs and Service Bus
 - Create a Python Function on Linux using a custom docker image
 - Triggers / Bindings : Custom binding support
```

### Comparing `azure-functions-1.8.0/azure_functions.egg-info/SOURCES.txt` & `azure-functions-1.9.0/azure_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/setup.py` & `azure-functions-1.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 
-from setuptools import setup
+from setuptools import find_packages, setup
 from azure.functions import __version__
 
 with open("README.md") as readme:
     long_description = readme.read()
 
 setup(
     name='azure-functions',
@@ -26,19 +26,17 @@
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Operating System :: MacOS :: MacOS X',
         'Environment :: Web Environment',
         'Development Status :: 5 - Production/Stable',
     ],
     license='MIT',
-    packages=[
-        'azure.functions',
-        'azure.functions.extension',
-        'azure.functions._thirdparty'
-    ],
+    packages=find_packages(exclude=[
+        'azure'
+    ]),
     package_data={
         'azure.functions': ['py.typed']
     },
     extras_require={
         'dev': [
             'flake8~=3.7.9',
             'mypy',
```

### Comparing `azure-functions-1.8.0/tests/test_blob.py` & `azure-functions-1.9.0/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_code_quality.py` & `azure-functions-1.9.0/tests/test_code_quality.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_cosmosdb.py` & `azure-functions-1.9.0/tests/test_cosmosdb.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_durable_functions.py` & `azure-functions-1.9.0/tests/test_durable_functions.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_eventgrid.py` & `azure-functions-1.9.0/tests/test_eventgrid.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_eventhub.py` & `azure-functions-1.9.0/tests/test_eventhub.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_extension.py` & `azure-functions-1.9.0/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_http.py` & `azure-functions-1.9.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_http_asgi.py` & `azure-functions-1.9.0/tests/test_http_asgi.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_http_wsgi.py` & `azure-functions-1.9.0/tests/test_http_wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_kafka.py` & `azure-functions-1.9.0/tests/test_kafka.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 import azure.functions.meta as meta
 
 from .testutils import CollectionBytes, CollectionString, CollectionSint64
 
 
 class Kafka(unittest.TestCase):
     SINGLE_KAFKA_DATAUM = '{"Offset":1,"Partition":0,"Topic":"users",'\
-        '"Timestamp":"2020-06-20T04:43:28.998Z","Value":"hello"}'
+        '"Timestamp":"2020-06-20T04:43:28.998Z","Value":"hello", ' \
+                          '"Headers":[{"Key":"test","Value":"1"}]}'
     SINGLE_KAFKA_TIMESTAMP = "2020-06-20T04:43:28.998Z"
     MULTIPLE_KAFKA_TIMESTAMP_0 = "2020-06-20T05:06:25.139Z"
     MULTIPLE_KAFKA_TIMESTAMP_1 = "2020-06-20T05:06:25.945Z"
     MULTIPLE_KAFKA_DATA_0 = '{"Offset":62,"Partition":1,"Topic":"message",'\
-        '"Timestamp":"2020-06-20T05:06:25.139Z","Value":"a"}'
+        '"Timestamp":"2020-06-20T05:06:25.139Z","Value":"a", ' \
+                            '"Headers":[{"Key":"test","Value":"1"}]}'
     MULTIPLE_KAFKA_DATA_1 = '{"Offset":63,"Partition":1,"Topic":"message",'\
-        '"Timestamp":"2020-06-20T05:06:25.945Z","Value":"a"}'
+        '"Timestamp":"2020-06-20T05:06:25.945Z","Value":"a", ' \
+                            '"Headers":[{"Key":"test2","Value":"2"}]}'
 
     def test_kafka_input_type(self):
         check_input_type = (
             azf_ka.KafkaConverter.check_input_type_annotation
         )
         self.assertTrue(check_input_type(func.KafkaEvent))
         self.assertTrue(check_input_type(List[func.KafkaEvent]))
@@ -198,17 +201,19 @@
         datum = self.SINGLE_KAFKA_DATAUM
         if datum_type == 'bytes':
             datum = datum.encode('utf-8')
         return meta.Datum(datum, datum_type)
 
     def _generate_multiple_kafka_data(self, data_type='json'):
         data = '[{"Offset":62,"Partition":1,"Topic":"message",'\
-               '"Timestamp":"2020-06-20T05:06:25.139Z","Value":"a"},'\
+               '"Timestamp":"2020-06-20T05:06:25.139Z","Value":"a",' \
+               ' "Headers":[{"Key":"test","Value":"1"}]},'\
                ' {"Offset":63,"Partition":1,"Topic":"message",'\
-               '"Timestamp":"2020-06-20T05:06:25.945Z","Value":"a"}]'
+               '"Timestamp":"2020-06-20T05:06:25.945Z","Value":"a", ' \
+               '"Headers":[{"Key":"test2","Value":"2"}]}]'
         if data_type == 'collection_bytes':
             data = list(
                 map(lambda x: json.dumps(x).encode('utf-8'),
                     json.loads(data))
             )
             data = CollectionBytes(data)
         elif data_type == 'collection_string':
@@ -262,14 +267,18 @@
             ),
             'TimestampArray': meta.Datum(
                 json.dumps(timestamp_array), 'json'
             ),
             'TopicArray': meta.Datum(
                 CollectionString(['message', 'message']), "collection_string"
             ),
+            'HeadersArray': meta.Datum(
+                json.dumps([['{"Key":"test","Value":"1"}'],
+                            ['{"Key":"test2","Value":"2"}']]), 'json'
+            ),
             'sys': meta.Datum(
                 '{"MethodName":"KafkaTriggerMany",'
                 '"UtcNow":"2020-06-20T05:06:26.5550868Z",'
                 '"RandGuid":"57d5eeb7-c86c-4924-a14a-160092154093"}',
                 'json'
             )
         }
```

### Comparing `azure-functions-1.8.0/tests/test_meta.py` & `azure-functions-1.9.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_queue.py` & `azure-functions-1.9.0/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/test_servicebus.py` & `azure-functions-1.9.0/tests/test_servicebus.py`

 * *Files identical despite different names*

### Comparing `azure-functions-1.8.0/tests/testutils.py` & `azure-functions-1.9.0/tests/testutils.py`

 * *Files identical despite different names*

