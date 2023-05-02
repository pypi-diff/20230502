# Comparing `tmp/ensembl-prodinf-core-2.0.5a2.tar.gz` & `tmp/ensembl-prodinf-core-2.0.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembl-prodinf-core-2.0.5a2.tar", last modified: Mon Apr 17 16:54:12 2023, max compression
+gzip compressed data, was "ensembl-prodinf-core-2.0.6a1.tar", last modified: Tue May  2 20:01:20 2023, max compression
```

## Comparing `ensembl-prodinf-core-2.0.5a2.tar` & `ensembl-prodinf-core-2.0.6a1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/
--rw-rw-rw-   0 root         (0) root         (0)    11366 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:54:12.834649 ensembl-prodinf-core-2.0.5a2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2495 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.827649 ensembl-prodinf-core-2.0.5a2/src/ensembl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.828649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.831649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/
--rw-rw-rw-   0 root         (0) root         (0)     4785 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6749 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py
--rw-rw-rw-   0 root         (0) root         (0)     3271 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py
--rw-rw-rw-   0 root         (0) root         (0)     4613 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py
--rw-rw-rw-   0 root         (0) root         (0)     4150 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3214 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/es.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.832649 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2849 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py
--rw-rw-rw-   0 root         (0) root         (0)     2517 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py
--rw-rw-rw-   0 root         (0) root         (0)    21611 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)    14102 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     5879 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3780 2023-04-17 16:53:47.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:54:12.833649 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1205 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1380 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      137 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 16:54:12.000000 ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.578914 ensembl-prodinf-core-2.0.6a1/
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-05-02 20:01:20.577914 ensembl-prodinf-core-2.0.6a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 20:01:20.578914 ensembl-prodinf-core-2.0.6a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.572914 ensembl-prodinf-core-2.0.6a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.571914 ensembl-prodinf-core-2.0.6a1/src/ensembl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.571914 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.575914 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/amqp_publishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/app_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.576914 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6749 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/datachecks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/dbcopy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/handover.py
+-rw-rw-rw-   0 root         (0) root         (0)     4150 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3214 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/db_introspects.py
+-rw-rw-rw-   0 root         (0) root         (0)     3701 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/db_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/es.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.576914 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2849 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/compara.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    21611 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/hive.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/perl_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)    14102 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/resource_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     5878 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5879 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2023-05-02 20:00:56.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 20:01:20.577914 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      137 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 20:01:20.000000 ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/top_level.txt
```

### Comparing `ensembl-prodinf-core-2.0.5a2/LICENSE` & `ensembl-prodinf-core-2.0.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/PKG-INFO` & `ensembl-prodinf-core-2.0.6a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.5a2
+Version: 2.0.6a1
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
```

### Comparing `ensembl-prodinf-core-2.0.5a2/setup.py` & `ensembl-prodinf-core-2.0.6a1/setup.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/amqp_publishing.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/amqp_publishing.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/app_logging.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/app_logging.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/datachecks.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/datachecks.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/dbcopy.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/dbcopy.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/event.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/event.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/handover.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/handover.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/clients/metadata.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/clients/metadata.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/config.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/config.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_introspects.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/db_introspects.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/db_utils.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/db_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/es.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/es.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/exceptions.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/compara.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/compara.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/core.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/core.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/models/hive.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/models/hive.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/perl_utils.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/perl_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/reporting.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/reporting.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/resource_lock.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/resource_lock.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/rest.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/rest.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,24 @@
     def _make_HTTPAdapter(self):
         retries = Retry(total=3, backoff_factor=1,
                         status_forcelist=[429, 500, 502, 503, 504],
                         allowed_methods=["GET", "PUT", "POST", "DELETE"])
         adapter = HTTPAdapter(max_retries=retries)
         return adapter
 
-    def _session(self):
+    def _session(self, use_ssl=False):
         http = requests.Session()
-        http.mount("http://", self._http_adapter)
+        if use_ssl:
+            http.mount("https://", self._http_adapter)
+        else:
+            http.mount("http://", self._http_adapter)
+        http.headers = {
+            'Accept': 'application/json',
+            'Content-Type': 'application/json'
+        }
         return http
 
     def submit_job(self, payload):
         """
         Submit a job using the supplied dict as payload. No checking is carried out on the payload
         Arguments:
           payload : job input as dict
```

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/server_utils.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/server_utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl/production/core/utils.py` & `ensembl-prodinf-core-2.0.6a1/src/ensembl/production/core/utils.py`

 * *Files identical despite different names*

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/PKG-INFO` & `ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembl-prodinf-core
-Version: 2.0.5a2
+Version: 2.0.6a1
 Summary: Ensembl Production infrastructure core package
 Home-page: https://github.com/Ensembl/ensembl-prodinf-core
 Author: Marc Chakiachvili,James Allen,Luca Da Rin Fioretto,Vinay Kaikala
 Author-email: mchakiachvili@ebi.ac.uk,jallen@ebi.ac.uk,ldrf@ebi.ac.uk,vkaikala@ebi.ac.uk
 Maintainer: Ensembl Production Team
 Maintainer-email: ensembl-production@ebi.ac.uk
 License: Apache 2.0
```

### Comparing `ensembl-prodinf-core-2.0.5a2/src/ensembl_prodinf_core.egg-info/SOURCES.txt` & `ensembl-prodinf-core-2.0.6a1/src/ensembl_prodinf_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

