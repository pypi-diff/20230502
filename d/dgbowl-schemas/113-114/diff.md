# Comparing `tmp/dgbowl-schemas-113.tar.gz` & `tmp/dgbowl-schemas-114.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgbowl-schemas-113.tar", last modified: Wed Jan 11 15:43:41 2023, max compression
+gzip compressed data, was "dgbowl-schemas-114.tar", last modified: Tue May  2 11:36:35 2023, max compression
```

## Comparing `dgbowl-schemas-113.tar` & `dgbowl-schemas-114.tar`

### file list

```diff
@@ -1,87 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.878595 dgbowl-schemas-113/
--rw-rw-rw-   0        0        0       15 2023-01-11 14:35:57.000000 dgbowl-schemas-113/MANIFEST.in
--rw-rw-rw-   0        0        0     1051 2023-01-11 15:43:41.877596 dgbowl-schemas-113/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-01-11 14:35:57.000000 dgbowl-schemas-113/README.md
--rw-rw-rw-   0        0        0        5 2023-01-11 15:42:30.000000 dgbowl-schemas-113/VERSION
--rw-rw-rw-   0        0        0      108 2023-01-11 14:35:57.000000 dgbowl-schemas-113/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-11 15:43:41.879596 dgbowl-schemas-113/setup.cfg
--rw-rw-rw-   0        0        0     1412 2023-01-11 14:35:57.000000 dgbowl-schemas-113/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.665837 dgbowl-schemas-113/src/
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.703595 dgbowl-schemas-113/src/dgbowl_schemas/
--rw-rw-rw-   0        0        0      252 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.735595 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/
--rw-rw-rw-   0        0        0      713 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.751596 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/
--rw-rw-rw-   0        0        0      499 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/extract.py
--rw-rw-rw-   0        0        0      285 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/load.py
--rw-rw-rw-   0        0        0     1045 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/plot.py
--rw-rw-rw-   0        0        0      289 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/save.py
--rw-rw-rw-   0        0        0      267 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/transform.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.766595 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/
--rw-rw-rw-   0        0        0      505 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/extract.py
--rw-rw-rw-   0        0        0      285 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/load.py
--rw-rw-rw-   0        0        0     1045 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/plot.py
--rw-rw-rw-   0        0        0      289 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/save.py
--rw-rw-rw-   0        0        0      267 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_1/transform.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.768762 dgbowl-schemas-113/src/dgbowl_schemas/tomato/
--rw-rw-rw-   0        0        0      725 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.777842 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/
--rw-rw-rw-   0        0        0     1680 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/__init__.py
--rw-rw-rw-   0        0        0      125 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/method.py
--rw-rw-rw-   0        0        0      103 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/sample.py
--rw-rw-rw-   0        0        0      403 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/tomato.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.787074 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/
--rw-rw-rw-   0        0        0     2064 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/__init__.py
--rw-rw-rw-   0        0        0      464 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/method.py
--rw-rw-rw-   0        0        0      296 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/sample.py
--rw-rw-rw-   0        0        0     1085 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/tomato.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.789596 dgbowl-schemas-113/src/dgbowl_schemas/yadg/
--rw-rw-rw-   0        0        0     1485 2023-01-11 15:31:08.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.805625 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/
--rw-rw-rw-   0        0        0     1613 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/externaldate.py
--rw-rw-rw-   0        0        0     1671 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/input.py
--rw-rw-rw-   0        0        0      296 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/metadata.py
--rw-rw-rw-   0        0        0      277 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/parameters.py
--rw-rw-rw-   0        0        0     5347 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/step.py
--rw-rw-rw-   0        0        0      454 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.822596 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/
--rw-rw-rw-   0        0        0     1613 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/externaldate.py
--rw-rw-rw-   0        0        0     1671 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/input.py
--rw-rw-rw-   0        0        0      296 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/metadata.py
--rw-rw-rw-   0        0        0      277 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/parameters.py
--rw-rw-rw-   0        0        0     5347 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/step.py
--rw-rw-rw-   0        0        0      454 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.840595 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/
--rw-rw-rw-   0        0        0     1470 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/__init__.py
--rw-rw-rw-   0        0        0      884 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/externaldate.py
--rw-rw-rw-   0        0        0     1280 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/input.py
--rw-rw-rw-   0        0        0      391 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/metadata.py
--rw-rw-rw-   0        0        0      277 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/parameters.py
--rw-rw-rw-   0        0        0     4918 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/step.py
--rw-rw-rw-   0        0        0      454 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.856596 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/
--rw-rw-rw-   0        0        0     2494 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/externaldate.py
--rw-rw-rw-   0        0        0     1761 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/input.py
--rw-rw-rw-   0        0        0      766 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/metadata.py
--rw-rw-rw-   0        0        0      346 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/parameters.py
--rw-rw-rw-   0        0        0     9498 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/step.py
--rw-rw-rw-   0        0        0      742 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.874597 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/
--rw-rw-rw-   0        0        0      430 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/externaldate.py
--rw-rw-rw-   0        0        0     1761 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/input.py
--rw-rw-rw-   0        0        0      958 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/metadata.py
--rw-rw-rw-   0        0        0      298 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/parameters.py
--rw-rw-rw-   0        0        0     4485 2023-01-11 15:42:30.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/step.py
--rw-rw-rw-   0        0        0      742 2023-01-11 14:35:57.000000 dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-01-11 15:43:41.733596 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/
--rw-rw-rw-   0        0        0     1051 2023-01-11 15:43:41.000000 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3142 2023-01-11 15:43:41.000000 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 15:43:41.000000 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-01-11 15:43:41.000000 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-11 15:43:41.000000 dgbowl-schemas-113/src/dgbowl_schemas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.861713 dgbowl-schemas-114/
+-rw-rw-rw-   0        0        0       63 2023-01-27 11:04:51.000000 dgbowl-schemas-114/MANIFEST.in
+-rw-rw-rw-   0        0        0     1056 2023-05-02 11:36:35.862757 dgbowl-schemas-114/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-01-27 11:04:51.000000 dgbowl-schemas-114/README.md
+-rw-rw-rw-   0        0        0      241 2023-05-02 11:36:35.868710 dgbowl-schemas-114/setup.cfg
+-rw-rw-rw-   0        0        0     1458 2023-01-27 11:04:51.000000 dgbowl-schemas-114/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.604002 dgbowl-schemas-114/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.869715 dgbowl-schemas-114/src/dgbowl_schemas/
+-rw-rw-rw-   0        0        0      330 2023-01-27 14:53:09.000000 dgbowl-schemas-114/src/dgbowl_schemas/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-05-02 11:36:35.870710 dgbowl-schemas-114/src/dgbowl_schemas/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.699958 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/
+-rw-rw-rw-   0        0        0      605 2023-01-27 11:04:51.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.719630 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/
+-rw-rw-rw-   0        0        0      520 2023-01-27 11:04:51.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/extract.py
+-rw-rw-rw-   0        0        0      285 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/load.py
+-rw-rw-rw-   0        0        0     1045 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/plot.py
+-rw-rw-rw-   0        0        0      289 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/save.py
+-rw-rw-rw-   0        0        0      267 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.722628 dgbowl-schemas-114/src/dgbowl_schemas/tomato/
+-rw-rw-rw-   0        0        0      725 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.735627 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/
+-rw-rw-rw-   0        0        0     1680 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/method.py
+-rw-rw-rw-   0        0        0      103 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/sample.py
+-rw-rw-rw-   0        0        0      403 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/tomato.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.749625 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/
+-rw-rw-rw-   0        0        0     2064 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/__init__.py
+-rw-rw-rw-   0        0        0      464 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/method.py
+-rw-rw-rw-   0        0        0      296 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/sample.py
+-rw-rw-rw-   0        0        0     1085 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/tomato.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.752631 dgbowl-schemas-114/src/dgbowl_schemas/yadg/
+-rw-rw-rw-   0        0        0     1648 2023-02-01 14:19:22.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.776628 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/
+-rw-rw-rw-   0        0        0     1613 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/externaldate.py
+-rw-rw-rw-   0        0        0     1671 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/input.py
+-rw-rw-rw-   0        0        0      296 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/metadata.py
+-rw-rw-rw-   0        0        0      277 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/parameters.py
+-rw-rw-rw-   0        0        0     5347 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/step.py
+-rw-rw-rw-   0        0        0      454 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.798716 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/
+-rw-rw-rw-   0        0        0     1470 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/__init__.py
+-rw-rw-rw-   0        0        0      884 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/externaldate.py
+-rw-rw-rw-   0        0        0     1280 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/input.py
+-rw-rw-rw-   0        0        0      391 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/metadata.py
+-rw-rw-rw-   0        0        0      277 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/parameters.py
+-rw-rw-rw-   0        0        0     4918 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/step.py
+-rw-rw-rw-   0        0        0      454 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.819711 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/
+-rw-rw-rw-   0        0        0     2871 2023-05-02 11:35:56.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/__init__.py
+-rw-rw-rw-   0        0        0     1721 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/externaldate.py
+-rw-rw-rw-   0        0        0     1761 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/input.py
+-rw-rw-rw-   0        0        0      766 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/metadata.py
+-rw-rw-rw-   0        0        0      346 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/parameters.py
+-rw-rw-rw-   0        0        0     9498 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/step.py
+-rw-rw-rw-   0        0        0      742 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.849738 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/
+-rw-rw-rw-   0        0        0      727 2023-02-01 14:19:22.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/externaldate.py
+-rw-rw-rw-   0        0        0     3628 2023-02-03 06:27:53.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/filetype.py
+-rw-rw-rw-   0        0        0     1704 2023-01-23 15:25:09.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/input.py
+-rw-rw-rw-   0        0        0      631 2023-01-23 15:25:09.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/metadata.py
+-rw-rw-rw-   0        0        0      298 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/parameters.py
+-rw-rw-rw-   0        0        0     4408 2023-05-02 11:35:56.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/step.py
+-rw-rw-rw-   0        0        0     1183 2023-01-23 15:25:09.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/stepdefaults.py
+-rw-rw-rw-   0        0        0      742 2023-01-11 15:46:48.000000 dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.697740 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/
+-rw-rw-rw-   0        0        0     1056 2023-05-02 11:36:35.000000 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2023-05-02 11:36:35.000000 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 11:36:35.000000 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-05-02 11:36:35.000000 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 11:36:35.000000 dgbowl-schemas-114/src/dgbowl_schemas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 11:36:35.859712 dgbowl-schemas-114/tests/
+-rw-rw-rw-   0        0        0     4684 2023-02-03 06:27:53.000000 dgbowl-schemas-114/tests/test_dataschema.py
+-rw-rw-rw-   0        0        0      626 2023-01-11 15:46:48.000000 dgbowl-schemas-114/tests/test_payload.py
+-rw-rw-rw-   0        0        0     1151 2023-01-11 15:46:48.000000 dgbowl-schemas-114/tests/test_recipe.py
+-rw-rw-rw-   0        0        0    86040 2023-01-27 11:04:51.000000 dgbowl-schemas-114/versioneer.py
```

### Comparing `dgbowl-schemas-113/PKG-INFO` & `dgbowl-schemas-114/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgbowl-schemas
-Version: 113
+Version: 114
 Summary: schemas for the dgbowl suite of tools
 Home-page: https://github.com/dgbowl/dgbowl-schemas
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/dgbowl-schemas/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,11 +17,11 @@
 Provides-Extra: testing
 Provides-Extra: docs
 
 # dgbowl-schemas
 ## Schemas and validators for the `dgbowl` suite of tools.
 
 Currently implemented schemas are:
-- `recipe` validator for `dgpost` at version `{1.1, 1.0}`
+- `recipe` validator for `dgpost` at version `{2.0, 1.1, 1.0}`
 - `dataschema` validator for `yadg`, versions `{5.0, 4.2, 4.1, 4.0}`
 - `payload` validator for `tomato`  at version `{0.2, 0.1}`
```

### Comparing `dgbowl-schemas-113/setup.py` & `dgbowl-schemas-114/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import setuptools
-
-with open("VERSION", "r") as infile:
-    version = infile.read().strip()
+import versioneer
 
 with open("README.md", "r", encoding="utf-8") as infile:
     readme = infile.read()
 
 packagedir = "src"
 
 setuptools.setup(
     name="dgbowl-schemas",
-    version=version,
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     author="Peter Kraus",
     author_email="peter@tondon.de",
     description="schemas for the dgbowl suite of tools",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/dgbowl/dgbowl-schemas",
     project_urls={
@@ -27,15 +26,19 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     package_dir={"": packagedir},
     packages=setuptools.find_packages(where=packagedir),
     python_requires=">=3.8",
-    install_requires=["pydantic>=1.8", "pyyaml>=5.0"],
+    install_requires=[
+        "pydantic>=1.8",
+        "pyyaml>=5.0",
+        "tzlocal",
+    ],
     extras_require={
         "testing": ["pytest"],
         "docs": [
             "sphinx==4.5.0",
             "sphinx-rtd-theme",
             "sphinx-autodoc-typehints",
             "autodoc-pydantic",
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/dgpost/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/dgpost/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import logging
 from pydantic import ValidationError
-from .recipe_1_1 import Recipe as Recipe_1_1
 from .recipe_1_0 import Recipe as Recipe_1_0
 
 logger = logging.getLogger(__name__)
 
-latest_version = "1.1"
-Recipe = Recipe_1_1
+Recipe = Recipe_1_0
+
+models = {
+    "1.0": Recipe_1_0,
+}
 
 
 def to_recipe(**kwargs):
-    models = {
-        "1.1": Recipe_1_1,
-        "1.0": Recipe_1_0,
-    }
     firste = None
     for ver, Model in models.items():
         try:
             payload = Model(**kwargs)
             return payload
         except ValidationError as e:
             logger.info("Could not parse 'kwargs' using Recipe v%s.", ver)
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/extract.py` & `dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/extract.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/dgpost/recipe_1_0/plot.py` & `dgbowl-schemas-114/src/dgbowl_schemas/dgpost/recipe_1_0/plot.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/tomato/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/tomato/__init__.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_1/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/__init__.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/tomato/payload_0_2/tomato.py` & `dgbowl-schemas-114/src/dgbowl_schemas/tomato/payload_0_2/tomato.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from pydantic import ValidationError
 import logging
-from .dataschema_5_0 import DataSchema as DataSchema_5_0, Metadata as Metadata_5_0
+from .dataschema_5_0 import (
+    DataSchema as DataSchema_5_0,
+    Metadata as Metadata_5_0,
+    FileType as FileType_5_0,
+    ExtractorFactory as ExtractorFactory_5_0,
+)
 from .dataschema_4_2 import DataSchema as DataSchema_4_2, Metadata as Metadata_4_2
 from .dataschema_4_1 import DataSchema as DataSchema_4_1, Metadata as Metadata_4_1
 from .dataschema_4_0 import DataSchema as DataSchema_4_0, Metadata as Metadata_4_0
 
+
 logger = logging.getLogger(__name__)
 
-latest_version = "5.0"
 DataSchema = DataSchema_5_0
+Metadata = Metadata_5_0
+FileType = FileType_5_0
+ExtractorFactory = ExtractorFactory_5_0
 
 models = {
     "5.0": (DataSchema_5_0, Metadata_5_0),
     "4.2": (DataSchema_4_2, Metadata_4_2),
     "4.1": (DataSchema_4_1, Metadata_4_1),
     "4.0": (DataSchema_4_0, Metadata_4_0),
 }
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/__init__.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/externaldate.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/externaldate.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/input.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/input.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_3_1/step.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_0/step.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from pydantic import BaseModel, Extra
 from typing import Sequence
 from .metadata import Metadata
 from .step import Steps
 import logging
 
-from ..dataschema_4_1 import DataSchema as NewDataSchema
+from ..dataschema_4_2 import DataSchema as NewDataSchema
 
 logger = logging.getLogger(__name__)
 
 
 class DataSchema(BaseModel, extra=Extra.forbid):
     metadata: Metadata
     steps: Sequence[Steps]
 
     def update(self):
-        logger.info("Updating from DataSchema-4.0 to DataSchema-4.1")
+        logger.info("Updating from DataSchema-4.1 to DataSchema-4.2")
 
         nsch = {"metadata": {}, "steps": []}
         nsch["metadata"] = {
-            "version": "4.1",
+            "version": "4.2",
             "timezone": self.metadata.timezone,
-            "provenance": {
-                "type": self.metadata.provenance,
-                "metadata": {
-                    "updated-using": "dgbowl-schemas",
-                    "from": self.metadata.version,
-                },
-            },
+            "provenance": self.metadata.provenance.dict(exclude_none=True),
         }
+        if "metadata" not in nsch["metadata"]["provenance"]:
+            nsch["metadata"]["provenance"]["metadata"] = {
+                "updated-using": "dgbowl-schemas",
+                "from": self.metadata.version,
+            }
         for step in self.steps:
             nstep = {
                 "parser": step.parser,
                 "tag": step.tag,
                 "input": step.input.dict(exclude_none=True),
             }
             if step.externaldate is not None:
                 nstep["externaldate"] = step.externaldate.dict(exclude_none=True)
             if step.parameters is not None:
                 nstep["parameters"] = step.parameters.dict(exclude_none=True)
-                if "tracetype" in nstep["parameters"]:
-                    nstep["parameters"]["filetype"] = nstep["parameters"]["tracetype"]
-                    del nstep["parameters"]["tracetype"]
 
             nsch["steps"].append(nstep)
 
         return NewDataSchema(**nsch)
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_0/step.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/step.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,158 +6,163 @@
 
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 
-class Dummy(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class Dummy(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.allow):
         pass
 
     parser: Literal["dummy"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Optional[Params]
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class BasicCSV(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class BasicCSV(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
         sep: str = ","
         sigma: Optional[Mapping[str, Tol]]
         calfile: Optional[str]
         timestamp: Optional[Timestamps]
         convert: Optional[Any]
         units: Optional[Mapping[str, str]]
 
     parser: Literal["basiccsv"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class MeasCSV(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class MeasCSV(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
         timestamp: Timestamps = Field(
             Timestamp(timestamp={"index": 0, "format": "%Y-%m-%d-%H-%M-%S"})
         )
         calfile: Optional[str]
         convert: Optional[Any]
 
     parser: Literal["meascsv"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class FlowData(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class FlowData(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
-        filetype: Literal["drycal", "drycal.csv", "drycal.rtf", "drycal.txt"] = "drycal"
+        filetype: Literal["drycal.csv", "drycal.rtf", "drycal.txt"] = "drycal.csv"
         convert: Optional[Any]
         calfile: Optional[str]
 
     parser: Literal["flowdata"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class ElectroChem(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class ElectroChem(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
-        filetype: Literal["eclab.mpt", "eclab.mpr"] = "eclab.mpr"
+        filetype: Literal["eclab.mpt", "eclab.mpr", "tomato.json"] = "eclab.mpr"
 
-    class ECInput(Input):
+    class Input(Input):
         encoding: str = "windows-1252"
 
     parser: Literal["electrochem"]
-    input: ECInput = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class ChromTrace(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class ChromTrace(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
         filetype: Literal[
             "ezchrom.asc",
             "fusion.json",
             "fusion.zip",
             "agilent.ch",
             "agilent.dx",
             "agilent.csv",
-        ] = Field("ezchrom.asc", alias="tracetype")
+        ] = "ezchrom.asc"
         calfile: Optional[str]
         species: Optional[Any]
         detectors: Optional[Any]
 
     parser: Literal["chromtrace"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class MassTrace(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class MassTrace(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
-        filetype: Literal["quadstar.sac"] = Field("quadstar.sac", alias="tracetype")
+        filetype: Literal["quadstar.sac"] = "quadstar.sac"
 
     parser: Literal["masstrace"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
 class QFTrace(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
     class Params(BaseModel, extra=Extra.forbid):
-        filetype: Literal["labview.csv"] = Field("labview.csv", alias="tracetype")
+        filetype: Literal["labview.csv"] = "labview.csv"
         method: Literal["naive", "lorentz", "kajfez"] = "kajfez"
         height: float = 1.0
         distance: float = 5000.0
         cutoff: float = 0.4
         threshold: float = 1e-6
 
     parser: Literal["qftrace"]
-    input: Input = Field(alias="import")
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
-class XPSTrace(BaseModel, extra=Extra.forbid, allow_population_by_field_name=True):
+class XPSTrace(BaseModel, extra=Extra.forbid):
     class Params(BaseModel, extra=Extra.forbid):
-        filetype: Literal["phi.spe"] = Field("phi.spe", alias="tracetype")
+        filetype: Literal["phi.spe"] = "phi.spe"
 
     parser: Literal["xpstrace"]
-    input: Input = Field(alias="import")
+    input: Input
+    parameters: Params = Field(default_factory=Params)
+    tag: Optional[str]
+    externaldate: Optional[ExternalDate]
+
+
+class XRDTrace(BaseModel, extra=Extra.forbid):
+    class Params(BaseModel, extra=Extra.forbid):
+        filetype: Literal[
+            "panalytical.xy", "panalytical.csv", "panalytical.xrdml"
+        ] = "panalytical.csv"
+
+    parser: Literal["xrdtrace"]
+    input: Input
     parameters: Params = Field(default_factory=Params)
     tag: Optional[str]
     externaldate: Optional[ExternalDate]
-    export: Optional[str]
 
 
 Steps = Annotated[
     Union[
         Dummy,
         BasicCSV,
         MeasCSV,
         FlowData,
         ElectroChem,
         ChromTrace,
         MassTrace,
         QFTrace,
         XPSTrace,
+        XRDTrace,
     ],
     Field(discriminator="parser"),
 ]
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/externaldate.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/externaldate.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_1/input.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_1/input.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/__init__.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
     def update(self):
         logger.info("Updating from DataSchema-4.2 to DataSchema-5.0")
 
         nsch = {"metadata": {}, "steps": []}
         nsch["metadata"] = {
             "version": "5.0",
-            "timezone": self.metadata.timezone,
             "provenance": self.metadata.provenance.dict(exclude_none=True),
         }
+        if self.metadata.timezone is not None:
+            nsch["step_defaults"] = {"timezone": self.metadata.timezone}
         if "metadata" not in nsch["metadata"]["provenance"]:
             nsch["metadata"]["provenance"]["metadata"] = {
                 "updated-using": "dgbowl-schemas",
                 "from": self.metadata.version,
             }
         for step in self.steps:
             nstep = {
@@ -39,28 +40,34 @@
             if step.externaldate is not None:
                 nstep["externaldate"] = step.externaldate.dict(exclude_none=True)
             if step.parameters is not None:
                 nstep["parameters"] = step.parameters.dict(exclude_none=True)
             else:
                 nstep["parameters"] = {}
 
-            if "filetype" in nstep["parameters"]:
-                nstep["filetype"] = nstep["parameters"].pop("filetype")
+            extractor = {}
+            if nstep["parameters"].get("filetype", None) is not None:
+                extractor["filetype"] = nstep["parameters"].pop("filetype")
+            if nstep["input"].get("encoding", None) is not None:
+                extractor["encoding"] = nstep["input"].pop("encoding")
+            if len(extractor) > 0:
+                nstep["extractor"] = extractor
 
             for k in {
                 "sigma",
                 "calfile",
                 "convert",
                 "species",
                 "detectors",
                 "method",
                 "height",
                 "distance",
                 "cutoff",
                 "threshold",
+                "transpose",
             }:
                 if k in nstep["parameters"]:
                     logger.warning(
                         "Parameter '%s' of parser '%s' is not "
                         "supported in DataSchema-5.0.",
                         k,
                         nstep["parser"],
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/externaldate.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/externaldate.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/input.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/input.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/metadata.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/metadata.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/step.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/step.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_4_2/timestamp.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_4_2/timestamp.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/externaldate.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/externaldate.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/input.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 
     contains: Optional[str]
     """A string the matched filenames must contain."""
 
     exclude: Optional[str]
     """A string the matched filenames must not contain."""
 
-    encoding: str = "UTF-8"
-    """File encoding."""
-
     def paths(self) -> List[str]:
         """Returns a list of files to be processed by the :class:`Step`."""
         ret = []
         for item in sorted(self.files):
             if os.path.isdir(item):
                 paths = [os.path.join(item, fn) for fn in sorted(os.listdir(item))]
             else:
```

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas/yadg/dataschema_5_0/timestamp.py` & `dgbowl-schemas-114/src/dgbowl_schemas/yadg/dataschema_5_0/timestamp.py`

 * *Files identical despite different names*

### Comparing `dgbowl-schemas-113/src/dgbowl_schemas.egg-info/PKG-INFO` & `dgbowl-schemas-114/src/dgbowl_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgbowl-schemas
-Version: 113
+Version: 114
 Summary: schemas for the dgbowl suite of tools
 Home-page: https://github.com/dgbowl/dgbowl-schemas
 Author: Peter Kraus
 Author-email: peter@tondon.de
 Project-URL: Bug Tracker, https://github.com/dgbowl/dgbowl-schemas/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,11 +17,11 @@
 Provides-Extra: testing
 Provides-Extra: docs
 
 # dgbowl-schemas
 ## Schemas and validators for the `dgbowl` suite of tools.
 
 Currently implemented schemas are:
-- `recipe` validator for `dgpost` at version `{1.1, 1.0}`
+- `recipe` validator for `dgpost` at version `{2.0, 1.1, 1.0}`
 - `dataschema` validator for `yadg`, versions `{5.0, 4.2, 4.1, 4.0}`
 - `payload` validator for `tomato`  at version `{0.2, 0.1}`
```

