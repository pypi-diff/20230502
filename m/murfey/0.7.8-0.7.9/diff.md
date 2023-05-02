# Comparing `tmp/murfey-0.7.8.tar.gz` & `tmp/murfey-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murfey-0.7.8.tar", last modified: Sun Apr 16 20:50:50 2023, max compression
+gzip compressed data, was "murfey-0.7.9.tar", last modified: Mon Apr 17 22:01:18 2023, max compression
```

## Comparing `murfey-0.7.8.tar` & `murfey-0.7.9.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.841428 murfey-0.7.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-16 20:50:45.000000 murfey-0.7.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-16 20:50:45.000000 murfey-0.7.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-16 20:50:50.841428 murfey-0.7.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-16 20:50:45.000000 murfey-0.7.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-16 20:50:45.000000 murfey-0.7.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-16 20:50:50.841428 murfey-0.7.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-16 20:50:45.000000 murfey-0.7.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.825428 murfey-0.7.8/src/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/
--rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/bootstrap/
--rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/bootstrap/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/dummy.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/cli/transfer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.833428 murfey-0.7.8/src/murfey/client/
--rw-r--r--   0 vsts      (1001) docker     (122)    10265 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12896 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/analyser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    44190 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/context.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.833428 murfey-0.7.8/src/murfey/client/contexts/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/contexts/tomo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/customlogging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/gain_ref.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7084 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/instance_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/rsync.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/client/tui/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19676 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5101 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/controller.css
--rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/forms.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/launcher.css
--rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/progress.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32434 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/screens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/tui/status_bar.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/watchdir.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/watchdir_multigrid.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/client/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/server/
--rw-r--r--   0 vsts      (1001) docker     (122)    18740 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18416 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/bootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (122)      978 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11850 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/demo_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/gain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/ispyb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/server/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/activevisits.html
--rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/base.html
--rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/bootstrap.html
--rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/home.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/images/
--rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/images/diamond.png
--rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/images/icon_268.png
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.837428 murfey-0.7.8/src/murfey/templates/static/
--rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/static/styles.css
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/templates/visit.html
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.841428 murfey-0.7.8/src/murfey/util/
--rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/dummy_setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/file_monitor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/mdoc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4128 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/rsync.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-16 20:50:45.000000 murfey-0.7.8/src/murfey/util/state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-16 20:50:50.829428 murfey-0.7.8/src/murfey.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-16 20:50:50.000000 murfey-0.7.8/src/murfey.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.650686 murfey-0.7.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1481 2023-04-17 22:01:13.000000 murfey-0.7.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-17 22:01:13.000000 murfey-0.7.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-17 22:01:18.650686 murfey-0.7.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1698 2023-04-17 22:01:13.000000 murfey-0.7.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      206 2023-04-17 22:01:13.000000 murfey-0.7.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-04-17 22:01:18.650686 murfey-0.7.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-04-17 22:01:13.000000 murfey-0.7.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.642686 murfey-0.7.9/src/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.642686 murfey-0.7.9/src/murfey/
+-rw-r--r--   0 vsts      (1001) docker     (122)       97 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.642686 murfey-0.7.9/src/murfey/bootstrap/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4237 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/bootstrap/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/cli/dummy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2621 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/cli/transfer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/client/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10265 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12868 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/analyser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    46053 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/context.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/client/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2476 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/contexts/tomo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1466 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/customlogging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/gain_ref.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7084 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/instance_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11696 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/rsync.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/client/tui/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19676 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5101 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/controller.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      179 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/launcher.css
+-rw-r--r--   0 vsts      (1001) docker     (122)     5280 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32434 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/screens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/tui/status_bar.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2594 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9178 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/watchdir.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2204 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/watchdir_multigrid.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4895 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/client/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/server/
+-rw-r--r--   0 vsts      (1001) docker     (122)    18740 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18416 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8109 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/bootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      978 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11850 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/demo_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1875 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/gain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/ispyb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4265 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/server/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      671 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/activevisits.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      891 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/base.html
+-rw-r--r--   0 vsts      (1001) docker     (122)     1148 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/bootstrap.html
+-rw-r--r--   0 vsts      (1001) docker     (122)      242 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/home.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.646686 murfey-0.7.9/src/murfey/templates/images/
+-rw-r--r--   0 vsts      (1001) docker     (122)   131288 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/images/diamond.png
+-rw-r--r--   0 vsts      (1001) docker     (122)    14468 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/images/icon_268.png
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.650686 murfey-0.7.9/src/murfey/templates/static/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1420 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/static/styles.css
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/templates/visit.html
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.650686 murfey-0.7.9/src/murfey/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3390 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3262 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/dummy_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/file_monitor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1133 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/mdoc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4128 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6530 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/rsync.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3210 2023-04-17 22:01:13.000000 murfey-0.7.9/src/murfey/util/state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 22:01:18.642686 murfey-0.7.9/src/murfey.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2463 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1947 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      252 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-17 22:01:18.000000 murfey-0.7.9/src/murfey.egg-info/top_level.txt
```

### Comparing `murfey-0.7.8/LICENSE` & `murfey-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/PKG-INFO` & `murfey-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.8
+Version: 0.7.9
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.8/README.md` & `murfey-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/setup.cfg` & `murfey-0.7.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = murfey
 description = Client-Server architecture hauling Cryo-EM data
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 0.7.8
+version = 0.7.9
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `murfey-0.7.8/src/murfey/bootstrap/__main__.py` & `murfey-0.7.9/src/murfey/bootstrap/__main__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/cli/dummy.py` & `murfey-0.7.9/src/murfey/cli/dummy.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/cli/transfer.py` & `murfey-0.7.9/src/murfey/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/__init__.py` & `murfey-0.7.9/src/murfey/client/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/analyser.py` & `murfey-0.7.9/src/murfey/client/analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,16 @@
                         dc_metadata = self._context.gather_metadata(
                             self._xml_file(transferred_file),
                             environment=self._environment,
                         )
                     self.notify({"form": dc_metadata})
 
     def _xml_file(self, data_file: Path) -> Path:
-        if (fxml := data_file.with_suffix(".xml")).is_file() or not self._environment:
-            return fxml
+        if not self._environment:
+            return data_file.with_suffix(".xml")
         file_name = (
             f"{data_file.stem.replace('_fractions', '').replace('_Fractions', '')}.xml"
         )
         data_directories = get_machine_config(self._environment.url.geturl()).get(
             "data_directories", {}
         )
         for dd in data_directories.keys():
```

### Comparing `murfey-0.7.8/src/murfey/client/context.py` & `murfey-0.7.9/src/murfey/client/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -239,14 +239,15 @@
             metadata["image_size_x"] = data["Acquisition"]["Info"]["ImageSize"]["Width"]
             metadata["image_size_y"] = data["Acquisition"]["Info"]["ImageSize"][
                 "Height"
             ]
             metadata["pixel_size_on_image"] = float(
                 data["Acquisition"]["Info"]["SensorPixelSize"]["Height"]
             )
+            metadata["magnification"] = magnification
         elif data.get("MicroscopeImage"):
             metadata["voltage"] = (
                 float(
                     data["MicroscopeImage"]["microscopeData"]["gun"][
                         "AccelerationVoltage"
                     ]
                 )
@@ -309,24 +310,61 @@
         metadata["motion_corr_binning"] = binning_factor
         metadata["gain_ref"] = None
         metadata["dose_per_frame"] = (
             environment.data_collection_parameters.get("dose_per_frame")
             if environment
             else None
         )
-        metadata["use_cryolo"] = True
-        metadata["symmetry"] = "C1"
-        metadata["mask_diameter"] = 190
-        metadata["boxsize"] = 256
-        metadata["downscale"] = False
-        metadata["small_boxsize"] = 128
-        metadata["eer_grouping"] = 20
+
+        metadata["use_cryolo"] = (
+            environment.data_collection_parameters.get("use_cryolo")
+            if environment
+            else None
+        ) or True
+        metadata["symmetry"] = (
+            environment.data_collection_parameters.get("symmetry")
+            if environment
+            else None
+        ) or "C1"
+        metadata["mask_diameter"] = (
+            environment.data_collection_parameters.get("mask_diameter")
+            if environment
+            else None
+        ) or 190
+        metadata["boxsize"] = (
+            environment.data_collection_parameters.get("boxsize")
+            if environment
+            else None
+        ) or 256
+        metadata["downscale"] = (
+            environment.data_collection_parameters.get("downscale")
+            if environment
+            else None
+        ) or True
+        metadata["small_boxsize"] = (
+            environment.data_collection_parameters.get("small_boxsize")
+            if environment
+            else None
+        ) or 128
+        metadata["eer_grouping"] = (
+            environment.data_collection_parameters.get("eer_grouping")
+            if environment
+            else None
+        ) or 20
         metadata["source"] = str(self._basepath)
-        metadata["particle_diameter"] = 0
-        metadata["estimate_particle_diameter"] = True
+        metadata["particle_diameter"] = (
+            environment.data_collection_parameters.get("particle_diameter")
+            if environment
+            else None
+        ) or 0
+        metadata["estimate_particle_diameter"] = (
+            environment.data_collection_parameters.get("estimate_particle_diameter")
+            if environment
+            else None
+        ) or True
         return metadata
 
 
 class ProcessFileIncomplete(BaseModel):
     dest: Path
     source: Path
     image_number: int
@@ -351,15 +389,15 @@
         ProcessingParameter("motion_corr_binning", "Motion Correction Binning"),
     ]
 
     def __init__(self, acquisition_software: str, basepath: Path):
         super().__init__(acquisition_software)
         self._basepath = basepath
         self._tilt_series: Dict[str, List[Path]] = {}
-        self._tilt_series_sizes: Dict[str, int | None] = {}
+        self._tilt_series_sizes: Dict[str, int] = {}
         self._completed_tilt_series: List[str] = []
         self._aligned_tilt_series: List[str] = []
         self._motion_corrected_tilt_series: Dict[str, List[Path]] = {}
         self._last_transferred_file: Path | None = None
         self._data_collection_stash: list = []
         self._processing_job_stash: dict = {}
         self._preprocessing_triggers: dict = {}
@@ -480,32 +518,56 @@
                     "gain_ref": environment.data_collection_parameters.get("gain_ref"),
                 }
                 return new_dict
         except KeyError:
             logger.warning("Key error encountered in _complete_process_file")
             return {}
 
+    def _file_transferred_to(
+        self, environment: MurfeyInstanceEnvironment, source: Path, file_path: Path
+    ):
+        machine_config = get_machine_config(
+            str(environment.url.geturl()), demo=environment.demo
+        )
+        if environment.visit in environment.default_destinations[source]:
+            return (
+                Path(machine_config.get("rsync_basepath", ""))
+                / Path(environment.default_destinations[source])
+                / file_path.name
+            )
+        return (
+            Path(machine_config.get("rsync_basepath", ""))
+            / Path(environment.default_destinations[source])
+            / environment.visit
+            / file_path.name
+        )
+
+    def _get_source(
+        self, file_path: Path, environment: MurfeyInstanceEnvironment
+    ) -> Path | None:
+        for s in environment.sources:
+            if file_path.is_relative_to(s):
+                return s
+        return None
+
     def _add_tilt(
         self,
         file_path: Path,
         extract_tilt_series: Callable[[Path], str],
         extract_tilt_angle: Callable[[Path], str],
         extract_tilt_tag: Callable[[Path], str],
         environment: MurfeyInstanceEnvironment | None = None,
         required_position_files: List[Path] | None = None,
         required_strings: List[str] | None = None,
     ) -> List[str]:
         if not environment:
             logger.warning("No environment passed in")
             return []
-        for s in environment.sources:
-            if file_path.is_relative_to(s):
-                source = s
-                break
-        else:
+        source = self._get_source(file_path, environment)
+        if not source:
             logger.warning(f"No source found for file {file_path}")
             return []
         # required_position_files = required_position_files or []
         required_strings = (
             ["fractions"] if required_strings is None else required_strings
         )
         for r in required_strings:
@@ -531,30 +593,17 @@
         except Exception:
             logger.debug(
                 f"Tilt series and angle could not be determined for {file_path}"
             )
             return []
 
         if environment:
-            machine_config = get_machine_config(
-                str(environment.url.geturl()), demo=environment.demo
+            file_transferred_to = self._file_transferred_to(
+                environment, source, file_path
             )
-            if environment.visit in environment.default_destinations[source]:
-                file_transferred_to = (
-                    Path(machine_config.get("rsync_basepath", ""))
-                    / Path(environment.default_destinations[source])
-                    / file_path.name
-                )
-            else:
-                file_transferred_to = (
-                    Path(machine_config.get("rsync_basepath", ""))
-                    / Path(environment.default_destinations[source])
-                    / environment.visit
-                    / file_path.name
-                )
             environment.movies[file_transferred_to] = MovieTracker(
                 movie_number=next(MovieID),
                 motion_correction_uuid=next(MurfeyID),
             )
             environment.movie_tilt_pair[file_transferred_to] = tilt_series
             if environment.tilt_angles.get(tilt_series):
                 environment.tilt_angles[tilt_series].append(
@@ -609,14 +658,17 @@
                                 ],
                                 "image_size_x": environment.data_collection_parameters[
                                     "image_size_x"
                                 ],
                                 "image_size_y": environment.data_collection_parameters[
                                     "image_size_y"
                                 ],
+                                "magnification": environment.data_collection_parameters[
+                                    "magnification"
+                                ],
                             }
                         )
                     if (
                         environment.data_collection_group_ids.get(str(self._basepath))
                         is None
                     ):
                         self._data_collection_stash.append((url, environment, data))
@@ -726,102 +778,108 @@
             last_tilt_angle = extract_tilt_angle(self._last_transferred_file)
             self._last_transferred_file = file_path
             if (
                 last_tilt_series != tilt_series
                 and last_tilt_angle != tilt_angle
                 or self._tilt_series_sizes.get(tilt_series)
             ) or self._completed_tilt_series:
-                newly_completed_series = []
-                if self._tilt_series:
-                    tilt_series_size = max(len(ts) for ts in self._tilt_series.values())
-                else:
-                    tilt_series_size = 0
-                this_tilt_series_size = len(self._tilt_series[tilt_series])
-                tilt_series_size_check = (
-                    (this_tilt_series_size == self._tilt_series_sizes.get(tilt_series))
-                    if self._tilt_series_sizes.get(tilt_series)
-                    else (this_tilt_series_size >= tilt_series_size)
+                return self._check_tilt_series(
+                    tilt_series,
+                    required_position_files or [],
+                    file_transferred_to,
+                    environment=environment,
                 )
-                if tilt_series_size_check and not required_position_files:
-                    self._completed_tilt_series.append(tilt_series)
-                    newly_completed_series.append(tilt_series)
-                for ts, ta in self._tilt_series.items():
-                    if self._tilt_series_sizes.get(ts):
-                        completion_test = len(ta) == self._tilt_series_sizes[ts]
-                    elif required_position_files:
-                        completion_test = all(
-                            _f.is_file() for _f in required_position_files
-                        )
-                    else:
-                        completion_test = len(ta) >= tilt_series_size
-                    if ts not in self._completed_tilt_series and completion_test:
-                        newly_completed_series.append(ts)
-                        self._completed_tilt_series.append(ts)
-                        if environment:
-                            file_tilt_list = []
-                            movie: str
-                            angle: str
-                            for movie, angle in environment.tilt_angles[ts]:
-                                if environment.motion_corrected_movies.get(Path(movie)):
-                                    file_tilt_list.append(
-                                        [
-                                            str(
-                                                environment.motion_corrected_movies[
-                                                    Path(movie)
-                                                ][0]
-                                            ),
-                                            angle,
-                                            str(
-                                                environment.motion_corrected_movies[
-                                                    Path(movie)
-                                                ][1]
-                                            ),
-                                        ]
-                                    )
-                                if environment.motion_corrected_movies.get(
-                                    file_transferred_to
-                                ):
-                                    self._check_for_alignment(
-                                        file_transferred_to,
-                                        Path(
-                                            environment.motion_corrected_movies[  # key error PosixPath
-                                                file_transferred_to
-                                            ][
-                                                0
-                                            ]
-                                        ),
-                                        environment.url.geturl(),
-                                        environment.data_collection_ids[ts],
-                                        environment.processing_job_ids[ts][
-                                            "em-tomo-align"
-                                        ],
-                                        environment.autoproc_program_ids[ts][
-                                            "em-tomo-align"
-                                        ],
-                                        int(
-                                            environment.motion_corrected_movies[
-                                                file_transferred_to
-                                            ][1]
-                                        ),
-                                        file_tilt_list,
-                                        environment.data_collection_parameters.get(
-                                            "manual_tilt_offset"
-                                        ),
-                                        environment.data_collection_parameters.get(
-                                            "pixel_size_on_image"
-                                        ),
-                                    )
-                if newly_completed_series:
-                    logger.info(
-                        f"The following tilt series are considered complete: {newly_completed_series}"
-                    )
-                return newly_completed_series
         self._last_transferred_file = file_path
         return []
 
+    def _check_tilt_series(
+        self,
+        tilt_series: str,
+        required_position_files: List[Path],
+        file_transferred_to: Path | None,
+        environment: MurfeyInstanceEnvironment | None = None,
+    ):
+        newly_completed_series = []
+        if self._tilt_series:
+            tilt_series_size = max(len(ts) for ts in self._tilt_series.values())
+        else:
+            tilt_series_size = 0
+        this_tilt_series_size = len(self._tilt_series[tilt_series])
+        tilt_series_size_check = (
+            (this_tilt_series_size == self._tilt_series_sizes.get(tilt_series))
+            if self._tilt_series_sizes.get(tilt_series)
+            else (this_tilt_series_size >= tilt_series_size)
+        )
+        if tilt_series_size_check and not required_position_files:
+            self._completed_tilt_series.append(tilt_series)
+            newly_completed_series.append(tilt_series)
+        for ts, ta in self._tilt_series.items():
+            if self._tilt_series_sizes.get(ts):
+                completion_test = len(ta) >= self._tilt_series_sizes[ts]
+            elif required_position_files:
+                completion_test = all(_f.is_file() for _f in required_position_files)
+            else:
+                completion_test = len(ta) >= tilt_series_size
+            if ts not in self._completed_tilt_series and completion_test:
+                newly_completed_series.append(ts)
+                self._completed_tilt_series.append(ts)
+                if environment and file_transferred_to:
+                    file_tilt_list = []
+                    movie: str
+                    angle: str
+                    for movie, angle in environment.tilt_angles[ts]:
+                        if environment.motion_corrected_movies.get(Path(movie)):
+                            file_tilt_list.append(
+                                [
+                                    str(
+                                        environment.motion_corrected_movies[
+                                            Path(movie)
+                                        ][0]
+                                    ),
+                                    angle,
+                                    str(
+                                        environment.motion_corrected_movies[
+                                            Path(movie)
+                                        ][1]
+                                    ),
+                                ]
+                            )
+                        if environment.motion_corrected_movies.get(file_transferred_to):
+                            self._check_for_alignment(
+                                file_transferred_to,
+                                Path(
+                                    environment.motion_corrected_movies[  # key error PosixPath
+                                        file_transferred_to
+                                    ][
+                                        0
+                                    ]
+                                ),
+                                environment.url.geturl(),
+                                environment.data_collection_ids[ts],
+                                environment.processing_job_ids[ts]["em-tomo-align"],
+                                environment.autoproc_program_ids[ts]["em-tomo-align"],
+                                int(
+                                    environment.motion_corrected_movies[
+                                        file_transferred_to
+                                    ][1]
+                                ),
+                                file_tilt_list,
+                                environment.data_collection_parameters.get(
+                                    "manual_tilt_offset"
+                                ),
+                                environment.data_collection_parameters.get(
+                                    "pixel_size_on_image"
+                                ),
+                            )
+        if newly_completed_series:
+            logger.info(
+                f"The following tilt series are considered complete: {newly_completed_series}"
+            )
+        return newly_completed_series
+
     def _add_tomo_tilt(
         self,
         file_path: Path,
         environment: MurfeyInstanceEnvironment | None = None,
         required_position_files: List[Path] | None = None,
         required_strings: List[str] | None = None,
     ) -> List[str]:
@@ -918,14 +976,25 @@
                     completed_tilts = self._add_serialem_tilt(
                         transferred_file, environment=environment
                     )
             if transferred_file.suffix == ".mdoc":
                 with open(transferred_file, "r") as md:
                     tilt_series = transferred_file.stem
                     self._tilt_series_sizes[tilt_series] = get_num_blocks(md)
+                if environment:
+                    source = self._get_source(transferred_file, environment)
+                    if source:
+                        completed_tilts = self._check_tilt_series(
+                            tilt_series,
+                            kwargs.get("required_position_files") or [],
+                            self._file_transferred_to(
+                                environment, source, transferred_file
+                            ),
+                            environment=environment,
+                        )
         return completed_tilts
 
     def post_first_transfer(
         self,
         transferred_file: Path,
         role: str = "",
         environment: MurfeyInstanceEnvironment | None = None,
```

### Comparing `murfey-0.7.8/src/murfey/client/contexts/tomo.py` & `murfey-0.7.9/src/murfey/client/contexts/tomo.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/customlogging.py` & `murfey-0.7.9/src/murfey/client/customlogging.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/gain_ref.py` & `murfey-0.7.9/src/murfey/client/gain_ref.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/instance_environment.py` & `murfey-0.7.9/src/murfey/client/instance_environment.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/rsync.py` & `murfey-0.7.9/src/murfey/client/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/tui/app.py` & `murfey-0.7.9/src/murfey/client/tui/app.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/tui/controller.css` & `murfey-0.7.9/src/murfey/client/tui/controller.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/tui/progress.py` & `murfey-0.7.9/src/murfey/client/tui/progress.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/tui/screens.py` & `murfey-0.7.9/src/murfey/client/tui/screens.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/tui/status_bar.py` & `murfey-0.7.9/src/murfey/client/tui/status_bar.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/update.py` & `murfey-0.7.9/src/murfey/client/update.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/watchdir.py` & `murfey-0.7.9/src/murfey/client/watchdir.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/watchdir_multigrid.py` & `murfey-0.7.9/src/murfey/client/watchdir_multigrid.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/client/websocket.py` & `murfey-0.7.9/src/murfey/client/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/__init__.py` & `murfey-0.7.9/src/murfey/server/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/api.py` & `murfey-0.7.9/src/murfey/server/api.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/bootstrap.py` & `murfey-0.7.9/src/murfey/server/bootstrap.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/config.py` & `murfey-0.7.9/src/murfey/server/config.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/demo_api.py` & `murfey-0.7.9/src/murfey/server/demo_api.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/gain.py` & `murfey-0.7.9/src/murfey/server/gain.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/ispyb.py` & `murfey-0.7.9/src/murfey/server/ispyb.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/main.py` & `murfey-0.7.9/src/murfey/server/main.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/server/websocket.py` & `murfey-0.7.9/src/murfey/server/websocket.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/activevisits.html` & `murfey-0.7.9/src/murfey/templates/activevisits.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/base.html` & `murfey-0.7.9/src/murfey/templates/base.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/bootstrap.html` & `murfey-0.7.9/src/murfey/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/images/diamond.png` & `murfey-0.7.9/src/murfey/templates/images/diamond.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/images/icon_268.png` & `murfey-0.7.9/src/murfey/templates/images/icon_268.png`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/static/styles.css` & `murfey-0.7.9/src/murfey/templates/static/styles.css`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/templates/visit.html` & `murfey-0.7.9/src/murfey/templates/visit.html`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/__init__.py` & `murfey-0.7.9/src/murfey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/dummy_setup.py` & `murfey-0.7.9/src/murfey/util/dummy_setup.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/file_monitor.py` & `murfey-0.7.9/src/murfey/util/file_monitor.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/mdoc.py` & `murfey-0.7.9/src/murfey/util/mdoc.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/models.py` & `murfey-0.7.9/src/murfey/util/models.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/rsync.py` & `murfey-0.7.9/src/murfey/util/rsync.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey/util/state.py` & `murfey-0.7.9/src/murfey/util/state.py`

 * *Files identical despite different names*

### Comparing `murfey-0.7.8/src/murfey.egg-info/PKG-INFO` & `murfey-0.7.9/src/murfey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: murfey
-Version: 0.7.8
+Version: 0.7.9
 Summary: Client-Server architecture hauling Cryo-EM data
 License: BSD
 Project-URL: Bug-Tracker, https://github.com/DiamondLightSource/python-murfey/issues
 Project-URL: Documentation, https://github.com/DiamondLightSource/python-murfey
 Project-URL: GitHub, https://github.com/DiamondLightSource/python-murfey
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `murfey-0.7.8/src/murfey.egg-info/SOURCES.txt` & `murfey-0.7.9/src/murfey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

