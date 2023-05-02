# Comparing `tmp/dbt-upsolver-0.1.9.tar.gz` & `tmp/dbt-upsolver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-0.1.9.tar", last modified: Sat Apr 29 21:26:14 2023, max compression
+gzip compressed data, was "dbt-upsolver-0.2.0.tar", last modified: Tue May  2 14:39:28 2023, max compression
```

## Comparing `dbt-upsolver-0.1.9.tar` & `dbt-upsolver-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/materialized_view_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/table_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.807418 dbt-upsolver-0.1.9/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.811418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-29 21:26:14.000000 dbt-upsolver-0.1.9/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:26:14.815418 dbt-upsolver-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-29 21:26:05.000000 dbt-upsolver-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/materialized_view_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/table_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.129591 dbt-upsolver-0.2.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.133592 dbt-upsolver-0.2.0/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:28.137591 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:39:27.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 14:39:28.000000 dbt-upsolver-0.2.0/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:39:28.141591 dbt-upsolver-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-02 14:39:14.000000 dbt-upsolver-0.2.0/setup.py
```

### Comparing `dbt-upsolver-0.1.9/LICENSE` & `dbt-upsolver-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/PKG-INFO` & `dbt-upsolver-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.1.9
+Version: 0.2.0
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.1.9/README.md` & `dbt-upsolver-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/connection_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "consumer_properties": {"type": "text", "editable": True, "optional": True},
         "version": {"type": "value", "editable": False, "optional": True},
         "require_static_ip": {"type": "boolean", "editable": True, "optional": True},
         "ssl": {"type": "boolean", "editable": True, "optional": True},
         "topic_display_filter": {"type": "text", "editable": True, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     },
-    "glue_katalog": {
+    "glue_catalog": {
         "aws_role": {"type": "text", "editable": True, "optional": True},
         "external_id": {"type": "text", "editable": True, "optional": True},
         "aws_access_key_id": {"type": "text", "editable": True, "optional": True},
         "aws_secret_access_key": {"type": "text", "editable": True, "optional": True},
         "default_storage_connection": {"type": "identifier", "editable": False, "optional": False},
         "default_storage_location": {"type": "text", "editable": False, "optional": False},
         "region": {"type": "text", "editable": False, "optional": True},
```

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/table_options.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/table_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-0.2.0/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-0.2.0/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-0.2.0/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.1.9
+Version: 0.2.0
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.1.9/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-0.2.0/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.1.9/setup.py` & `dbt-upsolver-0.2.0/setup.py`

 * *Files identical despite different names*

