# Comparing `tmp/pwclient-2.6.0.tar.gz` & `tmp/pwclient-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwclient-2.6.0.tar", last modified: Thu Mar 30 11:24:16 2023, max compression
+gzip compressed data, was "pwclient-2.6.1.tar", last modified: Tue May  2 10:42:05 2023, max compression
```

## Comparing `pwclient-2.6.0.tar` & `pwclient-2.6.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.111894 pwclient-2.6.0/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       41 2022-06-13 12:28:36.000000 pwclient-2.6.0/.git-blame-ignore-revs
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.104894 pwclient-2.6.0/.github/
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.106893 pwclient-2.6.0/.github/workflows/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     2578 2023-03-30 11:24:01.000000 pwclient-2.6.0/.github/workflows/ci.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      526 2022-06-13 12:28:36.000000 pwclient-2.6.0/.pre-commit-config.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1549 2023-03-30 11:24:15.000000 pwclient-2.6.0/AUTHORS
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)    18092 2018-10-17 14:18:19.000000 pwclient-2.6.0/COPYING
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     7848 2023-03-30 11:24:15.000000 pwclient-2.6.0/ChangeLog
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     3440 2023-03-30 11:24:16.111894 pwclient-2.6.0/PKG-INFO
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     2400 2022-06-13 12:42:23.000000 pwclient-2.6.0/README.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.106893 pwclient-2.6.0/docs/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      984 2023-02-13 12:11:03.000000 pwclient-2.6.0/docs/conf.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     2838 2022-06-13 12:42:23.000000 pwclient-2.6.0/docs/configuration.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      185 2023-02-13 12:11:03.000000 pwclient-2.6.0/docs/index.rst
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       48 2019-09-06 16:28:37.000000 pwclient-2.6.0/docs/release-notes.rst
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       43 2023-02-13 12:11:03.000000 pwclient-2.6.0/docs/requirements.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       78 2019-09-06 16:28:37.000000 pwclient-2.6.0/docs/usage.rst
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.106893 pwclient-2.6.0/man/
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     9219 2023-03-30 11:13:44.000000 pwclient-2.6.0/man/pwclient.1
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.107894 pwclient-2.6.0/pwclient/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      503 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/__init__.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    25527 2023-03-30 11:10:06.000000 pwclient-2.6.0/pwclient/api.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1973 2022-06-14 17:38:45.000000 pwclient-2.6.0/pwclient/checks.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      212 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/exceptions.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     9483 2023-02-13 11:24:12.000000 pwclient-2.6.0/pwclient/parser.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     6358 2023-03-30 11:08:12.000000 pwclient-2.6.0/pwclient/patches.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      518 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/projects.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     8388 2023-02-13 11:24:12.000000 pwclient-2.6.0/pwclient/shell.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      403 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/states.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1552 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/utils.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1563 2022-06-13 12:28:36.000000 pwclient-2.6.0/pwclient/xmlrpc.py
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.108893 pwclient-2.6.0/pwclient.egg-info/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     3440 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/PKG-INFO
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1949 2023-03-30 11:24:16.000000 pwclient-2.6.0/pwclient.egg-info/SOURCES.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/dependency_links.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       49 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/entry_points.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        1 2019-09-16 12:25:29.000000 pwclient-2.6.0/pwclient.egg-info/not-zip-safe
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       46 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/pbr.json
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       46 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/requires.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        9 2023-03-30 11:24:15.000000 pwclient-2.6.0/pwclient.egg-info/top_level.txt
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       63 2022-06-13 12:28:36.000000 pwclient-2.6.0/pyproject.toml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       66 2019-09-06 16:28:37.000000 pwclient-2.6.0/readthedocs.yml
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.108893 pwclient-2.6.0/releasenotes/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       25 2022-07-18 11:28:36.000000 pwclient-2.6.0/releasenotes/config.yaml
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.110894 pwclient-2.6.0/releasenotes/notes/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      127 2019-09-06 22:44:36.000000 pwclient-2.6.0/releasenotes/notes/add-long-opts-4611e7cce3993f08.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      106 2022-12-06 13:19:20.000000 pwclient-2.6.0/releasenotes/notes/add-python3-10-drop-python-3-6-support-32b91d5753adfc29.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)       60 2022-12-06 13:19:19.000000 pwclient-2.6.0/releasenotes/notes/add-python3-11-support-eb86886925d2e5ec.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      119 2021-08-17 21:30:24.000000 pwclient-2.6.0/releasenotes/notes/check-get-4f010b2c4fdcd55c.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      114 2022-06-13 12:28:36.000000 pwclient-2.6.0/releasenotes/notes/check-list-create-help-94ccb51660af1138.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      593 2022-06-13 12:28:36.000000 pwclient-2.6.0/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       63 2019-09-21 18:45:09.000000 pwclient-2.6.0/releasenotes/notes/drop-pypy-support-17f1f95b9394b257.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      132 2021-08-17 21:30:24.000000 pwclient-2.6.0/releasenotes/notes/drop-python2-support-0351245b41052e20.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      107 2021-08-17 21:30:24.000000 pwclient-2.6.0/releasenotes/notes/git-am--m-flag-190f3a7e17cec6f4.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       58 2019-09-06 16:28:37.000000 pwclient-2.6.0/releasenotes/notes/initial-release-eb74a7ae0ce3b1fb.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      102 2019-09-06 21:28:26.000000 pwclient-2.6.0/releasenotes/notes/issue-1-c7e4c3e4e57c1c22.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      115 2023-02-13 11:26:26.000000 pwclient-2.6.0/releasenotes/notes/list--hash-option-ebb96d3a70920cf5.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      171 2022-06-13 15:29:40.000000 pwclient-2.6.0/releasenotes/notes/pwclientrc-environment-variable-e070047b82e3b77f.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      697 2022-06-13 12:28:36.000000 pwclient-2.6.0/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      355 2022-06-14 16:52:17.000000 pwclient-2.6.0/releasenotes/notes/version-2-2-0d142cb0ab85eb67.yaml
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)      134 2022-08-16 10:14:18.000000 pwclient-2.6.0/releasenotes/notes/version-2-3-fd18e538b15396d8.yaml
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       40 2022-06-13 12:28:36.000000 pwclient-2.6.0/requirements.txt
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1088 2023-03-30 11:24:16.111894 pwclient-2.6.0/setup.cfg
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      104 2019-09-06 16:28:37.000000 pwclient-2.6.0/setup.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)       18 2022-06-13 12:28:36.000000 pwclient-2.6.0/test-requirements.txt
-drwxr-xr-x   0 stephenfin  (1000) stephenfin  (1000)        0 2023-03-30 11:24:16.110894 pwclient-2.6.0/tests/
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)        0 2019-09-06 16:28:37.000000 pwclient-2.6.0/tests/__init__.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     3167 2022-06-14 17:38:03.000000 pwclient-2.6.0/tests/fakes.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)     1036 2023-03-30 10:34:51.000000 pwclient-2.6.0/tests/test_api.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     2211 2022-06-14 17:37:39.000000 pwclient-2.6.0/tests/test_checks.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    13530 2023-02-13 11:24:12.000000 pwclient-2.6.0/tests/test_patches.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      445 2022-06-13 12:28:36.000000 pwclient-2.6.0/tests/test_projects.py
--rw-r--r--   0 stephenfin  (1000) stephenfin  (1000)    27493 2023-02-13 11:24:12.000000 pwclient-2.6.0/tests/test_shell.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      342 2022-06-13 12:28:36.000000 pwclient-2.6.0/tests/test_states.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)      888 2022-06-13 12:28:36.000000 pwclient-2.6.0/tests/test_utils.py
--rw-rw-r--   0 stephenfin  (1000) stephenfin  (1000)     1418 2022-12-06 13:16:55.000000 pwclient-2.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.216703 pwclient-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-02 10:41:53.000000 pwclient-2.6.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-02 10:41:53.000000 pwclient-2.6.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-02 10:41:53.000000 pwclient-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-02 10:42:05.000000 pwclient-2.6.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-02 10:41:53.000000 pwclient-2.6.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-02 10:42:05.000000 pwclient-2.6.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-02 10:42:05.216703 pwclient-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-02 10:41:53.000000 pwclient-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-02 10:41:53.000000 pwclient-2.6.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.208703 pwclient-2.6.1/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-05-02 10:41:53.000000 pwclient-2.6.1/man/pwclient.1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/pwclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25612 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-02 10:41:53.000000 pwclient-2.6.1/pwclient/xmlrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/pwclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 10:42:05.000000 pwclient-2.6.1/pwclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 10:41:53.000000 pwclient-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-02 10:41:53.000000 pwclient-2.6.1/readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/releasenotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.212703 pwclient-2.6.1/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-long-opts-4611e7cce3993f08.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-python3-10-drop-python-3-6-support-32b91d5753adfc29.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/add-python3-11-support-eb86886925d2e5ec.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-get-4f010b2c4fdcd55c.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-list-create-help-94ccb51660af1138.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/drop-pypy-support-17f1f95b9394b257.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/drop-python2-support-0351245b41052e20.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/git-am--m-flag-190f3a7e17cec6f4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/initial-release-eb74a7ae0ce3b1fb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/issue-1-c7e4c3e4e57c1c22.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/list--hash-option-ebb96d3a70920cf5.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/pwclientrc-environment-variable-e070047b82e3b77f.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/version-2-2-0d142cb0ab85eb67.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-02 10:41:53.000000 pwclient-2.6.1/releasenotes/notes/version-2-3-fd18e538b15396d8.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-02 10:41:53.000000 pwclient-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-02 10:42:05.216703 pwclient-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 10:41:53.000000 pwclient-2.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 10:41:53.000000 pwclient-2.6.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:42:05.216703 pwclient-2.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27493 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 10:41:53.000000 pwclient-2.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 10:41:53.000000 pwclient-2.6.1/tox.ini
```

### Comparing `pwclient-2.6.0/.github/workflows/ci.yaml` & `pwclient-2.6.1/.github/workflows/ci.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -58,31 +58,54 @@
           name: html-docs-build
           path: docs/_build/html
           retention-days: 7
   release:
     name: Upload release artifacts
     runs-on: ubuntu-latest
     needs: test
-    if: github.event_name == 'push'
+    if: ${{ github.event_name == 'push' }}
     steps:
       - name: Checkout source code
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.11'
       - name: Install dependencies
         run: python -m pip install build
       - name: Build a binary wheel and a source tarball
         run: python -m build --sdist --wheel --outdir dist/ .
       - name: Publish distribution to Test PyPI
+        if: ${{ ! startsWith(github.ref, 'refs/tags') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
       - name: Publish distribution to PyPI
-        if: startsWith(github.ref, 'refs/tags')
+        if: ${{ startsWith(github.ref, 'refs/tags') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Create release on GitHub
+        id: create_release
+        if: startsWith(github.ref, 'refs/tags')
+        uses: actions/create-release@v1
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+          tag_name: ${{ github.ref }}
+          release_name: ${{ github.ref }}
+          draft: false
+          prerelease: false
+      - name: Add sdist to release
+        id: upload-release-asset
+        if: startsWith(github.ref, 'refs/tags')
+        uses: actions/upload-release-asset@v1
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+          upload_url: ${{ steps.create_release.outputs.upload_url }}
+          asset_path: ./dist/git-pw-${{ github.ref }}.tar.gz
+          asset_name: git-pw-${{ github.ref }}.tar.gz
+          asset_content_type: application/gzip
```

### Comparing `pwclient-2.6.0/.pre-commit-config.yaml` & `pwclient-2.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/AUTHORS` & `pwclient-2.6.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/COPYING` & `pwclient-2.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/ChangeLog` & `pwclient-2.6.1/ChangeLog`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+2.6.1
+-----
+
+* Release 2.6.1
+* xmlrpc: Enable 'allow\_none'
+* CI: Enable releases
+* CI: Don't put to test-pypi on release
+
 2.6.0
 -----
 
 * Release 2.6.0
 * api: More signature corrections
 * api: Strip trailing slashes
 * api: Fix patch list for REST API
```

### Comparing `pwclient-2.6.0/PKG-INFO` & `pwclient-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwclient
-Version: 2.6.0
+Version: 2.6.1
 Summary: The command-line client for the Patchwork patch tracking tool
 Home-page: https://github.com/getpatchwork/pwclient
 Author: Nate Case
 Author-email: ncase@xes-inc.com
 Maintainer: Stephen Finucane
 Maintainer-email: stephen@that.guru
 License: GPL v2
```

### Comparing `pwclient-2.6.0/README.rst` & `pwclient-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/docs/conf.py` & `pwclient-2.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/docs/configuration.rst` & `pwclient-2.6.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/man/pwclient.1` & `pwclient-2.6.1/man/pwclient.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH PWCLIENT "1" "2023\-03\-30" "pwclient" "Generated Python Manual"
+.TH PWCLIENT "1" "2023\-05\-02" "pwclient" "Generated Python Manual"
 .SH NAME
 pwclient
 .SH SYNOPSIS
 .B pwclient
 [-h] {apply,git-am,get,info,projects,check-get,check-list,check-info,check-create,states,view,update,list,search} ...
 
 .SH
```

### Comparing `pwclient-2.6.0/pwclient/api.py` & `pwclient-2.6.1/pwclient/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,19 @@
         self._server = server
 
         transport = xmlrpc.Transport(self._server)
         if username and password:
             transport.set_credentials(username, password)
 
         try:
-            rpc = xmlrpc.xmlrpclib.Server(self._server, transport=transport)
+            rpc = xmlrpc.xmlrpclib.ServerProxy(
+                self._server,
+                transport=transport,
+                allow_none=True,
+            )
         except (IOError, OSError):
             raise exceptions.APIError(f'Unable to connect to {self._server}')
 
         self._client = rpc
 
     # project
```

### Comparing `pwclient-2.6.0/pwclient/checks.py` & `pwclient-2.6.1/pwclient/checks.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/parser.py` & `pwclient-2.6.1/pwclient/parser.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/patches.py` & `pwclient-2.6.1/pwclient/patches.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/projects.py` & `pwclient-2.6.1/pwclient/projects.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/shell.py` & `pwclient-2.6.1/pwclient/shell.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/utils.py` & `pwclient-2.6.1/pwclient/utils.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient/xmlrpc.py` & `pwclient-2.6.1/pwclient/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/pwclient.egg-info/PKG-INFO` & `pwclient-2.6.1/pwclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwclient
-Version: 2.6.0
+Version: 2.6.1
 Summary: The command-line client for the Patchwork patch tracking tool
 Home-page: https://github.com/getpatchwork/pwclient
 Author: Nate Case
 Author-email: ncase@xes-inc.com
 Maintainer: Stephen Finucane
 Maintainer-email: stephen@that.guru
 License: GPL v2
```

### Comparing `pwclient-2.6.0/pwclient.egg-info/SOURCES.txt` & `pwclient-2.6.1/pwclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml` & `pwclient-2.6.1/releasenotes/notes/check-patch-id-82f673f7c520ca24.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml` & `pwclient-2.6.1/releasenotes/notes/rest-api-support-4341d2884f8d41c8.yaml`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/setup.cfg` & `pwclient-2.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/fakes.py` & `pwclient-2.6.1/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/test_api.py` & `pwclient-2.6.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/test_checks.py` & `pwclient-2.6.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/test_patches.py` & `pwclient-2.6.1/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/test_shell.py` & `pwclient-2.6.1/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tests/test_utils.py` & `pwclient-2.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pwclient-2.6.0/tox.ini` & `pwclient-2.6.1/tox.ini`

 * *Files identical despite different names*

