# Comparing `tmp/bfet-0.1.8.tar.gz` & `tmp/bfet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfet-0.1.8.tar", last modified: Thu Dec 22 23:51:03 2022, max compression
+gzip compressed data, was "bfet-0.1.9.tar", last modified: Tue Apr 25 23:06:19 2023, max compression
```

## Comparing `bfet-0.1.8.tar` & `bfet-0.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.150411 bfet-0.1.8/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      156 2022-09-13 20:59:52.000000 bfet-0.1.8/AUTHORS.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3472 2022-09-13 20:59:52.000000 bfet-0.1.8/CONTRIBUTING.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      164 2022-11-04 22:19:06.000000 bfet-0.1.8/HISTORY.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1071 2022-09-13 20:59:52.000000 bfet-0.1.8/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      262 2022-09-13 20:59:52.000000 bfet-0.1.8/MANIFEST.in
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2948 2022-12-22 23:51:03.150411 bfet-0.1.8/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2020 2022-11-19 20:57:38.000000 bfet-0.1.8/README.rst
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.142411 bfet-0.1.8/bfet/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      234 2022-12-22 23:48:19.000000 bfet-0.1.8/bfet/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       99 2022-10-11 09:31:39.000000 bfet-0.1.8/bfet/__main__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.142411 bfet-0.1.8/bfet/automatic_tests/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2022-09-14 08:49:03.000000 bfet-0.1.8/bfet/automatic_tests/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      273 2022-10-11 09:31:39.000000 bfet-0.1.8/bfet/automatic_tests/autotest.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7033 2022-12-07 18:26:47.000000 bfet-0.1.8/bfet/automatic_tests/create_tests.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 14:06:03.000000 bfet-0.1.8/bfet/automatic_tests/django_tests.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2583 2022-10-11 14:06:03.000000 bfet-0.1.8/bfet/automatic_tests/settings.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1241 2022-12-06 20:18:42.000000 bfet-0.1.8/bfet/cli.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.142411 bfet-0.1.8/bfet/create_data/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       64 2022-09-14 08:49:03.000000 bfet-0.1.8/bfet/create_data/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     9006 2022-09-14 08:49:03.000000 bfet-0.1.8/bfet/create_data/constants.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6684 2022-12-22 23:49:08.000000 bfet-0.1.8/bfet/create_data/create_data.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.142411 bfet-0.1.8/bfet/testing_models/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       86 2022-10-11 09:31:39.000000 bfet-0.1.8/bfet/testing_models/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8091 2022-12-22 23:43:07.000000 bfet-0.1.8/bfet/testing_models/django_model.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.142411 bfet-0.1.8/bfet.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2948 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1353 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       39 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/not-zip-safe
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        5 2022-12-22 23:51:02.000000 bfet-0.1.8/bfet.egg-info/top_level.txt
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/docs/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      605 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/Makefile
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       28 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/authors.rst
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)     4739 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/conf.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       33 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/contributing.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       28 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/history.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/index.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/installation.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      802 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/make.bat
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       27 2022-09-13 20:59:52.000000 bfet-0.1.8/docs/readme.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1606 2022-10-21 16:26:57.000000 bfet-0.1.8/docs/usage.rst
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       71 2022-10-11 14:06:03.000000 bfet-0.1.8/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      490 2022-12-22 23:51:03.150411 bfet-0.1.8/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1622 2022-12-22 23:48:19.000000 bfet-0.1.8/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 22:53:00.000000 bfet-0.1.8/tests/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2460 2022-10-11 14:06:03.000000 bfet-0.1.8/tests/conftest.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/django_examples/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.8/tests/django_examples/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/django_examples/migrations/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      953 2022-12-22 23:50:33.000000 bfet-0.1.8/tests/django_examples/migrations/0001_initial.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-12 16:03:58.000000 bfet-0.1.8/tests/django_examples/migrations/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3208 2022-12-22 23:50:35.000000 bfet-0.1.8/tests/django_examples/models.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/test_automatic_tests/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 23:14:02.000000 bfet-0.1.8/tests/test_automatic_tests/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3375 2022-10-11 14:06:03.000000 bfet-0.1.8/tests/test_automatic_tests/test_create_tests.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/test_create_data/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 23:13:06.000000 bfet-0.1.8/tests/test_create_data/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     2043 2022-10-11 14:06:03.000000 bfet-0.1.8/tests/test_create_data/test_datacreator.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/test_testing_models/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.8/tests/test_testing_models/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2022-12-22 23:51:03.146411 bfet-0.1.8/tests/test_testing_models/test_django/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.8/tests/test_testing_models/test_django/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1240 2022-12-22 23:50:54.000000 bfet-0.1.8/tests/test_testing_models/test_django/test_django_model.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      156 2022-09-13 20:59:52.000000 bfet-0.1.9/AUTHORS.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3472 2022-09-13 20:59:52.000000 bfet-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      164 2022-11-04 22:19:06.000000 bfet-0.1.9/HISTORY.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1071 2022-09-13 20:59:52.000000 bfet-0.1.9/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      262 2022-09-13 20:59:52.000000 bfet-0.1.9/MANIFEST.in
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2948 2023-04-25 23:06:19.414242 bfet-0.1.9/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2020 2022-11-19 20:57:38.000000 bfet-0.1.9/README.rst
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.406242 bfet-0.1.9/bfet/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      234 2023-04-25 23:05:46.000000 bfet-0.1.9/bfet/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       99 2022-10-11 09:31:39.000000 bfet-0.1.9/bfet/__main__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.410242 bfet-0.1.9/bfet/automatic_tests/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       62 2022-09-14 08:49:03.000000 bfet-0.1.9/bfet/automatic_tests/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      273 2022-10-11 09:31:39.000000 bfet-0.1.9/bfet/automatic_tests/autotest.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7033 2022-12-07 18:26:47.000000 bfet-0.1.9/bfet/automatic_tests/create_tests.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 14:06:03.000000 bfet-0.1.9/bfet/automatic_tests/django_tests.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2583 2022-10-11 14:06:03.000000 bfet-0.1.9/bfet/automatic_tests/settings.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1241 2022-12-06 20:18:42.000000 bfet-0.1.9/bfet/cli.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.410242 bfet-0.1.9/bfet/create_data/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       64 2022-09-14 08:49:03.000000 bfet-0.1.9/bfet/create_data/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     9006 2022-09-14 08:49:03.000000 bfet-0.1.9/bfet/create_data/constants.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6948 2023-04-25 22:59:48.000000 bfet-0.1.9/bfet/create_data/create_data.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.410242 bfet-0.1.9/bfet/testing_models/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       86 2022-10-11 09:31:39.000000 bfet-0.1.9/bfet/testing_models/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7981 2023-04-25 22:51:45.000000 bfet-0.1.9/bfet/testing_models/django_model.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.410242 bfet-0.1.9/bfet.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2948 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1353 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       39 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/not-zip-safe
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        7 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        5 2023-04-25 23:06:19.000000 bfet-0.1.9/bfet.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/docs/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      605 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/Makefile
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       28 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/authors.rst
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)     4739 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/conf.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       33 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/contributing.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       28 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/history.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/index.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1090 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/installation.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      802 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/make.bat
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       27 2022-09-13 20:59:52.000000 bfet-0.1.9/docs/readme.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1606 2022-10-21 16:26:57.000000 bfet-0.1.9/docs/usage.rst
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       71 2022-10-11 14:06:03.000000 bfet-0.1.9/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      490 2023-04-25 23:06:19.414242 bfet-0.1.9/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1622 2023-04-25 23:05:46.000000 bfet-0.1.9/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 22:53:00.000000 bfet-0.1.9/tests/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2460 2022-10-11 14:06:03.000000 bfet-0.1.9/tests/conftest.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/django_examples/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.9/tests/django_examples/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/django_examples/migrations/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      953 2022-12-22 23:50:33.000000 bfet-0.1.9/tests/django_examples/migrations/0001_initial.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-12 16:03:58.000000 bfet-0.1.9/tests/django_examples/migrations/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3208 2022-12-22 23:50:35.000000 bfet-0.1.9/tests/django_examples/models.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/test_automatic_tests/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 23:14:02.000000 bfet-0.1.9/tests/test_automatic_tests/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3375 2022-10-11 14:06:03.000000 bfet-0.1.9/tests/test_automatic_tests/test_create_tests.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/test_create_data/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-09-13 23:13:06.000000 bfet-0.1.9/tests/test_create_data/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     2043 2022-10-11 14:06:03.000000 bfet-0.1.9/tests/test_create_data/test_datacreator.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/test_testing_models/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.9/tests/test_testing_models/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-25 23:06:19.414242 bfet-0.1.9/tests/test_testing_models/test_django/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        0 2022-10-11 09:31:39.000000 bfet-0.1.9/tests/test_testing_models/test_django/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1246 2022-12-22 23:54:38.000000 bfet-0.1.9/tests/test_testing_models/test_django/test_django_model.py
```

### Comparing `bfet-0.1.8/CONTRIBUTING.rst` & `bfet-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/LICENSE` & `bfet-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/PKG-INFO` & `bfet-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Better Faster Easier Testing. Create Django models quickly and easly, create different data types for testing cases or create default tests files
 Home-page: https://github.com/lluc2397/bfet
 Author: Lucas Montes
 Author-email: lluc23@hotmail.com
 License: MIT license
 Keywords: bfet
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bfet-0.1.8/README.rst` & `bfet-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/bfet/automatic_tests/create_tests.py` & `bfet-0.1.9/bfet/automatic_tests/create_tests.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/bfet/automatic_tests/settings.py` & `bfet-0.1.9/bfet/automatic_tests/settings.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/bfet/cli.py` & `bfet-0.1.9/bfet/cli.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/bfet/create_data/constants.py` & `bfet-0.1.9/bfet/create_data/constants.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/bfet/create_data/create_data.py` & `bfet-0.1.9/bfet/create_data/create_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
 import random
 import string
 import textwrap
-from typing import Dict
+from typing import Dict, Optional
 import uuid
 
 from .constants import LIST_EMAIL_DOMAINS, LOREM_TEXT
 
 
 class DataCreator:
     @staticmethod
     def create_random_string(
-        max_value: int = 10,
+        max_value: int = 100,
         use_punctuation: bool = False,
         use_digits: bool = True,
     ) -> str:
         min_value = 10
         characters = string.ascii_letters
         if use_digits:
             characters += string.digits
@@ -28,32 +28,27 @@
 
     @staticmethod
     def create_random_text(max_value: int = 50) -> str:
         return textwrap.wrap(LOREM_TEXT, max_value)[0]
 
     @staticmethod
     def create_random_bool() -> bool:
-        return bool(random.randint(0, 1) == 1)
+        return random.randint(0, 1) == 1
 
     @staticmethod
     def create_random_json() -> Dict:
-        random_dict = {}
         choices = {
             1: DataCreator.create_random_string(),
             2: DataCreator.create_random_bool(),
-            3: DataCreator.create_random_datetime().strftime("%m/%d/%Y, %H:%M:%S"),
+            3: DataCreator.create_random_datetime().strftime(
+                "%m/%d/%Y, %H:%M:%S",
+            ),
             4: DataCreator.create_random_float(),
         }
-        for index in range(3):
-            variable_key = random.randint(1, 4)
-            variable_value = random.randint(1, 4)
-            key = choices[variable_key]
-            value = choices[variable_value]
-            random_dict[f"{key}"] = value
-        return random_dict
+        return {choices[random.randint(1, 4)]: choices[random.randint(1, 4)] for _ in range(3)}
 
     @staticmethod
     def create_random_slug(
         max_value: int = 50,
         use_digits: bool = True,
     ) -> str:
         return "-".join(
@@ -79,75 +74,99 @@
         top_level_domain = random.choice(LIST_EMAIL_DOMAINS).split(".")[-1]
         protocol = "https" if secure else "http"
         return f"{protocol}://{domain}.{top_level_domain}"
 
     @staticmethod
     def create_random_uuid(kind: int = 4, **kwargs) -> uuid.UUID:
         # TODO fix and do a better implementation
-        uuids = {1: uuid.uuid1, 3: uuid.uuid3, 4: uuid.uuid4, 5: uuid.uuid5}
+        uuids = {
+            1: uuid.uuid1,
+            3: uuid.uuid3,
+            4: uuid.uuid4,
+            5: uuid.uuid5,
+        }
         if kind == 4:
             return uuids[kind]()  # type: ignore
         if ("namespace" or "name") in kwargs:
             return uuids[kind](**kwargs)  # type: ignore
         try:
             final_uuid = uuids[kind](**kwargs)  # type: ignore
         except Exception:
             final_uuid = uuids[kind]()  # type: ignore
         return final_uuid
 
     @staticmethod
     def create_random_date(
-        day: int = None,  # type: ignore
-        month: int = None,  # type: ignore
-        year: int = None,  # type: ignore
+        day: Optional[int] = None,  # type: ignore
+        month: Optional[int] = None,  # type: ignore
+        year: Optional[int] = None,  # type: ignore
     ) -> datetime.date:
-        month = month if month else random.randint(1, 12)
+        month = month or random.randint(1, 12)
         if month == 2:
             max_day = 28
-        elif month in [1, 3, 5, 7, 8, 10, 12]:
+        elif month in {1, 3, 5, 7, 8, 10, 12}:
             max_day = 31
         else:
             max_day = 30
-        day = day if day else random.randint(1, max_day)
-        year = year if year else random.randint(1900, 2100)
-        return datetime.date(year=year, month=month, day=day)
+        day = day or random.randint(1, max_day)
+        year = year or random.randint(1900, 2100)
+        return datetime.date(
+            year=year,
+            month=month,
+            day=day,
+        )
 
     @staticmethod
     def create_random_hour(
-        hour: int = 0,
-        minute: int = 0,
-        second: int = 0,
-        microsecond: int = 0,
+        hour: Optional[int] = None,
+        minute: Optional[int] = None,
+        second: Optional[int] = None,
+        microsecond: Optional[int] = None,
         tzinfo: datetime.timezone = datetime.timezone.utc,
     ) -> datetime.time:
-        hour = hour if hour else random.randint(0, 23)
-        minute = minute if minute else random.randint(0, 59)
-        second = second if second else random.randint(0, 59)
-        return datetime.time(hour, minute, second, microsecond, tzinfo)
+        hour = hour or random.randint(0, 23)
+        minute = minute or random.randint(0, 59)
+        second = second or random.randint(0, 59)
+        microsecond = microsecond or random.randint(0, 59)
+        return datetime.time(
+            hour,
+            minute,
+            second,
+            microsecond,
+            tzinfo,
+        )
 
     @staticmethod
     def create_random_datetime(
-        day: int = 0,
-        month: int = 0,
-        year: int = 0,
-        hour: int = 0,
-        minute: int = 0,
-        second: int = 0,
-        microsecond: int = 0,
+        day: Optional[int] = None,
+        month: Optional[int] = None,
+        year: Optional[int] = None,
+        hour: Optional[int] = None,
+        minute: Optional[int] = None,
+        second: Optional[int] = None,
+        microsecond: Optional[int] = None,
         tzinfo: datetime.timezone = datetime.timezone.utc,
     ) -> datetime.datetime:
-        date = DataCreator.create_random_date(day=day, month=month, year=year)
+        date = DataCreator.create_random_date(
+            day=day,
+            month=month,
+            year=year,
+        )
         time = DataCreator.create_random_hour(
             hour=hour,
             minute=minute,
             second=second,
             microsecond=microsecond,
             tzinfo=tzinfo,
         )
-        return datetime.datetime.combine(date=date, time=time, tzinfo=tzinfo)
+        return datetime.datetime.combine(
+            date=date,
+            time=time,
+            tzinfo=tzinfo,
+        )
 
     @staticmethod
     def create_random_integer(
         min_value: int = 0,
         max_value: int = 10000000,
     ) -> int:
         if max_value < min_value:
```

### Comparing `bfet-0.1.8/bfet/testing_models/django_model.py` & `bfet-0.1.9/bfet/testing_models/django_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Dict, List, Type, Union
+from typing import Dict, List, Optional, Type, Union
 
 from ..create_data import DataCreator
 
 
 class DjangoTestingModel(DataCreator):
     def __init__(
-        self, model, quantity: int, in_bulk: bool, fill_all_fields: bool, force_create: bool
+        self,
+        model,
+        quantity: int,
+        in_bulk: bool,
+        fill_all_fields: bool,
+        force_create: bool,
     ) -> None:
         self.model = model
         self.quantity = quantity
         self.in_bulk = in_bulk
         self.fill_all_fields = fill_all_fields
         self.force_create = force_create
 
@@ -51,92 +56,92 @@
                 Fields of the model that we want to manually fill
 
         Returns
         -------
             Union[Type, List[Type]]
                 An instance or a list of instances created
         """
-        if quantity > 1:
-            if in_bulk:
-                return cls(
-                    model,
-                    quantity,
-                    in_bulk,
-                    fill_all_fields,
-                    force_create,
-                ).create_in_bulk(**kwargs)
-            else:
-                return [
-                    cls(
-                        model,
-                        quantity,
-                        in_bulk,
-                        fill_all_fields,
-                        force_create,
-                    ).create_model(**kwargs)
-                    for number in range(quantity)
-                ]
-        else:
+        if quantity == 1:
             return cls(
                 model,
                 quantity,
                 in_bulk,
                 fill_all_fields,
                 force_create,
             ).create_model(**kwargs)
+        if in_bulk:
+            return cls(
+                model,
+                quantity,
+                in_bulk,
+                fill_all_fields,
+                force_create,
+            ).create_in_bulk(**kwargs)
+        else:
+            return [
+                cls(
+                    model,
+                    quantity,
+                    in_bulk,
+                    fill_all_fields,
+                    force_create,
+                ).create_model(**kwargs)
+                for _ in range(quantity)
+            ]
 
     def get_model_manager(self) -> Type:
         try:
             manager = self.model._default_manager
         except AttributeError:
             manager = self.model.objects
-        finally:
-            return manager
+        return manager
 
     def create_in_bulk(self, **kwargs):
         pre_objects = [
-            self.model(**self.inspect_model(**kwargs)) for number in range(self.quantity)
+            self.model(
+                **self.inspect_model(**kwargs),
+            )
+            for _ in range(self.quantity)
         ]
         return self.get_model_manager().bulk_create(pre_objects)
 
     def create_model(self, **kwargs) -> Type:
         model_data = self.inspect_model(**kwargs)
         model_manager = self.get_model_manager()
         if self.force_create:
-            kwargs.update(model_data)
-            return model_manager.create(**kwargs)
+            kwargs |= model_data
+            model = model_manager.create(**kwargs)
+        elif model_manager.filter(**kwargs).exists():
+            model = model_manager.filter(**kwargs).first()
         else:
-            if model_manager.filter(**kwargs).exists():
-                return model_manager.filter(**kwargs).first()
-            else:
-                model, created = model_manager.get_or_create(**kwargs, defaults=model_data)
-                return model
+            model, created = model_manager.get_or_create(
+                **kwargs,
+                defaults=model_data,
+            )
+        return model
 
     def inspect_model(self, **kwargs) -> Dict:
-        fields_info = dict()
-        # all_model_fields = model._meta.get_fields()
+        fields_info = {}
         for field in self.model._meta.fields:
             field_name = field.name
             if field_name == "id":
                 continue
             if field_name in kwargs:
                 fields_info[field_name] = kwargs.pop(field_name)
             else:
-                if self.fill_all_fields is False:
-                    field_allow_null = field.__dict__.get("null")
-                    if field_allow_null and field_allow_null is True:
-                        fields_info.update({field_name: None})
-                        continue
+                if self.fill_all_fields is False and field.__dict__.get("null"):
+                    fields_info[field_name] = None
+                    continue
 
-                fields_info.update(self.inspect_field(field, field_name))
+                fields_info |= self.inspect_field(field, field_name)
 
         return fields_info
 
     @staticmethod
-    def set_max_value(max_length) -> int:
+    def set_max_value(max_length: Optional[int | float]) -> int:
         # TODO test
         if not max_length:
             return 5
         if max_length > 1000:
             max_length = max_length / 1000
         elif max_length > 100:
             max_length = max_length / 100
@@ -147,15 +152,20 @@
     def inspect_field(self, field: Type, field_name: str) -> Dict:
         field_type = field.get_internal_type()
         field_specs = field.__dict__
         max_length = field_specs.get("max_length")
         extra_params = {}
         if max_length:
             extra_params["max_value"] = self.set_max_value(max_length)
-        return {field_name: self.generate_random_data_per_field(field_type, extra_params)}
+        return {
+            field_name: self.generate_random_data_per_field(
+                field_type,
+                extra_params,
+            )
+        }
 
     def generate_random_data_per_field(self, field_type: str, extra_params):
         # BigIntegerField (min_value=10000)
         # PositiveBigIntegerField (min_value=10000)
         data_generator = {
             "DateTimeField": DjangoTestingModel.create_random_datetime,
             "DateField": DjangoTestingModel.create_random_date,
```

### Comparing `bfet-0.1.8/bfet.egg-info/PKG-INFO` & `bfet-0.1.9/bfet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Better Faster Easier Testing. Create Django models quickly and easly, create different data types for testing cases or create default tests files
 Home-page: https://github.com/lluc2397/bfet
 Author: Lucas Montes
 Author-email: lluc23@hotmail.com
 License: MIT license
 Keywords: bfet
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bfet-0.1.8/bfet.egg-info/SOURCES.txt` & `bfet-0.1.9/bfet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/docs/Makefile` & `bfet-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/docs/conf.py` & `bfet-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/docs/installation.rst` & `bfet-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/docs/make.bat` & `bfet-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/docs/usage.rst` & `bfet-0.1.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/setup.py` & `bfet-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,10 +50,10 @@
     include_package_data=True,
     keywords="bfet",
     name="bfet",
     packages=find_packages(include=["bfet", "bfet.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/lluc2397/bfet",
-    version="0.1.8",
+    version="0.1.9",
     zip_safe=False,
 )
```

### Comparing `bfet-0.1.8/tests/conftest.py` & `bfet-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/tests/django_examples/migrations/0001_initial.py` & `bfet-0.1.9/tests/django_examples/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/tests/django_examples/models.py` & `bfet-0.1.9/tests/django_examples/models.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/tests/test_automatic_tests/test_create_tests.py` & `bfet-0.1.9/tests/test_automatic_tests/test_create_tests.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/tests/test_create_data/test_datacreator.py` & `bfet-0.1.9/tests/test_create_data/test_datacreator.py`

 * *Files identical despite different names*

### Comparing `bfet-0.1.8/tests/test_testing_models/test_django/test_django_model.py` & `bfet-0.1.9/tests/test_testing_models/test_django/test_django_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
     def test_max_lenght(self):
         new_obj = DjangoTestingModel.create(FKTestingModel)
         assert new_obj.integer_test < 5
 
     def test_datetime(self):
         new_obj = DjangoTestingModel.create(FKTestingModel)
-        assert new_obj.datetime_test < 5
+        assert new_obj.datetime_test.day() < 5
```

