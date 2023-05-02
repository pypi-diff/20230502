# Comparing `tmp/maisaedu-poormans-dms-1.0.8.tar.gz` & `tmp/maisaedu-poormans-dms-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-poormans-dms-1.0.8.tar", last modified: Wed Nov 16 19:23:53 2022, max compression
+gzip compressed data, was "maisaedu-poormans-dms-1.0.9.tar", last modified: Wed Nov 16 19:30:53 2022, max compression
```

## Comparing `maisaedu-poormans-dms-1.0.8.tar` & `maisaedu-poormans-dms-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.943929 maisaedu-poormans-dms-1.0.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     1076 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:23:53.943929 maisaedu-poormans-dms-1.0.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.939929 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/
--rw-r--r--   0 vsts      (1001) docker     (122)    16071 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.939929 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.939929 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/
--rw-r--r--   0 vsts      (1001) docker     (122)      510 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
--rw-r--r--   0 vsts      (1001) docker     (122)      509 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
--rw-r--r--   0 vsts      (1001) docker     (122)      337 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
--rw-r--r--   0 vsts      (1001) docker     (122)      189 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2095 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Migrator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.943929 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/
--rw-r--r--   0 vsts      (1001) docker     (122)     4611 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3302 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4976 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4928 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11139 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/sql_server_migration.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:23:53.939929 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:23:53.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1192 2022-11-16 19:23:53.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:23:53.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       75 2022-11-16 19:23:53.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       22 2022-11-16 19:23:53.000000 maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:23:53.943929 maisaedu-poormans-dms-1.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2022-11-16 19:23:37.000000 maisaedu-poormans-dms-1.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.922747 maisaedu-poormans-dms-1.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1076 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.914747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16071 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/
+-rw-r--r--   0 vsts      (1001) docker     (122)      510 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      509 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      337 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      189 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2095 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Migrator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.918747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4611 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3302 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4976 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4928 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11139 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/sql_server_migration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:53.914747 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1192 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       75 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       22 2022-11-16 19:30:53.000000 maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:30:53.922747 maisaedu-poormans-dms-1.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2022-11-16 19:30:28.000000 maisaedu-poormans-dms-1.0.9/setup.py
```

### Comparing `maisaedu-poormans-dms-1.0.8/LICENSE` & `maisaedu-poormans-dms-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/__init__.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/Migrator.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/Migrator.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/postgres_migration/MigratorTable.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/postgres_migration/MigratorTable.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms/sql_server_migration.py` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms/sql_server_migration.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/maisaedu_poormans_dms.egg-info/SOURCES.txt` & `maisaedu-poormans-dms-1.0.9/maisaedu_poormans_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.0.8/setup.py` & `maisaedu-poormans-dms-1.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-poormans-dms",
-    version="1.0.8",
+    version="1.0.9",
     description="A library for making database migration tasks, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[],
     install_requires=[
```

