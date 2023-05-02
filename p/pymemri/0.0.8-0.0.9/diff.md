# Comparing `tmp/pymemri-0.0.8.tar.gz` & `tmp/pymemri-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymemri-0.0.8.tar", last modified: Mon Dec 13 13:22:50 2021, max compression
+gzip compressed data, was "dist/pymemri-0.0.9.tar", last modified: Wed Jan 19 11:28:22 2022, max compression
```

## Comparing `pymemri-0.0.8.tar` & `pymemri-0.0.9.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/
--rw-r--r--   0 koen       (501) staff       (20)      258 2021-12-13 13:07:36.000000 pymemri-0.0.8/MANIFEST.in
--rw-r--r--   0 koen       (501) staff       (20)     5331 2021-12-13 13:22:50.000000 pymemri-0.0.8/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)     4008 2021-12-13 13:22:19.000000 pymemri-0.0.8/README.md
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/
--rw-r--r--   0 koen       (501) staff       (20)       22 2021-12-13 13:22:46.000000 pymemri-0.0.8/pymemri/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     5063 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/_nbdev.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/client_simulator/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/client_simulator/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1765 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/client_simulator/password_simulator.py
--rw-r--r--   0 koen       (501) staff       (20)     8255 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/client_simulator/qr_server.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/client_simulator/template/
--rw-r--r--   0 koen       (501) staff       (20)      105 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/client_simulator/template/images.html
--rw-r--r--   0 koen       (501) staff       (20)      168 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/client_simulator/template/success.html
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/cvu/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/cvu/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/cvu/definitions/
--rw-r--r--   0 koen       (501) staff       (20)     1354 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/cvu/definitions/password_auth.cvu
--rw-r--r--   0 koen       (501) staff       (20)     1210 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/cvu/definitions/qr_code_auth.cvu
--rw-r--r--   0 koen       (501) staff       (20)     2329 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/cvu/definitions/request_email.cvu
--rw-r--r--   0 koen       (501) staff       (20)      922 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/cvu/utils.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/data/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.8/pymemri/data/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     1306 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/data/basic.py
--rw-r--r--   0 koen       (501) staff       (20)    35835 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/data/central_schema.py
--rw-r--r--   0 koen       (501) staff       (20)    11598 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/data/itembase.py
--rw-r--r--   0 koen       (501) staff       (20)     4016 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/data/photo.py
--rw-r--r--   0 koen       (501) staff       (20)     2976 2021-12-13 13:19:18.000000 pymemri-0.0.8/pymemri/data/schema.py
--rw-r--r--   0 koen       (501) staff       (20)      197 2021-08-27 13:29:24.000000 pymemri-0.0.8/pymemri/imports.py
--rw-r--r--   0 koen       (501) staff       (20)      259 2021-08-27 13:29:24.000000 pymemri-0.0.8/pymemri/integrator_registry.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/plugin/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.8/pymemri/plugin/__init__.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/plugin/authenticators/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/plugin/authenticators/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)      532 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/authenticators/credentials.py
--rw-r--r--   0 koen       (501) staff       (20)     3437 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/authenticators/oauth.py
--rw-r--r--   0 koen       (501) staff       (20)     5558 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/authenticators/password.py
--rw-r--r--   0 koen       (501) staff       (20)     1837 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/listeners.py
--rw-r--r--   0 koen       (501) staff       (20)    12061 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/pluginbase.py
--rw-r--r--   0 koen       (501) staff       (20)      201 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/plugin/schema.py
--rw-r--r--   0 koen       (501) staff       (20)     7703 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/plugin/stateful.py
--rw-r--r--   0 koen       (501) staff       (20)      568 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/plugin/states.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/pod/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.8/pymemri/pod/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     6835 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/pod/api.py
--rw-r--r--   0 koen       (501) staff       (20)    17160 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/pod/client.py
--rw-r--r--   0 koen       (501) staff       (20)      934 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/pod/db.py
--rw-r--r--   0 koen       (501) staff       (20)      934 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/pod/utils.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri/template/
--rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.8/pymemri/template/__init__.py
--rw-r--r--   0 koen       (501) staff       (20)     2715 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/template/config.py
--rw-r--r--   0 koen       (501) staff       (20)     4787 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/template/formatter.py
--rw-r--r--   0 koen       (501) staff       (20)      365 2021-12-13 13:22:22.000000 pymemri-0.0.8/pymemri/test_utils.py
-drwxr-xr-x   0 koen       (501) staff       (20)        0 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/
--rw-r--r--   0 koen       (501) staff       (20)     5331 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/PKG-INFO
--rw-r--r--   0 koen       (501) staff       (20)     1423 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/SOURCES.txt
--rw-r--r--   0 koen       (501) staff       (20)        1 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/dependency_links.txt
--rw-r--r--   0 koen       (501) staff       (20)      519 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/entry_points.txt
--rw-r--r--   0 koen       (501) staff       (20)        1 2021-08-27 13:34:39.000000 pymemri-0.0.8/pymemri.egg-info/not-zip-safe
--rw-r--r--   0 koen       (501) staff       (20)      162 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/requires.txt
--rw-r--r--   0 koen       (501) staff       (20)        8 2021-12-13 13:22:50.000000 pymemri-0.0.8/pymemri.egg-info/top_level.txt
--rw-r--r--   0 koen       (501) staff       (20)     1337 2021-12-13 13:19:58.000000 pymemri-0.0.8/settings.ini
--rw-r--r--   0 koen       (501) staff       (20)       38 2021-12-13 13:22:50.000000 pymemri-0.0.8/setup.cfg
--rw-r--r--   0 koen       (501) staff       (20)     1866 2021-08-27 13:29:24.000000 pymemri-0.0.8/setup.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/
+-rw-r--r--   0 koen       (501) staff       (20)      258 2021-12-13 13:07:36.000000 pymemri-0.0.9/MANIFEST.in
+-rw-r--r--   0 koen       (501) staff       (20)     5367 2022-01-19 11:28:22.000000 pymemri-0.0.9/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)     4044 2022-01-19 11:27:57.000000 pymemri-0.0.9/README.md
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/
+-rw-r--r--   0 koen       (501) staff       (20)       22 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     5470 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/_nbdev.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/client_simulator/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/client_simulator/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     1765 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/client_simulator/password_simulator.py
+-rw-r--r--   0 koen       (501) staff       (20)     8255 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/client_simulator/qr_server.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/client_simulator/template/
+-rw-r--r--   0 koen       (501) staff       (20)      105 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/client_simulator/template/images.html
+-rw-r--r--   0 koen       (501) staff       (20)      412 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/client_simulator/template/success.html
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/cvu/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/cvu/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/cvu/definitions/
+-rw-r--r--   0 koen       (501) staff       (20)     1354 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/cvu/definitions/password_auth.cvu
+-rw-r--r--   0 koen       (501) staff       (20)     1210 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/cvu/definitions/qr_code_auth.cvu
+-rw-r--r--   0 koen       (501) staff       (20)     2329 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/cvu/definitions/request_email.cvu
+-rw-r--r--   0 koen       (501) staff       (20)      922 2022-01-13 14:54:17.000000 pymemri-0.0.9/pymemri/cvu/utils.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/data/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.9/pymemri/data/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)    37807 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/_central_schema.py
+-rw-r--r--   0 koen       (501) staff       (20)     1002 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/basic.py
+-rw-r--r--   0 koen       (501) staff       (20)     2192 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/dataset.py
+-rw-r--r--   0 koen       (501) staff       (20)    12558 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/itembase.py
+-rw-r--r--   0 koen       (501) staff       (20)     4856 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/photo.py
+-rw-r--r--   0 koen       (501) staff       (20)     3031 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/data/schema.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/exporters/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/exporters/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     2971 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/exporters/exporters.py
+-rw-r--r--   0 koen       (501) staff       (20)      197 2021-08-27 13:29:24.000000 pymemri-0.0.9/pymemri/imports.py
+-rw-r--r--   0 koen       (501) staff       (20)      259 2021-08-27 13:29:24.000000 pymemri-0.0.9/pymemri/integrator_registry.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/plugin/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.9/pymemri/plugin/__init__.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/plugin/authenticators/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/plugin/authenticators/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)      532 2022-01-13 14:54:17.000000 pymemri-0.0.9/pymemri/plugin/authenticators/credentials.py
+-rw-r--r--   0 koen       (501) staff       (20)     3437 2022-01-13 14:54:17.000000 pymemri-0.0.9/pymemri/plugin/authenticators/oauth.py
+-rw-r--r--   0 koen       (501) staff       (20)     5558 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/plugin/authenticators/password.py
+-rw-r--r--   0 koen       (501) staff       (20)     1837 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/plugin/listeners.py
+-rw-r--r--   0 koen       (501) staff       (20)    12061 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/plugin/pluginbase.py
+-rw-r--r--   0 koen       (501) staff       (20)      201 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/plugin/schema.py
+-rw-r--r--   0 koen       (501) staff       (20)     7703 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/plugin/stateful.py
+-rw-r--r--   0 koen       (501) staff       (20)      568 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/plugin/states.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/pod/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-08-27 13:29:24.000000 pymemri-0.0.9/pymemri/pod/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     6841 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/pod/api.py
+-rw-r--r--   0 koen       (501) staff       (20)    18082 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/pod/client.py
+-rw-r--r--   0 koen       (501) staff       (20)      934 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/pod/db.py
+-rw-r--r--   0 koen       (501) staff       (20)      934 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/pod/utils.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri/template/
+-rw-r--r--   0 koen       (501) staff       (20)        0 2021-12-13 13:07:36.000000 pymemri-0.0.9/pymemri/template/__init__.py
+-rw-r--r--   0 koen       (501) staff       (20)     2715 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/template/config.py
+-rw-r--r--   0 koen       (501) staff       (20)     6223 2022-01-19 11:27:57.000000 pymemri-0.0.9/pymemri/template/formatter.py
+-rw-r--r--   0 koen       (501) staff       (20)      365 2022-01-13 14:54:18.000000 pymemri-0.0.9/pymemri/test_utils.py
+drwxr-xr-x   0 koen       (501) staff       (20)        0 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/
+-rw-r--r--   0 koen       (501) staff       (20)     5367 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/PKG-INFO
+-rw-r--r--   0 koen       (501) staff       (20)     1509 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/SOURCES.txt
+-rw-r--r--   0 koen       (501) staff       (20)        1 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/dependency_links.txt
+-rw-r--r--   0 koen       (501) staff       (20)      519 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/entry_points.txt
+-rw-r--r--   0 koen       (501) staff       (20)        1 2021-08-27 13:34:39.000000 pymemri-0.0.9/pymemri.egg-info/not-zip-safe
+-rw-r--r--   0 koen       (501) staff       (20)      155 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/requires.txt
+-rw-r--r--   0 koen       (501) staff       (20)        8 2022-01-19 11:28:22.000000 pymemri-0.0.9/pymemri.egg-info/top_level.txt
+-rw-r--r--   0 koen       (501) staff       (20)     1330 2022-01-19 11:27:57.000000 pymemri-0.0.9/settings.ini
+-rw-r--r--   0 koen       (501) staff       (20)       38 2022-01-19 11:28:22.000000 pymemri-0.0.9/setup.cfg
+-rw-r--r--   0 koen       (501) staff       (20)     1866 2021-08-27 13:29:24.000000 pymemri-0.0.9/setup.py
```

### Comparing `pymemri-0.0.8/PKG-INFO` & `pymemri-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pymemri
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the memri data
 Home-page: https://gitlab.memri.io/memri/pymemri/tree/prod/
 Author: Koen van der Veen
 Author-email: koen.vanderveen@polis.global
 License: Apache Software License 2.0
 Description: # Pymemri
         > Pymemri is a python library for creating <b>Plugins</b> for the Memri Personal online datastore <a href='https://gitlab.memri.io/memri/pod'>(pod)</a>. Pymemri has a PodClient to communicate with the pod, and tools to build and test plugins.
         
         
         [![Gitlab pipeline status (self-hosted)](https://img.shields.io/gitlab/pipeline/memri/pymemri/dev?gitlab_url=https%3A%2F%2Fgitlab.memri.io&label=CI&logo=gitlab&style=plastic)](https://gitlab.memri.io/memri/pymemri/-/pipelines/latest)
         [![Discord](https://img.shields.io/discord/799216875480678430?color=blue&label=Discord&logo=discord&style=plastic)](https://discord.gg/BcRfajJk4k)
         [![Twitter URL](https://img.shields.io/twitter/url?label=%40YourMemri&logo=twitter&style=plastic&url=https%3A%2F%2Ftwitter.com%2FYourMemri)](https://twitter.com/YourMemri)
+        <a href="https://pypi.org/project/pymemri/"><img src="https://pepy.tech/badge/pymemri" /></a>
         
         Plugins connect and add the information to your Pod. Plugins that <b>import your data from external services</b> are called **Importers** (Gmail, WhatsApp, etc.). Plugins that <b>connect new data to the existing data</b> are called  **indexers** (face recognition, spam detection, object detection, etc.). Lastly there are plugins that <b>execute actions</b> (sending messages, uploading files). This repository is built with [nbdev](https://github.com/fastai/nbdev), which means that the repo structure has a few differences compared to a standard python repo. 
         
         ## Installing
         
         ### As a package
         ```bash
@@ -68,16 +69,15 @@
         run_plugin --metadata "example_plugin.json"
         ```
         
         This stores a random owner key and database key on your disk for future use, and runs the pymemri example plugin. If everything works correctly, the output should read `Plugin run success.`
         
         ## Docs
         
-        - [pymemri docs](http://memri.docs.memri.io/pymemri/pod.client.html#File-API)
-        - [plugin tutorial](https://blog.memri.io/getting-started-building-a-plugin/)
+        [pymemri docs](https://memri.docs.memri.io/docs.memri.io/component-architectures/plugins/readme/)
         
         ## Nbdev & Jupyter Notebooks
         The Python integrators are written in [nbdev](https://nbdev.fast.ai/) ([video](https://www.youtube.com/watch?v=9Q6sLbz37gk&t=1301s)). With nbdev, it is encouraged to write code in 
         [Jupyter Notebooks](https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html). Nbdev syncs all the notebooks in `/nbs` with the python code in `/pymemri`. Tests are written side by side with the code in the notebooks, and documentation is automatically generated from the code and markdown in the notebooks and exported into the `/docs` folder. Check out the [nbdev quickstart](wiki/nbdev_quickstart.md) for an introduction, **watch the video linked above**, or see the [nbdev documentation](https://nbdev.fast.ai/) for a all functionalities and tutorials.
         
 Keywords: memri privacy personal data client python
 Platform: UNKNOWN
```

### Comparing `pymemri-0.0.8/README.md` & `pymemri-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Pymemri
 > Pymemri is a python library for creating <b>Plugins</b> for the Memri Personal online datastore <a href='https://gitlab.memri.io/memri/pod'>(pod)</a>. Pymemri has a PodClient to communicate with the pod, and tools to build and test plugins.
 
 
 [![Gitlab pipeline status (self-hosted)](https://img.shields.io/gitlab/pipeline/memri/pymemri/dev?gitlab_url=https%3A%2F%2Fgitlab.memri.io&label=CI&logo=gitlab&style=plastic)](https://gitlab.memri.io/memri/pymemri/-/pipelines/latest)
 [![Discord](https://img.shields.io/discord/799216875480678430?color=blue&label=Discord&logo=discord&style=plastic)](https://discord.gg/BcRfajJk4k)
 [![Twitter URL](https://img.shields.io/twitter/url?label=%40YourMemri&logo=twitter&style=plastic&url=https%3A%2F%2Ftwitter.com%2FYourMemri)](https://twitter.com/YourMemri)
+<a href="https://pypi.org/project/pymemri/"><img src="https://pepy.tech/badge/pymemri" /></a>
 
 Plugins connect and add the information to your Pod. Plugins that <b>import your data from external services</b> are called **Importers** (Gmail, WhatsApp, etc.). Plugins that <b>connect new data to the existing data</b> are called  **indexers** (face recognition, spam detection, object detection, etc.). Lastly there are plugins that <b>execute actions</b> (sending messages, uploading files). This repository is built with [nbdev](https://github.com/fastai/nbdev), which means that the repo structure has a few differences compared to a standard python repo. 
 
 ## Installing
 
 ### As a package
 ```bash
@@ -60,13 +61,12 @@
 run_plugin --metadata "example_plugin.json"
 ```
 
 This stores a random owner key and database key on your disk for future use, and runs the pymemri example plugin. If everything works correctly, the output should read `Plugin run success.`
 
 ## Docs
 
-- [pymemri docs](http://memri.docs.memri.io/pymemri/pod.client.html#File-API)
-- [plugin tutorial](https://blog.memri.io/getting-started-building-a-plugin/)
+[pymemri docs](https://memri.docs.memri.io/docs.memri.io/component-architectures/plugins/readme/)
 
 ## Nbdev & Jupyter Notebooks
 The Python integrators are written in [nbdev](https://nbdev.fast.ai/) ([video](https://www.youtube.com/watch?v=9Q6sLbz37gk&t=1301s)). With nbdev, it is encouraged to write code in 
 [Jupyter Notebooks](https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html). Nbdev syncs all the notebooks in `/nbs` with the python code in `/pymemri`. Tests are written side by side with the code in the notebooks, and documentation is automatically generated from the code and markdown in the notebooks and exported into the `/docs` folder. Check out the [nbdev quickstart](wiki/nbdev_quickstart.md) for an introduction, **watch the video linked above**, or see the [nbdev documentation](https://nbdev.fast.ai/) for a all functionalities and tutorials.
```

### Comparing `pymemri-0.0.8/pymemri/_nbdev.py` & `pymemri-0.0.9/pymemri/_nbdev.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 __all__ = ["index", "modules", "custom_doc_links", "git_url"]
 
 index = {"read_file": "basic.ipynb",
          "read_json": "basic.ipynb",
          "write_json": "basic.ipynb",
          "unzip": "basic.ipynb",
-         "resize": "data.photo.ipynb",
-         "get_size": "data.photo.ipynb",
          "Path.ls": "basic.ipynb",
          "PYI_HOME": "basic.ipynb",
          "PYI_TESTDATA": "basic.ipynb",
          "HOME_DIR": "basic.ipynb",
          "MODEL_DIR": "basic.ipynb",
          "MEMRI_S3": "basic.ipynb",
          "CVU_BASE_PATH": "cvu.utils.ipynb",
          "get_default_cvu": "cvu.utils.ipynb",
          "list_default_cvus": "cvu.utils.ipynb",
+         "filter_rows": "data.dataset.ipynb",
+         "Dataset": "data.dataset.ipynb",
+         "DEFAULT_ENCODING": "data.photo.ipynb",
          "show_images": "data.photo.ipynb",
-         "get_height_width_channels": "data.photo.ipynb",
          "Photo": "data.photo.ipynb",
+         "Query": "exporters.exporters.ipynb",
          "ALL_EDGES": "itembase.ipynb",
          "Edge": "itembase.ipynb",
          "ItemBase": "itembase.ipynb",
          "Item": "itembase.ipynb",
          "PLUGIN_DIR": "plugin.authenticators.credentials.ipynb",
          "read_username_password": "plugin.authenticators.credentials.ipynb",
          "OAuthAuthenticator": "plugin.authenticators.oauth.ipynb",
@@ -76,24 +77,31 @@
          "get_params": "template.config.ipynb",
          "identifier_to_displayname": "template.config.ipynb",
          "get_param_config": "template.config.ipynb",
          "create_config": "template.config.ipynb",
          "create_plugin_config": "template.config.ipynb",
          "TEMPLATE_URL": "template.formatter.ipynb",
          "TEMPLATE_BASE_PATH": "template.formatter.ipynb",
+         "get_remote_url": "template.formatter.ipynb",
+         "infer_git_info": "template.formatter.ipynb",
+         "GITLAB_GROUPS": "template.formatter.ipynb",
          "str_to_identifier": "template.formatter.ipynb",
+         "reponame_to_displayname": "template.formatter.ipynb",
          "download_plugin_template": "template.formatter.ipynb",
          "get_templates": "template.formatter.ipynb",
          "TemplateFormatter": "template.formatter.ipynb",
+         "get_template_replace_dict": "template.formatter.ipynb",
          "plugin_from_template": "template.formatter.ipynb",
          "get_ci_variables": "test_utils.ipynb"}
 
 modules = ["data/basic.py",
            "cvu/utils.py",
+           "data/dataset.py",
            "data/photo.py",
+           "exporters/exporters.py",
            "data/itembase.py",
            "plugin/authenticators/credentials.py",
            "plugin/authenticators/oauth.py",
            "plugin/listeners.py",
            "plugin/pluginbase.py",
            "plugin/states.py",
            "plugin/authenticators/password.py",
```

### Comparing `pymemri-0.0.8/pymemri/client_simulator/password_simulator.py` & `pymemri-0.0.9/pymemri/client_simulator/password_simulator.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/client_simulator/qr_server.py` & `pymemri-0.0.9/pymemri/client_simulator/qr_server.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/cvu/definitions/password_auth.cvu` & `pymemri-0.0.9/pymemri/cvu/definitions/password_auth.cvu`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/cvu/definitions/qr_code_auth.cvu` & `pymemri-0.0.9/pymemri/cvu/definitions/qr_code_auth.cvu`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/cvu/definitions/request_email.cvu` & `pymemri-0.0.9/pymemri/cvu/definitions/request_email.cvu`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/cvu/utils.py` & `pymemri-0.0.9/pymemri/cvu/utils.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/data/central_schema.py` & `pymemri-0.0.9/pymemri/data/_central_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "changelog",
         "cryptoTransaction",
         "location",
         "network",
         "ownCurrency",
         "owner",
         "trust",
+        "profilePicture",
     ]
 
     def __init__(
         self,
         avatarUrl: str = None,
         authEmail: str = None,
         code: str = None,
@@ -53,14 +54,15 @@
         changelog: list = None,
         cryptoTransaction: list = None,
         location: list = None,
         network: list = None,
         ownCurrency: list = None,
         owner: list = None,
         trust: list = None,
+        profilePicture: list = None,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         # Properties
         self.avatarUrl: Optional[str] = avatarUrl
         self.authEmail: Optional[str] = authEmail
@@ -74,20 +76,23 @@
         self.secret: Optional[str] = secret
         self.service: Optional[str] = service
         self.accessToken: Optional[str] = accessToken
         self.refreshToken: Optional[str] = refreshToken
 
         # Edges
         self.changelog: list = changelog if changelog is not None else []
-        self.cryptoTransaction: list = cryptoTransaction if cryptoTransaction is not None else []
+        self.cryptoTransaction: list = (
+            cryptoTransaction if cryptoTransaction is not None else []
+        )
         self.location: list = location if location is not None else []
         self.network: list = network if network is not None else []
         self.ownCurrency: list = ownCurrency if ownCurrency is not None else []
         self.owner: list = owner if owner is not None else []
         self.trust: list = trust if trust is not None else []
+        self.profilePicture: list = profilePicture if profilePicture is not None else []
 
 
 class AuditItem(Item):
     description = """TBD"""
     properties = Item.properties + ["actionname", "content", "date"]
     edges = Item.edges + []
 
@@ -110,37 +115,43 @@
     description = """TBD"""
     properties = Item.properties + [
         "definition",
         "domain",
         "itemType",
         "name",
         "querystr",
+        "renderer",
         "selector",
+        "type",
     ]
     edges = Item.edges + []
 
     def __init__(
         self,
         definition: str = None,
         domain: str = None,
         itemType: str = None,
         name: str = None,
         querystr: str = None,
+        renderer: str = None,
         selector: str = None,
+        type: str = None,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         # Properties
         self.definition: Optional[str] = definition
         self.domain: Optional[str] = domain
         self.itemType: Optional[str] = itemType
         self.name: Optional[str] = name
         self.querystr: Optional[str] = querystr
+        self.renderer: Optional[str] = renderer
         self.selector: Optional[str] = selector
+        self.type: Optional[str] = type
 
 
 class CreativeWork(Item):
     description = """The most generic kind of creative work, including books, movies, photographs, software programs, etc."""
     properties = Item.properties + [
         "abstract",
         "content",
@@ -178,17 +189,21 @@
         self.itemType: Optional[str] = itemType
         self.keyword: Optional[str] = keyword
         self.textContent: Optional[str] = textContent
         self.title: Optional[str] = title
         self.transcript: Optional[str] = transcript
 
         # Edges
-        self.contentLocation: list = contentLocation if contentLocation is not None else []
+        self.contentLocation: list = (
+            contentLocation if contentLocation is not None else []
+        )
         self.file: list = file if file is not None else []
-        self.locationCreated: list = locationCreated if locationCreated is not None else []
+        self.locationCreated: list = (
+            locationCreated if locationCreated is not None else []
+        )
         self.writtenBy: list = writtenBy if writtenBy is not None else []
 
 
 class CryptoCurrency(Item):
     description = """"""
     properties = Item.properties + ["myToken", "name", "topic"]
     edges = Item.edges + ["currencySetting", "picture"]
@@ -206,15 +221,17 @@
 
         # Properties
         self.myToken: Optional[float] = myToken
         self.name: Optional[str] = name
         self.topic: Optional[str] = topic
 
         # Edges
-        self.currencySetting: list = currencySetting if currencySetting is not None else []
+        self.currencySetting: list = (
+            currencySetting if currencySetting is not None else []
+        )
         self.picture: list = picture if picture is not None else []
 
 
 class CryptoKey(Item):
     description = """A key used in an cryptography protocol."""
     properties = Item.properties + [
         "active",
@@ -304,14 +321,27 @@
         self.seedPhrase: Optional[str] = seedPhrase
         self.tokenAddress: Optional[str] = tokenAddress
 
         # Edges
         self.wallet: list = wallet if wallet is not None else []
 
 
+class Dataset(Item):
+    description = """A Dataset of items."""
+    properties = Item.properties + ["name", "querystr"]
+    edges = Item.edges + []
+
+    def __init__(self, name: str = None, querystr: str = None, **kwargs):
+        super().__init__(**kwargs)
+
+        # Properties
+        self.name: Optional[str] = name
+        self.querystr: Optional[str] = querystr
+
+
 class Diet(Item):
     description = """A strategy of regulating the intake of food to achieve or maintain a specific health-related goal."""
     properties = Item.properties + [
         "abstract",
         "content",
         "datePublished",
         "duration",
@@ -353,40 +383,46 @@
         self.keyword: Optional[str] = keyword
         self.name: Optional[str] = name
         self.textContent: Optional[str] = textContent
         self.title: Optional[str] = title
         self.transcript: Optional[str] = transcript
 
         # Edges
-        self.contentLocation: list = contentLocation if contentLocation is not None else []
+        self.contentLocation: list = (
+            contentLocation if contentLocation is not None else []
+        )
         self.file: list = file if file is not None else []
-        self.locationCreated: list = locationCreated if locationCreated is not None else []
+        self.locationCreated: list = (
+            locationCreated if locationCreated is not None else []
+        )
         self.writtenBy: list = writtenBy if writtenBy is not None else []
 
 
 class File(Item):
     description = """Any file that can be stored on disk."""
-    properties = Item.properties + ["filename", "keystr", "nonce", "sha256"]
+    properties = Item.properties + ["filename", "keystr", "nonce", "sha256", "starred"]
     edges = Item.edges + []
 
     def __init__(
         self,
         filename: str = None,
         keystr: str = None,
         nonce: str = None,
         sha256: str = None,
+        starred: bool = None,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         # Properties
         self.filename: Optional[str] = filename
         self.keystr: Optional[str] = keystr
         self.nonce: Optional[str] = nonce
         self.sha256: Optional[str] = sha256
+        self.starred: Optional[bool] = starred
 
 
 class Integrator(Item):
     description = """An integrator operates on your database enhances your personal data by inferring facts over existing data and adding those to the database."""
     properties = Item.properties + ["name", "repository"]
     edges = Item.edges + []
 
@@ -469,14 +505,56 @@
         self.allowSharing: Optional[bool] = allowSharing
         self.labels: Optional[str] = labels
 
         # Edges
         self.annotatedItem: list = annotatedItem if annotatedItem is not None else []
 
 
+class LabelingDataType(Item):
+    description = """A labelling data type definition."""
+    properties = Item.properties + ["name", "icon"]
+    edges = Item.edges + ["dataset"]
+
+    def __init__(
+        self, name: str = None, icon: str = None, dataset: list = None, **kwargs
+    ):
+        super().__init__(**kwargs)
+
+        # Properties
+        self.name: Optional[str] = name
+        self.icon: Optional[str] = icon
+
+        # Edges
+        self.dataset: list = dataset if dataset is not None else []
+
+
+class LabelingTask(Item):
+    description = """A labelling task definition."""
+    properties = Item.properties + ["name"]
+    edges = Item.edges + ["labelOption", "dataset", "view"]
+
+    def __init__(
+        self,
+        name: str = None,
+        labelOption: list = None,
+        dataset: list = None,
+        view: list = None,
+        **kwargs
+    ):
+        super().__init__(**kwargs)
+
+        # Properties
+        self.name: Optional[str] = name
+
+        # Edges
+        self.labelOption: list = labelOption if labelOption is not None else []
+        self.dataset: list = dataset if dataset is not None else []
+        self.view: list = view if view is not None else []
+
+
 class Location(Item):
     description = """The location of something."""
     properties = Item.properties + ["latitude", "longitude"]
     edges = Item.edges + []
 
     def __init__(self, latitude: float = None, longitude: float = None, **kwargs):
         super().__init__(**kwargs)
@@ -697,15 +775,17 @@
         self.birthPlace: list = birthPlace if birthPlace is not None else []
         self.cryptoKey: list = cryptoKey if cryptoKey is not None else []
         self.deathPlace: list = deathPlace if deathPlace is not None else []
         self.diet: list = diet if diet is not None else []
         self.hasPhoneNumber: list = hasPhoneNumber if hasPhoneNumber is not None else []
         self.label: list = label if label is not None else []
         self.me: list = me if me is not None else []
-        self.medicalCondition: list = medicalCondition if medicalCondition is not None else []
+        self.medicalCondition: list = (
+            medicalCondition if medicalCondition is not None else []
+        )
         self.mergedFrom: list = mergedFrom if mergedFrom is not None else []
         self.profilePicture: list = profilePicture if profilePicture is not None else []
         self.relationship: list = relationship if relationship is not None else []
         self.website: list = website if website is not None else []
 
 
 class PhoneNumber(Item):
@@ -1146,33 +1226,29 @@
 
         # Edges
         self.label: list = label if label is not None else []
 
 
 class EmailMessage(Message):
     description = """A single email message."""
-    properties = Message.properties + ["starred", "read"]
-    edges = Message.edges + ["bcc", "cc", "message", "replyTo", "inbox"]
+    properties = Message.properties + ["starred"]
+    edges = Message.edges + ["bcc", "cc", "message", "replyTo"]
 
     def __init__(
         self,
         starred: bool = None,
-        read: bool = None,
         bcc: list = None,
         cc: list = None,
         message: list = None,
         replyTo: list = None,
-        inbox: list = None,
         **kwargs
     ):
         super().__init__(**kwargs)
 
         # Properties
         self.starred: Optional[bool] = starred
-        self.read: Optional[bool] = read
 
         # Edges
         self.bcc: list = bcc if bcc is not None else []
         self.cc: list = cc if cc is not None else []
         self.message: list = message if message is not None else []
         self.replyTo: list = replyTo if replyTo is not None else []
-        self.inbox: list = inbox if inbox is not None else []
```

### Comparing `pymemri-0.0.8/pymemri/data/itembase.py` & `pymemri-0.0.9/pymemri/data/itembase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/itembase.ipynb (unless otherwise specified).
 
 __all__ = ['ALL_EDGES', 'Edge', 'ItemBase', 'Item']
 
 # Cell
 # hide
-from typing import Optional, Dict
+from typing import Optional, Dict, List, Set
 from ..imports import *
 from datetime import datetime
 
 ALL_EDGES = "allEdges"
 SOURCE, TARGET, TYPE, EDGE_TYPE, LABEL, SEQUENCE = "_source", "_target", "_type", "_type", "label", "sequence"
 
 # Cell
@@ -61,29 +61,54 @@
 
 # Cell
 # hide
 class ItemBase:
     """Provides a base class for all items.
     All items in the schema inherit from this class, and it provides some
     basic functionality for consistency and to enable easier usage."""
+    properties: List[str] = list()
+    edges: List[str] = list()
 
     def __init__(self, id: str = None):
+        self._updated_properties: Set[str] = set()
+
         self.id: Optional[str] = id
+        self._client: Optional["PodClient"] = None
+        self._in_pod: bool = False
+
+    def _set_client(self, client: "PodClient"):
+        if self._client is not None and self._client != client:
+            raise ValueError(f"Attempted to overwrite existing client of item {self}")
+        self._client = client
+
+    def __setattr__(self, name, value):
+        prev_val = getattr(self, name, None)
+        super(ItemBase, self).__setattr__(name, value)
+        if name in self.properties and value != prev_val:
+            self._updated_properties.add(name)
 
     def __getattribute__(self, name):
         val = object.__getattribute__(self, name)
         if isinstance(val, Edge):
             edge = val
             return edge.traverse(start=self)
         if isinstance(val, list) and len(val) > 0 and isinstance(val[0], Edge):
             edges = val
             return [edge.traverse(start=self) for edge in edges]
         else:
             return val
 
+    def on_sync_to_pod(self, client):
+        """
+        on_sync_to_pod is called when self is created or updated (optionally via bulk) in the PodClient.
+        """
+        self._set_client(client)
+        self._updated_properties = set()
+        self._in_pod = True
+
     def add_edge(self, name, val):
         """Creates an edge of type name and makes it point to val"""
         val = Edge(self, val, name, created=True)
         if name not in self.__dict__:
             raise NameError(f"object {self} does not have edge with name {name}")
         existing = object.__getattribute__(self, name)
         if val not in existing:
```

### Comparing `pymemri-0.0.8/pymemri/data/photo.py` & `pymemri-0.0.9/pymemri/data/photo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/data.photo.ipynb (unless otherwise specified).
 
-__all__ = ['show_images', 'get_size', 'resize', 'get_height_width_channels', 'Photo']
+__all__ = ['DEFAULT_ENCODING', 'show_images', 'Photo']
 
 # Cell
 from .schema import Item
 
 # Cell
 from .schema import *
 from .basic import *
 from matplotlib.pyplot import imshow
 from matplotlib import patches
 from matplotlib.collections import PatchCollection
 from numpy.linalg import norm
 from hashlib import sha256
-import cv2
 import matplotlib.pyplot as plt
 import math
 import numpy as np
 import io
 from PIL import Image
 from hashlib import sha256
 from typing import Any
 
 # Cell
-NUMPY, BYTES = "numpy", "bytes"
+DEFAULT_ENCODING = "PNG"
 
 # Cell
 def show_images(images, cols = 3, titles = None):
     image_list = [x.data for x in images] if isinstance(images[0], Photo) else images
     assert((titles is None) or (len(image_list) == len(titles)))
     n_images = len(image_list)
     if titles is None: titles = ["" for i in range(1,n_images + 1)]
@@ -38,102 +37,125 @@
         if image.ndim == 2:
             plt.gray()
         plt.imshow(image[:,:,::-1])
         a.set_title(title)
     fig.set_size_inches(np.array(fig.get_size_inches()) * n_images)
     plt.show()
 
-def get_size(img, maxsize):
-    s = img.shape
-    assert len(s) > 1
-    div = max(s) / maxsize
-    return (int(s[1]//div), int(s[0]//div))
-
-def resize(img, maxsize):
-    size = get_size(img, maxsize)
-    return cv2.resize(img, dsize=size, interpolation=cv2.INTER_CUBIC)
-
-def get_height_width_channels(img):
-    s = img.shape
-    if len(s) == 2: return s[0], s[1], 1
-    else: return img.shape
-
 # Cell
 class Photo(Item):
 
-    properties = Item.properties + ["width", "height", "channels", "encoding"]
+    properties = Item.properties + ["width", "height", "channels", "encoding", "mode"]
     edges = Item.edges + ["file"]
 
     def __init__(
         self,
         data: Any=None,
-        includes: Any=None,
-        thumbnail: Any=None,
+        includes: Any=None,  # TODO
+        thumbnail: Any=None, # TODO
         height: int=None,
         width: int=None,
         channels: int=None,
         encoding: str=None,
+        mode: str=None,
         file: list=None,
         _file_created: bool=False,
         **kwargs
     ):
         super().__init__(**kwargs)
-        self.private = ["data", "embedding", "path"]
+        self.private = ["data", "embedding", "path"] #TODO
         self.height = height
         self.width = width
         self.channels = channels
         self.encoding = encoding
+        self.mode = mode
         self.file = file if file is not None else []
         self.data = data
         self._file_created = _file_created
 
     def show(self):
         fig, ax = plt.subplots(1)
         fig.set_figheight(15)
         fig.set_figwidth(15)
         ax.axis("off")
         imshow(self.data[:, :, ::-1])
         fig.set_size_inches((6, 6))
         plt.show()
 
+    @property
+    def size(self):
+        return self.width, self.height
+
     @classmethod
     def from_data(cls, *args, **kwargs):
         res = super().from_data(*args, **kwargs)
         if res.file:
-            res.file[0]
+            res.file[0]  # TODO
         return res
 
     @classmethod
     def from_path(cls, path, size=None):
-        data = cv2.imread(str(path))
-        res = cls.from_np(data, size)
+        pil_image = Image.open(path)
+        encoding, mode, shape = cls.infer_PIL_metadata(pil_image)
+        w, h, c = shape
+        _bytes = cls.PIL_to_bytes(pil_image, encoding)
+
+        res = cls(data=_bytes, height=h, width=w, channels=c, encoding=encoding, mode=mode)
+        file = File.from_data(sha256=sha256(_bytes).hexdigest())
+        res.add_edge("file", file)
         return res
 
     @classmethod
     def from_np(cls, data, size=None, *args, **kwargs):
+        pil_image = Image.fromarray(data)
         if size is not None:
-            data = resize(data, size)
-        h, w, c = get_height_width_channels(data)
-        res = cls(
-            data=data, height=h, width=w, channels=c, encoding=NUMPY, *args, **kwargs
-        )
-        file = File.from_data(sha256=sha256(data.tobytes()).hexdigest())
+            pil_image = pil_image.resize(size)
+        encoding, mode, shape = cls.infer_PIL_metadata(pil_image)
+        w, h, c = shape
+        _bytes = cls.PIL_to_bytes(pil_image, encoding)
+
+        res = cls(data=_bytes, height=h, width=w, channels=c, encoding=encoding, mode=mode)
+        file = File.from_data(sha256=sha256(_bytes).hexdigest())
         res.add_edge("file", file)
         return res
 
     @classmethod
     def from_bytes(cls, _bytes):
         image_stream = io.BytesIO(_bytes)
         pil_image = Image.open(image_stream)
+        encoding, mode, shape = cls.infer_PIL_metadata(pil_image)
+        w, h, c = shape
+
+        res = cls(data=_bytes, height=h, width=w, channels=c, encoding=encoding, mode=mode)
+        file = File.from_data(sha256=sha256(_bytes).hexdigest())
+        res.add_edge("file", file)
+        return res
+
+    @staticmethod
+    def PIL_to_bytes(pil_image, encoding):
+        byte_io = io.BytesIO()
+        pil_image.save(byte_io, encoding)
+        return byte_io.getvalue()
+
+    @staticmethod
+    def infer_PIL_metadata(pil_image):
+        encoding = pil_image.format or DEFAULT_ENCODING
+        mode = pil_image.mode
         size = pil_image.size
         if len(size) == 3:
             w, h, c = size
         if len(size) == 2:
             w, h = size
             c = 1
         else:
             raise Error
+        return encoding, mode, (w, h, c)
 
-        res = cls(data=_bytes, height=h, width=w, encoding=BYTES, channels=c)
-        file = File.from_data(sha256=sha256(_bytes).hexdigest())
-        res.add_edge("file", file)
-        return res
+    def to_PIL(self):
+        if self.data is None:
+            raise ValueError("Photo object has no data")
+
+        return Image.open(io.BytesIO(self.data))
+
+    def to_np(self):
+        pil_img = self.to_PIL()
+        return np.asarray(pil_img)
```

### Comparing `pymemri-0.0.8/pymemri/data/schema.py` & `pymemri-0.0.9/pymemri/data/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import random, string
 from .itembase import ItemBase, Edge, Item
-from .central_schema import *
+from ._central_schema import *
+from .photo import Photo
+from .dataset import Dataset
 
 
 def get_constructor(_type, plugin_class=None, plugin_package=None, extra=None):
     from .photo import Photo
     import pymemri.integrator_registry
 
     if _type == "Indexer" and plugin_class is not None and hasattr(pymemri.integrator_registry, plugin_class):
```

### Comparing `pymemri-0.0.8/pymemri/plugin/authenticators/credentials.py` & `pymemri-0.0.9/pymemri/plugin/authenticators/credentials.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/authenticators/oauth.py` & `pymemri-0.0.9/pymemri/plugin/authenticators/oauth.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/authenticators/password.py` & `pymemri-0.0.9/pymemri/plugin/authenticators/password.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/listeners.py` & `pymemri-0.0.9/pymemri/plugin/listeners.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/pluginbase.py` & `pymemri-0.0.9/pymemri/plugin/pluginbase.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/stateful.py` & `pymemri-0.0.9/pymemri/plugin/stateful.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/plugin/states.py` & `pymemri-0.0.9/pymemri/plugin/states.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/pod/api.py` & `pymemri-0.0.9/pymemri/pod/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     def bulk(
         self,
         create_items: List[dict] = None,
         update_items: List[dict] = None,
         create_edges: List[dict] = None,
         delete_items: List[str] = None,
-        search: dict = None,
+        search: List[dict] = None,
     ) -> Dict[str, Any]:
 
         payload = {
             "createItems": create_items,
             "updateItems": update_items,
             "createEdges": create_edges,
             "deleteItems": delete_items,
```

### Comparing `pymemri-0.0.8/pymemri/pod/client.py` & `pymemri-0.0.9/pymemri/pod/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 __all__ = ['PodClient', 'Dog']
 
 # Cell
 from ..data.basic import *
 from ..data.schema import *
 from ..data.itembase import Edge, ItemBase, Item
-from ..data.photo import Photo, NUMPY, BYTES
 from ..imports import *
 from hashlib import sha256
 from .db import DB
 from .utils import *
 from ..plugin.schema import *
 from ..test_utils import get_ci_variables
 from .api import PodAPI, PodError, DEFAULT_POD_ADDRESS, POD_VERSION
@@ -92,28 +91,31 @@
 
     def create(self, node):
         create_dict = self.get_create_dict(node)
         try:
             result = self.api.create_item(create_dict)
             node.id = result
             self.add_to_db(node)
+            node.on_sync_to_pod(self)
             return True
         except Exception as e:
             print(e)
             return False
 
     def create_photo(self, photo):
-        # create the file
-        file_success = self.create_photo_file(photo)
-        if not file_success:
-            raise ValueError("Could not create file")
+        file = photo.file[0]
+
         # create the photo
-        return self.bulk_action(
-            create_items=[photo], create_edges=photo.get_edges("file")
+        items_edges_success = self.bulk_action(
+            create_items=[photo, file], create_edges=photo.get_edges("file")
         )
+        if not items_edges_success:
+            raise ValueError("Could not create file or photo item")
+
+        return self._upload_image(photo.data)
 
     def _property_dicts_from_instance(self, node):
         create_items = []
         attributes = node.to_json()
         for k, v in attributes.items():
             if type(v) not in self.TYPE_TO_SCHEMA:
                 raise ValueError(f"Could not add property {k} with type {type(v)}")
@@ -158,19 +160,14 @@
         try:
             self.api.bulk(create_items=create_items)
             return True
         except Exception as e:
             print(e)
             return False
 
-    def create_photo_file(self, photo):
-        file = photo.file[0]
-        self.create(file)
-        return self._upload_image(photo.data)
-
     def _upload_image(self, img):
         if isinstance(img, np.ndarray):
             return self.upload_file(img.tobytes())
         elif isinstance(img, bytes):
             return self.upload_file(img)
         else:
             raise ValueError(f"Unknown image data type {type(img)}")
@@ -197,33 +194,17 @@
         if len(photo.file) > 0 and photo.data is None:
             file = self.get_file(photo.file[0].sha256)
             if file is None:
                 print(
                     f"Could not load data of {photo} attached file item does not have data in pod"
                 )
                 return
-            if photo.encoding == NUMPY:
-                data = np.frombuffer(file, dtype=np.uint8)
-                c = photo.channels
-                shape = (
-                    (photo.height, photo.width, c)
-                    if c is not None and c > 1
-                    else (photo.height, photo.width)
-                )
-                data = data.reshape(shape)
-                if size is not None:
-                    data = resize(data, size)
-                photo.data = data
-                return
-            elif photo.encoding == BYTES:
-                photo.data = file
-                return
-            else:
-                raise ValueError("Unsupported encoding")
-        print(f"could not load data of {photo}, no file attached")
+            photo.data = file
+        else:
+            print(f"could not load data of {photo}, no file attached")
 
     def create_if_external_id_not_exists(self, node):
         if not self.external_id_exists(node):
             self.create(node)
 
     def external_id_exists(self, node):
         if node.externalId is None:
@@ -232,15 +213,14 @@
         return len(existing) > 0
 
     def create_edges(self, edges):
         return self.bulk_action(create_edges=edges)
 
     def delete_items(self, items):
         return self.bulk_action(delete_items=items)
-
     def delete_all(self):
         items = self.get_all_items()
         self.delete_items(items)
 
     @staticmethod
     def gather_batch(items, start_idx, start_size=0, max_size=5000000):
         idx = start_idx
@@ -257,28 +237,37 @@
                 total_size += len(str(x))
                 idx = i + 1
             else:
                 break
         return batch_items, idx, total_size
 
     def bulk_action(
-        self, create_items=None, update_items=None, create_edges=None, delete_items=None
+        self, create_items=None, update_items=None, create_edges=None, delete_items=None, partial_update=True
     ):
+        all_items = []
+        if create_items:
+            all_items += create_items
+        if update_items:
+            all_items += update_items
+        for item in all_items:
+            item._set_client(self)
+
         # we need to set the id to not lose the reference
         if create_items is not None:
             for c in create_items:
                 if c.id is None:
                     c.id = uuid.uuid4().hex
+
         create_items = (
             [self.get_create_dict(i) for i in create_items]
             if create_items is not None
             else []
         )
         update_items = (
-            [self.get_update_dict(i) for i in update_items]
+            [self.get_update_dict(i, partial_update=partial_update) for i in update_items]
             if update_items is not None
             else []
         )
         create_edges = (
             [self.get_create_edge_dict(i) for i in create_edges]
             if create_edges is not None
             else []
@@ -333,14 +322,17 @@
                     delete_items_batch,
                 )
             except PodError as e:
                 print(e)
                 print("could not complete bulk action, aborting")
                 return False
         print(f"Completed Bulk action, written {n} items/edges")
+
+        for item in all_items:
+            item.on_sync_to_pod(self)
         return True
 
     def get_create_edge_dict(self, edge):
         return {"_source": edge.source.id, "_target": edge.target.id, "_name": edge._type}
 
     def create_edge(self, edge):
         edge_dict = self.get_create_edge_dict(edge)
@@ -393,24 +385,26 @@
             if not len(result):
                 return
             return self.item_from_json(result[0])
         except PodError as e:
             print(e)
             return
 
-    def get_update_dict(self, node):
+    def get_update_dict(self, node, partial_update=True):
         properties = node.to_json(dates=False)
         properties.pop("type", None)
         properties.pop("deleted", None)
+        properties = {k: v for k, v in properties.items() if k=="id" or k in node._updated_properties}
         return properties
 
-    def update_item(self, node):
-        data = self.get_update_dict(node)
+    def update_item(self, node, partial_update=True):
+        data = self.get_update_dict(node, partial_update=partial_update)
         try:
             self.api.update_item(data)
+            node.on_sync_to_pod(self)
             return True
         except PodError as e:
             print(e)
             return False
 
     def exists(self, id):
         try:
@@ -418,58 +412,77 @@
             if isinstance(result, list) and len(result) > 0:
                 return True
             return False
         except PodError as e:
             print(e)
             return False
 
-    def search_paginate(self, fields_data, limit=50, include_edges=True):
+    def search_paginate(self, fields_data, limit=50, include_edges=True, add_to_local_db: bool = True):
+        if "ids" in fields_data:
+            raise NotImplementedError("Searching by multiple IDs is not implemented for paginated search.")
+
         extra_fields = {"[[edges]]": {}} if include_edges else {}
         query = {**fields_data, **extra_fields}
 
         try:
             for page in self.api.search_paginate(query, limit):
-                result = [self._item_from_search(item) for item in page]
+                result = [self._item_from_search(item, add_to_local_db=add_to_local_db) for item in page]
                 yield self.filter_deleted(result)
         except PodError as e:
             print(e)
 
-    def search(self, fields_data, include_edges: bool = True):
+    def search(self, fields_data, include_edges: bool = True, add_to_local_db: bool = True):
         extra_fields = {"[[edges]]": {}} if include_edges else {}
         query = {**fields_data, **extra_fields}
-        try:
-            result = self.api.search(query)
-            result = [self._item_from_search(item) for item in result]
-            return self.filter_deleted(result)
-        except PodError as e:
-            print(e)
 
-    def _item_from_search(self, item_json: dict):
+        # Special key "ids" for searching a list of ids.
+        # Requires /bulk search instead of /search.
+        if "ids" in query:
+            ids = query.pop("ids")
+            bulk_query = [{"id": uid, **query} for uid in ids]
+            try:
+                result = self.api.bulk(search=bulk_query)["search"]
+            except PodError as e:
+                print(e)
+
+            result = [item for sublist in result for item in sublist]
+        else:
+            try:
+                result = self.api.search(query)
+            except PodError as e:
+                print(e)
+
+        result = [self._item_from_search(item, add_to_local_db=add_to_local_db) for item in result]
+        return self.filter_deleted(result)
+
+    def _item_from_search(self, item_json: dict, add_to_local_db: bool = True):
         # search returns different fields w.r.t. edges compared to `get` api,
         # different method to keep `self.get` clean.
         item = self.item_from_json(item_json)
 
         for edge_json in item_json.get("[[edges]]", []):
             edge_name = edge_json["_edge"]
             try:
                 edge_item = self.item_from_json(edge_json["_item"])
                 item.add_edge(edge_name, edge_item)
             except Exception as e:
+                print(f"Could not attach edge {edge_json['_item']} to {item}")
+                print(e)
                 continue
         return item
 
     def search_last_added(self, type=None, with_prop=None, with_val=None):
         query = {"_limit": 1, "_sortOrder": "Desc"}
         if type is not None:
             query["type"] = type
         if with_prop is not None:
             query[f"{with_prop}=="] = with_val
         return self.search(query)[0]
 
-    def item_from_json(self, json):
+    def item_from_json(self, json, add_client_ref: bool = True, from_pod: bool = True):
         plugin_class = json.get("pluginClass", None)
         plugin_package = json.get("pluginPackage", None)
 
         constructor = get_constructor(
             json["type"],
             plugin_class,
             plugin_package=plugin_package,
@@ -484,17 +497,23 @@
                     edges = new_item.get_edges(edge_name)
                     for e in edges:
                         e.source = existing
                     existing.__setattr__(edge_name, edges)
 
             for prop_name in new_item.get_property_names():
                 existing.__setattr__(prop_name, new_item.__getattribute__(prop_name))
-            return existing
+            result = existing
         else:
-            return new_item
+            result = new_item
+
+        result._set_client(self) if add_client_ref else None
+        if from_pod:
+            result._in_pod = True
+            result._updated_properties = set()
+        return result
 
     def get_properties(self, expanded):
         properties = copy(expanded)
         if ALL_EDGES in properties:
             del properties[ALL_EDGES]
         return properties
```

### Comparing `pymemri-0.0.8/pymemri/pod/db.py` & `pymemri-0.0.9/pymemri/pod/db.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/pod/utils.py` & `pymemri-0.0.9/pymemri/pod/utils.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri/template/config.py` & `pymemri-0.0.9/pymemri/template/config.py`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/pymemri.egg-info/PKG-INFO` & `pymemri-0.0.9/pymemri.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pymemri
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python client for the memri data
 Home-page: https://gitlab.memri.io/memri/pymemri/tree/prod/
 Author: Koen van der Veen
 Author-email: koen.vanderveen@polis.global
 License: Apache Software License 2.0
 Description: # Pymemri
         > Pymemri is a python library for creating <b>Plugins</b> for the Memri Personal online datastore <a href='https://gitlab.memri.io/memri/pod'>(pod)</a>. Pymemri has a PodClient to communicate with the pod, and tools to build and test plugins.
         
         
         [![Gitlab pipeline status (self-hosted)](https://img.shields.io/gitlab/pipeline/memri/pymemri/dev?gitlab_url=https%3A%2F%2Fgitlab.memri.io&label=CI&logo=gitlab&style=plastic)](https://gitlab.memri.io/memri/pymemri/-/pipelines/latest)
         [![Discord](https://img.shields.io/discord/799216875480678430?color=blue&label=Discord&logo=discord&style=plastic)](https://discord.gg/BcRfajJk4k)
         [![Twitter URL](https://img.shields.io/twitter/url?label=%40YourMemri&logo=twitter&style=plastic&url=https%3A%2F%2Ftwitter.com%2FYourMemri)](https://twitter.com/YourMemri)
+        <a href="https://pypi.org/project/pymemri/"><img src="https://pepy.tech/badge/pymemri" /></a>
         
         Plugins connect and add the information to your Pod. Plugins that <b>import your data from external services</b> are called **Importers** (Gmail, WhatsApp, etc.). Plugins that <b>connect new data to the existing data</b> are called  **indexers** (face recognition, spam detection, object detection, etc.). Lastly there are plugins that <b>execute actions</b> (sending messages, uploading files). This repository is built with [nbdev](https://github.com/fastai/nbdev), which means that the repo structure has a few differences compared to a standard python repo. 
         
         ## Installing
         
         ### As a package
         ```bash
@@ -68,16 +69,15 @@
         run_plugin --metadata "example_plugin.json"
         ```
         
         This stores a random owner key and database key on your disk for future use, and runs the pymemri example plugin. If everything works correctly, the output should read `Plugin run success.`
         
         ## Docs
         
-        - [pymemri docs](http://memri.docs.memri.io/pymemri/pod.client.html#File-API)
-        - [plugin tutorial](https://blog.memri.io/getting-started-building-a-plugin/)
+        [pymemri docs](https://memri.docs.memri.io/docs.memri.io/component-architectures/plugins/readme/)
         
         ## Nbdev & Jupyter Notebooks
         The Python integrators are written in [nbdev](https://nbdev.fast.ai/) ([video](https://www.youtube.com/watch?v=9Q6sLbz37gk&t=1301s)). With nbdev, it is encouraged to write code in 
         [Jupyter Notebooks](https://jupyter.readthedocs.io/en/latest/install/notebook-classic.html). Nbdev syncs all the notebooks in `/nbs` with the python code in `/pymemri`. Tests are written side by side with the code in the notebooks, and documentation is automatically generated from the code and markdown in the notebooks and exported into the `/docs` folder. Check out the [nbdev quickstart](wiki/nbdev_quickstart.md) for an introduction, **watch the video linked above**, or see the [nbdev documentation](https://nbdev.fast.ai/) for a all functionalities and tutorials.
         
 Keywords: memri privacy personal data client python
 Platform: UNKNOWN
```

### Comparing `pymemri-0.0.8/pymemri.egg-info/SOURCES.txt` & `pymemri-0.0.9/pymemri.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,19 +21,22 @@
 pymemri/client_simulator/template/success.html
 pymemri/cvu/__init__.py
 pymemri/cvu/utils.py
 pymemri/cvu/definitions/password_auth.cvu
 pymemri/cvu/definitions/qr_code_auth.cvu
 pymemri/cvu/definitions/request_email.cvu
 pymemri/data/__init__.py
+pymemri/data/_central_schema.py
 pymemri/data/basic.py
-pymemri/data/central_schema.py
+pymemri/data/dataset.py
 pymemri/data/itembase.py
 pymemri/data/photo.py
 pymemri/data/schema.py
+pymemri/exporters/__init__.py
+pymemri/exporters/exporters.py
 pymemri/plugin/__init__.py
 pymemri/plugin/listeners.py
 pymemri/plugin/pluginbase.py
 pymemri/plugin/schema.py
 pymemri/plugin/stateful.py
 pymemri/plugin/states.py
 pymemri/plugin/authenticators/__init__.py
```

### Comparing `pymemri-0.0.8/pymemri.egg-info/entry_points.txt` & `pymemri-0.0.9/pymemri.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pymemri-0.0.8/settings.ini` & `pymemri-0.0.9/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 description = Python client for the memri data
 keywords = memri privacy personal data client python
 user = koenvanderveen
 author = Koen van der Veen
 author_email = koen.vanderveen@polis.global 
 copyright = Memri 
 branch = prod
-version = 0.0.8
+version = 0.0.9
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
 console_scripts = run_plugin=pymemri.plugin.pluginbase:run_plugin simulate_run_plugin_from_frontend=pymemri.plugin.pluginbase:simulate_run_plugin_from_frontend store_keys=pymemri.plugin.pluginbase:store_keys qr_simulator=pymemri.client_simulator.qr_simulator:run_qr_simulator simulate_enter_credentials=pymemri.plugin.authenticators.password:simulate_enter_credentials plugin_from_template=pymemri.template.formatter:plugin_from_template create_plugin_config=pymemri.template.config:create_plugin_config
-requirements = requests tqdm ipdb fastprogress fastscript opencv-python fastcore==1.3.21 nbdev==1.1.21 matplotlib jupyter-client==6.1.12 flask multidimensional_urlencode==0.0.4
+requirements = requests tqdm ipdb fastprogress fastscript fastcore==1.3.21 nbdev==1.1.21 matplotlib jupyter-client==6.1.12 flask giturlparse==0.10.0 pandas pillow==8.4.0
 
 nbs_path = nbs
 doc_path = docs 
 
 # url = /
 doc_host = http://memri.docs.memri.io
 doc_baseurl = /%(lib_name)s/
```

### Comparing `pymemri-0.0.8/setup.py` & `pymemri-0.0.9/setup.py`

 * *Files identical despite different names*

