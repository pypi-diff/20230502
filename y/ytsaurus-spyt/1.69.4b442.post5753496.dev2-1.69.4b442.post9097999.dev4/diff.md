# Comparing `tmp/ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar.gz` & `tmp/ytsaurus-spyt-1.69.4b442.post9097999.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar", last modified: Tue May  2 07:20:39 2023, max compression
+gzip compressed data, was "dist/ytsaurus-spyt-1.69.4b442.post9097999.dev4.tar", last modified: Tue May  2 08:13:15 2023, max compression
```

## Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2.tar` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-discovery-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-launch-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-manage-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-shell-yt
--rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-submit-yt
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/spark-yt-submit.jar
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/__init__.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/client.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/common.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/conf.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/dependency_utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/enabler.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36917 2023-05-02 07:19:09.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/standalone.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/submit.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/types.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/utils.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-05-02 07:19:43.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/version.py
-drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/SOURCES.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/dependency_links.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/requires.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/top_level.txt
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/MANIFEST.in
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.py
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/PKG-INFO
--rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-02 07:20:39.000000 ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.cfg
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:15.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1192 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-discovery-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    11500 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-launch-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     2299 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-manage-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      760 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-shell-yt
+-rwxrw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1277 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-submit-yt
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/jars/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)  1798367 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/jars/spark-yt-submit.jar
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:15.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       95 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/__init__.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    16500 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/client.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1106 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/common.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     7357 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/conf.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      326 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/dependency_utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     3877 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/enabler.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    36987 2023-05-02 08:12:05.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/standalone.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     9779 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/submit.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     4003 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/types.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)    10300 2023-04-26 14:37:27.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/utils.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      179 2023-05-02 08:12:22.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/version.py
+drwxrwxr-x   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        0 2023-05-02 08:13:15.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      540 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        1 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       40 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/requires.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)        5 2023-05-02 08:13:14.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/top_level.txt
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      110 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/MANIFEST.in
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)     1011 2023-04-26 14:22:18.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/setup.py
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)      332 2023-05-02 08:13:15.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/PKG-INFO
+-rw-rw-r--   0 alex-shishkin (323389) dpt_yandex_infra_tech_ytdev_dep8 (246647)       38 2023-05-02 08:13:15.000000 ytsaurus-spyt-1.69.4b442.post9097999.dev4/setup.cfg
```

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-discovery-yt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-discovery-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-launch-yt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-launch-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-manage-yt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-manage-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-shell-yt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-shell-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/bin/spark-submit-yt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/bin/spark-submit-yt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/deps/jars/spark-yt-submit.jar` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/deps/jars/spark-yt-submit.jar`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/client.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/client.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/common.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/common.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/conf.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/conf.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/enabler.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/enabler.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/standalone.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/standalone.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,26 +199,26 @@
                                          permission='read', path=discovery_path, client=client)
     if permission_status.get('action', 'deny') != 'allow':
         raise RuntimeError(
             'No permission for reading cluster, actual permission status is ' + str(permission_status))
     discovery = SparkDiscovery(discovery_path=discovery_path)
 
     cluster_conf = read_cluster_conf(str(discovery.conf()), client)
-    enablers = cluster_conf['enablers']
     spark_conf = cluster_conf['spark_conf']
     dedicated_driver_op = _parse_bool(spark_conf.get('spark.dedicated_operation_mode'))
     jar_caching_enabled = _parse_bool(spark_conf.get('spark.yt.jarCaching'))
+    ipv6_preference_enabled = _parse_bool(spark_conf.get('spark.hadoop.yt.preferenceIpv6.enabled'))
 
     _add_master(discovery, spark_base_args, rest=True, client=client)
     _add_shs_option(discovery, spark_base_args, client=client)
     _add_base_spark_conf(client, discovery, spark_base_args)
     _add_spyt_deps(spyt_version, spark_base_args, discovery, client, jar_caching_enabled)
     _add_python_version(python_version, spark_base_args, client)
     _add_dedicated_driver_op_conf(spark_base_args, dedicated_driver_op)
-    _add_ipv6_preference(enablers['enable_preference_ipv6'], spark_args)
+    _add_ipv6_preference(ipv6_preference_enabled, spark_base_args)
     spark_env = _create_spark_env(client, spark_home)
 
     if local_files:
         remote_paths = {}
         new_spark_args = []
         local_files_pattern = "[A-Za-z0-9]+:\/[^,]+(,[A-Za-z0-9]+:\/[^,]+)*" # Matches "FS:/..." path sequence
         for spark_arg in spark_args:
@@ -268,16 +268,16 @@
                 "spark.pyspark.python": python_path
             }, spark_args)
         else:
             raise RuntimeError(
                 "Interpreter for python version `{}` is not found".format(python_version))
 
 
-def _add_ipv6_preference(ipv6_preference, spark_args):
-    if ipv6_preference:
+def _add_ipv6_preference(ipv6_preference_enabled, spark_args):
+    if ipv6_preference_enabled:
         _add_conf({
             'spark.driver.extraJavaOptions': '-Djava.net.preferIPv6Addresses=true',
             'spark.executor.extraJavaOptions': '-Djava.net.preferIPv6Addresses=true'
         }, spark_args)
 
 
 def wrap_cached_jar(path, jar_caching_enabled):
```

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/submit.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/submit.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/types.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/types.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/spyt/utils.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/spyt/utils.py`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/ytsaurus_spyt.egg-info/SOURCES.txt` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/ytsaurus_spyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ytsaurus-spyt-1.69.4b442.post5753496.dev2/setup.py` & `ytsaurus-spyt-1.69.4b442.post9097999.dev4/setup.py`

 * *Files identical despite different names*

