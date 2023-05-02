# Comparing `tmp/deployv-0.9.98.tar.gz` & `tmp/deployv-0.9.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deployv-0.9.98.tar", last modified: Thu Jul 26 04:29:00 2018, max compression
+gzip compressed data, was "dist/deployv-0.9.99.tar", last modified: Fri Aug  3 02:53:38 2018, max compression
```

## Comparing `deployv-0.9.98.tar` & `deployv-0.9.99.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/
--rw-rw-rw-   0 root         (0) root         (0)     1475 2018-07-25 20:48:24.000000 deployv-0.9.98/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     4659 2018-07-25 20:48:24.000000 deployv-0.9.98/README.md
--rw-r--r--   0 root         (0) root         (0)     6378 2018-07-26 04:29:00.000000 deployv-0.9.98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      238 2018-07-25 20:48:24.000000 deployv-0.9.98/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)       38 2018-07-26 04:29:00.000000 deployv-0.9.98/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3442 2018-07-25 20:48:24.000000 deployv-0.9.98/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     4658 2018-07-26 04:20:27.000000 deployv-0.9.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/base/
--rw-rw-rw-   0 root         (0) root         (0)    12979 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/postgresv.py
--rw-rw-rw-   0 root         (0) root         (0)    67407 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/commandv.py
--rw-rw-rw-   0 root         (0) root         (0)     6174 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/extensions_core.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/update_production.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    30104 2018-07-26 03:39:13.000000 deployv-0.9.98/deployv/base/dockerv.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/nginxv.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/commands/
--rw-rw-rw-   0 root         (0) root         (0)    27171 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/commands/deployvcmd.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/commands/updatev.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/commands/workerv.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/instance/
--rw-rw-rw-   0 root         (0) root         (0)    72324 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/instance/instancev.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/messaging/
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/messaging/http/
--rw-rw-rw-   0 root         (0) root         (0)     1334 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/http/worker.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/http/httpv.py
--rw-rw-rw-   0 root         (0) root         (0)     1588 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/http/receiverv.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/http/senderv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/messaging/rabbit/
--rw-rw-rw-   0 root         (0) root         (0)     1726 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/rabbit/worker.py
--rw-rw-rw-   0 root         (0) root         (0)    14454 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/rabbit/receiverv.py
--rw-rw-rw-   0 root         (0) root         (0)      580 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/rabbit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4248 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/rabbit/senderv.py
--rw-rw-rw-   0 root         (0) root         (0)     4254 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/rabbit/rabbitv.py
--rw-rw-rw-   0 root         (0) root         (0)    14543 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/basemsg.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/messaging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/helpers/
--rw-rw-rw-   0 root         (0) root         (0)    19998 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/build_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     6592 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/database_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/decompress_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    27703 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5322 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/clone_oca_dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     6515 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/container.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/backup.py
--rw-rw-rw-   0 root         (0) root         (0)     7646 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/json_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    14115 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/configuration_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     2545 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/sender_message.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/helpers/helpers-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv/extensions/
--rw-rw-rw-   0 root         (0) root         (0)     9620 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/extensions/checkers.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2018-07-25 20:48:24.000000 deployv-0.9.98/deployv/extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2018-07-26 04:20:27.000000 deployv-0.9.98/deployv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6378 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1604 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        8 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      127 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      252 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-07-26 04:29:00.000000 deployv-0.9.98/deployv.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      131 2018-07-25 20:48:24.000000 deployv-0.9.98/test-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      224 2018-07-25 20:48:24.000000 deployv-0.9.98/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      252 2018-07-25 20:48:24.000000 deployv-0.9.98/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2018-08-02 15:44:10.000000 deployv-0.9.99/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2018-08-02 15:44:10.000000 deployv-0.9.99/README.md
+-rw-r--r--   0 root         (0) root         (0)     6378 2018-08-03 02:53:38.000000 deployv-0.9.99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      238 2018-08-02 15:44:10.000000 deployv-0.9.99/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2018-08-03 02:53:38.000000 deployv-0.9.99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2018-08-02 15:44:10.000000 deployv-0.9.99/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4658 2018-08-02 18:29:14.000000 deployv-0.9.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/base/
+-rw-rw-rw-   0 root         (0) root         (0)    12979 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/postgresv.py
+-rw-rw-rw-   0 root         (0) root         (0)    67572 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/commandv.py
+-rw-rw-rw-   0 root         (0) root         (0)     6174 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/extensions_core.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/update_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    30104 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/dockerv.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/nginxv.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/commands/
+-rw-rw-rw-   0 root         (0) root         (0)    27171 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/commands/deployvcmd.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/commands/updatev.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/commands/workerv.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/instance/
+-rw-rw-rw-   0 root         (0) root         (0)    72324 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/instance/instancev.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/messaging/
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/messaging/http/
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/http/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/http/httpv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1588 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/http/receiverv.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/http/senderv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/messaging/rabbit/
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/rabbit/worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14454 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/rabbit/receiverv.py
+-rw-rw-rw-   0 root         (0) root         (0)      580 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/rabbit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/rabbit/senderv.py
+-rw-rw-rw-   0 root         (0) root         (0)     4254 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/rabbit/rabbitv.py
+-rw-rw-rw-   0 root         (0) root         (0)    14543 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/basemsg.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/messaging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)    19998 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/build_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     6592 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/database_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/decompress_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    27703 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5322 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/clone_oca_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     6515 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/container.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/backup.py
+-rw-rw-rw-   0 root         (0) root         (0)     7646 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/json_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    14115 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/configuration_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/sender_message.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/helpers/helpers-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)     9620 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/extensions/checkers.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2018-08-02 15:44:10.000000 deployv-0.9.99/deployv/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2018-08-02 18:29:14.000000 deployv-0.9.99/deployv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6378 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1604 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      252 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-08-03 02:53:38.000000 deployv-0.9.99/deployv.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      131 2018-08-02 15:44:10.000000 deployv-0.9.99/test-requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      224 2018-08-02 15:44:10.000000 deployv-0.9.99/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      252 2018-08-02 15:44:10.000000 deployv-0.9.99/requirements.txt
```

### Comparing `deployv-0.9.98/LICENSE` & `deployv-0.9.99/LICENSE`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/README.md` & `deployv-0.9.99/README.md`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/PKG-INFO` & `deployv-0.9.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: deployv
-Version: 0.9.98
+Version: 0.9.99
 Summary: Base for all clases and scripts in VauxooTools
 Home-page: https://github.com/vauxoo/deployv
 Author: Tulio Ruiz
 Author-email: tulio@vauxoo.com
 License: BSD
 Download-URL: https://github.com/vauxoo/deployv
 Description: CI Status
```

### Comparing `deployv-0.9.98/CONTRIBUTING.rst` & `deployv-0.9.99/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/setup.py` & `deployv-0.9.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 readme = open('README.md').read()
 requirements = open('requirements.txt').readlines()
 test_requirements = open('test-requirements.txt').readlines()
 
 setup(
     name='deployv',
-    version='0.9.98',
+    version='0.9.99',
     description='Base for all clases and scripts in VauxooTools',
     long_description=readme,
     package_data={'': [
         'templates/files/*', 'templates/*.jinja', 'config/*', 'helpers/json_schemas/*',
     ]},
     author='Tulio Ruiz',
     author_email='tulio@vauxoo.com',
```

### Comparing `deployv-0.9.98/deployv/base/postgresv.py` & `deployv-0.9.99/deployv/base/postgresv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/base/commandv.py` & `deployv-0.9.99/deployv/base/commandv.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
         base_img = (base_img.split(':')[0] if base_img else
                     'quay.io/vauxoo/{}'.format(res['result'].get('image_name')))
         tag_img = '{img}:{tag}'.format(
             img=base_img, tag=res['result'].get('image_sha'))
         if not isinstance(self.__config.container_config.get('push_image'), list):
             self.__config.container_config.update({'push_image': []})
         self.__config.container_config.get('push_image').append(tag_img)
+        self.__config.container_config.update({'tag_latest': tag_img})
         self.build_done_trigger()
         return res
 
     @utils.traceback_docker_error
     @events
     def create(self):
         """Creates an Odoo dockerized instance with the provided configuration.
@@ -942,15 +943,16 @@
             push_details = push_result.get('result').get('push_result').get('log')
             res.get('attachments').append({
                 'file_name': 'push_image_{tag}.json'.format(tag=tag),
                 'file': base64.b64encode(utils.encode(json.dumps(push_details, indent=4))),
                 'type': 'application/json',
             })
             pushed_imgs.append(push_result.get('result').get('tagged_image'))
-        res['result'].update({'images': pushed_imgs})
+        res['result'].update({'images': pushed_imgs,
+                              'tag_latest': self.__config.container_config.get('tag_latest')})
         self.sender.send_message('Images pushed.', body=res)
         self.push_images_done_trigger()
         return res
 
     def create_db_demo(self):
         """ This method creates an empty database.
```

### Comparing `deployv-0.9.98/deployv/base/extensions_core.py` & `deployv-0.9.99/deployv/base/extensions_core.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/base/errors.py` & `deployv-0.9.99/deployv/base/errors.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/base/dockerv.py` & `deployv-0.9.99/deployv/base/dockerv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/base/nginxv.py` & `deployv-0.9.99/deployv/base/nginxv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/commands/deployvcmd.py` & `deployv-0.9.99/deployv/commands/deployvcmd.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/commands/workerv.py` & `deployv-0.9.99/deployv/commands/workerv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/instance/instancev.py` & `deployv-0.9.99/deployv/instance/instancev.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/instance/__init__.py` & `deployv-0.9.99/deployv/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/http/worker.py` & `deployv-0.9.99/deployv/messaging/http/worker.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/http/httpv.py` & `deployv-0.9.99/deployv/messaging/http/httpv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/http/receiverv.py` & `deployv-0.9.99/deployv/messaging/http/receiverv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/http/senderv.py` & `deployv-0.9.99/deployv/messaging/http/senderv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/rabbit/worker.py` & `deployv-0.9.99/deployv/messaging/rabbit/worker.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/rabbit/receiverv.py` & `deployv-0.9.99/deployv/messaging/rabbit/receiverv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/rabbit/__init__.py` & `deployv-0.9.99/deployv/messaging/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/rabbit/senderv.py` & `deployv-0.9.99/deployv/messaging/rabbit/senderv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/rabbit/rabbitv.py` & `deployv-0.9.99/deployv/messaging/rabbit/rabbitv.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/messaging/basemsg.py` & `deployv-0.9.99/deployv/messaging/basemsg.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/build_helper.py` & `deployv-0.9.99/deployv/helpers/build_helper.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/database_helper.py` & `deployv-0.9.99/deployv/helpers/database_helper.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/decompress_helper.py` & `deployv-0.9.99/deployv/helpers/decompress_helper.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/utils.py` & `deployv-0.9.99/deployv/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/clone_oca_dependencies.py` & `deployv-0.9.99/deployv/helpers/clone_oca_dependencies.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/container.py` & `deployv-0.9.99/deployv/helpers/container.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/backup.py` & `deployv-0.9.99/deployv/helpers/backup.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/json_helper.py` & `deployv-0.9.99/deployv/helpers/json_helper.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/configuration_helper.py` & `deployv-0.9.99/deployv/helpers/configuration_helper.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/helpers/sender_message.py` & `deployv-0.9.99/deployv/helpers/sender_message.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/extensions/checkers.py` & `deployv-0.9.99/deployv/extensions/checkers.py`

 * *Files identical despite different names*

### Comparing `deployv-0.9.98/deployv/__init__.py` & `deployv-0.9.99/deployv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 For that we created a package with all needed modules (at least those developed by us) to backup,
 start, update and build instances.
 """
 
 import logging
 
 __author__ = 'Tulio Ruiz <tulio@vauxoo.com>'
-__version__ = '0.9.98'
+__version__ = '0.9.99'
 __all__ = ['base', 'helpers', 'instance', 'messaging']
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s - %(levelname)-5s - %(name)s.%(funcName)s - %(message)s"
 )
```

### Comparing `deployv-0.9.98/deployv.egg-info/PKG-INFO` & `deployv-0.9.99/deployv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: deployv
-Version: 0.9.98
+Version: 0.9.99
 Summary: Base for all clases and scripts in VauxooTools
 Home-page: https://github.com/vauxoo/deployv
 Author: Tulio Ruiz
 Author-email: tulio@vauxoo.com
 License: BSD
 Download-URL: https://github.com/vauxoo/deployv
 Description: CI Status
```

### Comparing `deployv-0.9.98/deployv.egg-info/SOURCES.txt` & `deployv-0.9.99/deployv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

