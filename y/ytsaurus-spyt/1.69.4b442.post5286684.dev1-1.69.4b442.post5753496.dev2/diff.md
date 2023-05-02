# Comparing `tmp/ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar.gz` & `tmp/ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar", last modified: Wed Apr 26 10:19:35 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar", last modified: Tue May  2 07:20:39 2023, max compression
```

## Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1.tar` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7434 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    35832 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-25 15:18:46.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-04-26 10:19:12.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-20 21:24:26.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-20 21:24:26.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-04-26 10:19:35.000000 ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36917 2023-05-02 07:19:09.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-05-02 07:19:43.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.cfg
```

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/client.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/common.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/conf.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,16 +62,16 @@
     if spyt_minor_version > spark_cluster_minor_version:
         logger.warning("Your SPYT library has version {} which is older than your cluster version {}. "
                        "Some new features may not work as expected. "
                        "Please update your cluster with spark-launch-yt utility".format(spyt_version, spark_cluster_version))
 
 
 def validate_mtn_config(enablers, network_project, tvm_id, tvm_secret):
-    if enablers.enable_mtn and not (network_project and tvm_id and tvm_secret):
-        raise RuntimeError("When using MTN, network_project arg, env variables SPARK_TVM_ID and SPARK_TVM_SECRET must be set.")
+    if enablers.enable_mtn and not network_project:
+        raise RuntimeError("When using MTN, network_project arg must be set.")
 
 
 def latest_compatible_spyt_version(spark_cluster_version, client=None):
     spark_cluster_minor_version = _get_spark_cluster_minor_version(spark_cluster_version)
     spyt_versions = get_available_spyt_versions(client)
     compatible_spyt_versions = [x for x in spyt_versions if _get_spyt_minor_version(x) <= spark_cluster_minor_version]
     return max(compatible_spyt_versions)
```

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/enabler.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/standalone.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/standalone.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,42 +198,58 @@
     permission_status = check_permission(user=client.get_user_name(),
                                          permission='read', path=discovery_path, client=client)
     if permission_status.get('action', 'deny') != 'allow':
         raise RuntimeError(
             'No permission for reading cluster, actual permission status is ' + str(permission_status))
     discovery = SparkDiscovery(discovery_path=discovery_path)
 
-    spark_conf = read_cluster_conf(str(discovery.conf()), client)['spark_conf']
+    cluster_conf = read_cluster_conf(str(discovery.conf()), client)
+    enablers = cluster_conf['enablers']
+    spark_conf = cluster_conf['spark_conf']
     dedicated_driver_op = _parse_bool(spark_conf.get('spark.dedicated_operation_mode'))
     jar_caching_enabled = _parse_bool(spark_conf.get('spark.yt.jarCaching'))
 
     _add_master(discovery, spark_base_args, rest=True, client=client)
     _add_shs_option(discovery, spark_base_args, client=client)
     _add_base_spark_conf(client, discovery, spark_base_args)
     _add_spyt_deps(spyt_version, spark_base_args, discovery, client, jar_caching_enabled)
     _add_python_version(python_version, spark_base_args, client)
     _add_dedicated_driver_op_conf(spark_base_args, dedicated_driver_op)
+    _add_ipv6_preference(enablers['enable_preference_ipv6'], spark_args)
     spark_env = _create_spark_env(client, spark_home)
 
     if local_files:
         remote_paths = {}
         new_spark_args = []
+        local_files_pattern = "[A-Za-z0-9]+:\/[^,]+(,[A-Za-z0-9]+:\/[^,]+)*" # Matches "FS:/..." path sequence
         for spark_arg in spark_args:
-            if spark_arg.startswith('local:/'):
-                if spark_arg not in remote_paths:
-                    file_path = spark_arg[7:] # Drops prefix
-                    _, file_extension = os.path.splitext(file_path)
-                    destination = upload_file_to_cache(file_path, client=client)
-                    destination_ext = "{}{}".format(destination, file_extension)
-                    cypress_copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
-                    logger.info("%s has been uploaded to YT as %s", file_path, destination_ext)
-                    remote_paths[spark_arg] = "yt:/{}".format(destination_ext)
-                new_spark_args.append(remote_paths[spark_arg])
-            else:
+            is_file_list = re.fullmatch(local_files_pattern, spark_arg)
+            if not is_file_list:
                 new_spark_args.append(spark_arg)
+                continue
+            file_list = spark_arg.split(",")
+            new_file_list = []
+            for single_file in file_list:
+                if single_file.startswith('local:/'):
+                    local_file_path = single_file[7:] # Drops prefix
+                    if local_file_path not in remote_paths:
+                        _, file_extension = os.path.splitext(local_file_path)
+                        destination = upload_file_to_cache(local_file_path, client=client)
+                        destination_ext = "{}{}".format(destination, file_extension)
+                        if file_extension != "":
+                            cypress_copy(destination, destination_ext, ignore_existing=True, client=client) # Extension is necessary
+                        else:
+                            logger.warn("%s has no extension. Usually such files are unacceptable")
+                        logger.info("%s has been uploaded to YT as %s", local_file_path, destination_ext)
+                        remote_paths[local_file_path] = "yt:/{}".format(destination_ext)
+                    new_file_list.append(remote_paths[local_file_path])
+                else:
+                    new_file_list.append(single_file)
+            new_spark_arg = ",".join(new_file_list)
+            new_spark_args.append(new_spark_arg)
         spark_args = new_spark_args
 
     # replace stdin to avoid https://bugs.openjdk.java.net/browse/JDK-8211842
     return subprocess.call(spark_base_args + spark_args, env=spark_env, stdin=subprocess.PIPE)
 
 
 def _add_dedicated_driver_op_conf(spark_args, dedicated_driver_op):
@@ -252,14 +268,22 @@
                 "spark.pyspark.python": python_path
             }, spark_args)
         else:
             raise RuntimeError(
                 "Interpreter for python version `{}` is not found".format(python_version))
 
 
+def _add_ipv6_preference(ipv6_preference, spark_args):
+    if ipv6_preference:
+        _add_conf({
+            'spark.driver.extraJavaOptions': '-Djava.net.preferIPv6Addresses=true',
+            'spark.executor.extraJavaOptions': '-Djava.net.preferIPv6Addresses=true'
+        }, spark_args)
+
+
 def wrap_cached_jar(path, jar_caching_enabled):
     if jar_caching_enabled and path.startswith("yt:/"):
         return "ytCached:/" + path[4:]
     else:
         return path
 
 
@@ -326,34 +350,32 @@
         spark_home = "."
     else:
         spark_home = "./tmpfs"
 
     def script_path(script):
         return "{}/{}".format(spark_home, driver_op_discovery_script)
 
-    def _launcher_command(component, xmx="512m", additional_java_opts=None):
-        additional_java_opts = additional_java_opts or []
+    def _launcher_command(component, xmx="512m", extra_java_opts=None):
         create_dir = "mkdir -p {}".format(spark_home)
         unpack_tar = "tar --warning=no-unknown-keyword -xf spark.tgz -C {}".format(
             spark_home)
         move_java = "cp -r /opt/jdk11 ./tmpfs/jdk11"
-        run_launcher = "./tmpfs/jdk11/bin/java -Xmx{0} -cp spark-yt-launcher.jar {1}".format(
-            xmx, " ".join(additional_java_opts))
+        extra_java_opts_str = " " + " ".join(extra_java_opts) if extra_java_opts else ""
+        run_launcher = "./tmpfs/jdk11/bin/java -Xmx{0} -cp spark-yt-launcher.jar{1}".format(
+            xmx, extra_java_opts_str)
         spark_conf = get_spark_conf(config=config, enablers=enablers)
 
         return "{5} && {0} && {1} && {2} {3} tech.ytsaurus.spark.launcher.{4}Launcher ".format(
             unpack_tar, move_java, run_launcher, spark_conf, component, create_dir)
 
-    additional_java_opts = []
+    extra_java_opts = []
     if enablers.enable_preference_ipv6:
-        additional_java_opts.append("-Djava.net.preferIPv6Addresses=true")
-        config["spark_conf"]["spark.driver.extraJavaOptions"] = "-Djava.net.preferIPv6Addresses=true"
-        config["spark_conf"]["spark.executor.extraJavaOptions"] = "-Djava.net.preferIPv6Addresses=true"
+        extra_java_opts.append("-Djava.net.preferIPv6Addresses=true")
 
-    master_command = _launcher_command("Master", additional_java_opts=additional_java_opts)
+    master_command = _launcher_command("Master", extra_java_opts=extra_java_opts)
 
     def _script_absolute_path(script):
         return "{}/{}".format(spark_home, script)
 
     worker_log_location = "yt:/{}".format(spark_discovery.worker_log())
     if "spark.workerLog.tablePath" not in config["spark_conf"]:
         config["spark_conf"]["spark.workerLog.tablePath"] = worker_log_location
@@ -369,30 +391,30 @@
     if autoscaler_enabled:
         config["spark_conf"]["spark.worker.resource.jobid.amount"] = "1"
         config["spark_conf"]["spark.worker.resource.jobid.discoveryScript"] = _script_absolute_path(
             "spark/bin/job-id-discovery.sh")
         config["spark_conf"]["spark.driver.resource.jobid.discoveryScript"] = _script_absolute_path(
             "spark/bin/job-id-discovery.sh")
 
-    worker_command = _launcher_command("Worker", "2g", additional_java_opts=additional_java_opts) + \
+    worker_command = _launcher_command("Worker", "2g", extra_java_opts=extra_java_opts) + \
         "--cores {0} --memory {1} --wait-master-timeout {2} --wlog-service-enabled {3} " \
         "--wlog-enable-json {4} --wlog-update-interval {5} --wlog-table-path {6} " \
         "--wlog-table-ttl {7}".format(
             worker.cores, worker.memory, worker.timeout, worker_log_transfer, worker_log_json_mode,
             worker_log_update_interval, worker_log_location, worker_log_table_ttl)
 
     if advanced_event_log:
         event_log_path = "ytEventLog:/{}".format(
             shs_location or spark_discovery.event_log_table())
     else:
         event_log_path = "yt:/{}".format(
             shs_location or spark_discovery.event_log())
     if "spark.history.fs.numReplayThreads" not in config["spark_conf"]:
         config["spark_conf"]["spark.history.fs.numReplayThreads"] = history_server_cpu_limit
-    history_command = _launcher_command("HistoryServer", additional_java_opts=additional_java_opts) + \
+    history_command = _launcher_command("HistoryServer", extra_java_opts=extra_java_opts) + \
         "--log-path {} --memory {}".format(event_log_path,
                                            history_server_memory_limit)
 
     user = get_user_name(client=client)
 
     operation_spec = config["operation_spec"]
 
@@ -434,30 +456,31 @@
     environment["SPARK_HOME"] = "$HOME/{}/spark".format(spark_home)
     environment["SPARK_CLUSTER_VERSION"] = config["cluster_version"]
     environment["SPARK_YT_CLUSTER_CONF_PATH"] = str(spark_discovery.conf())
     environment["SPARK_YT_BYOP_PORT"] = "27002"
     environment["SPARK_LOCAL_DIRS"] = "./tmpfs"
     environment["SPARK_YT_SOLOMON_ENABLED"] = str(enablers.enable_solomon_agent)
     environment["SOLOMON_PUSH_PORT"] = "27099"
+    environment["SPARK_YT_IPV6_PREFERENCE_ENABLED"] = str(enablers.enable_preference_ipv6)
 
     ytserver_proxy_path = config.get("ytserver_proxy_path")
 
+    tvm_enabled = enablers.enable_mtn and bool(tvm_id) and bool(tvm_secret)
     worker_environment = {
-        "SPARK_YT_BYOP_ENABLED": str(enablers.enable_byop),
-        "SPARK_YT_IPV6_PREFERENCE_ENABLED": str(enablers.enable_preference_ipv6)
+        "SPARK_YT_BYOP_ENABLED": str(enablers.enable_byop)
     }
     worker_environment = update(environment, worker_environment)
     if enablers.enable_byop:
         ytserver_binary_name = ytserver_proxy_path.split(
             "/")[-1] if ytserver_proxy_path else "ytserver-proxy"
         byop_worker_environment = {
             "SPARK_YT_BYOP_BINARY_PATH": "$HOME/{}".format(ytserver_binary_name),
             "SPARK_YT_BYOP_CONFIG_PATH": "$HOME/ytserver-proxy.template.yson",
             "SPARK_YT_BYOP_HOST": "localhost",
-            "SPARK_YT_BYOP_TVM_ENABLED": str(enablers.enable_mtn)
+            "SPARK_YT_BYOP_TVM_ENABLED": str(tvm_enabled)
         }
         worker_environment = update(worker_environment, byop_worker_environment)
 
     if enablers.enable_byop:
         worker_cores_overhead = worker.cores_overhead or SparkDefaultArguments.SPARK_WORKER_CORES_BYOP_OVERHEAD
     else:
         worker_cores_overhead = worker.cores_overhead or SparkDefaultArguments.SPARK_WORKER_CORES_OVERHEAD
@@ -482,14 +505,15 @@
         worker_file_paths.append("//home/sashbel/profiler.zip")
         shs_file_paths.append("//home/sashbel/profiler.zip")
 
     secure_vault = {"YT_USER": user, "YT_TOKEN": get_token(client=client)}
 
     if enablers.enable_mtn:
         common_task_spec["network_project"] = network_project
+    if tvm_enabled:
         secure_vault["SPARK_TVM_ID"] = tvm_id
         secure_vault["SPARK_TVM_SECRET"] = tvm_secret
 
     worker_task_spec = copy.deepcopy(common_task_spec)
     worker_task_spec["environment"] = worker_environment
     if ssd_limit:
         worker_task_spec["disk_request"] = {
```

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/submit.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/types.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/spyt/utils.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5286684.dev1/setup.py` & `ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.py`

 * *Files identical despite different names*

