# Comparing `tmp/auterion-cli-1.0.8.tar.gz` & `tmp/auterion-cli-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.0.8.tar", last modified: Fri Apr 28 08:44:58 2023, max compression
+gzip compressed data, was "auterion-cli-1.0.9.tar", last modified: Tue May  2 10:11:33 2023, max compression
```

## Comparing `auterion-cli-1.0.8.tar` & `auterion-cli-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 08:44:58.000000 auterion-cli-1.0.8/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:44:58.877290 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:44:58.881290 auterion-cli-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 08:44:49.000000 auterion-cli-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 10:11:31.000000 auterion-cli-1.0.9/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-02 10:11:33.000000 auterion-cli-1.0.9/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 10:11:32.000000 auterion-cli-1.0.9/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.096391 auterion-cli-1.0.9/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-02 10:11:23.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-05-02 10:11:23.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8872 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3549 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:11:33.100390 auterion-cli-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-02 10:11:22.000000 auterion-cli-1.0.9/setup.py
```

### Comparing `auterion-cli-1.0.8/README.md` & `auterion-cli-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.0.9/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_command.py` & `auterion-cli-1.0.9/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,17 +161,18 @@
                     compose['services'][name]['image'] = service_config['image']
 
             # api version 1 still allows for dict update
             if 'compose-override' in meta:
                 deep_dict_update(compose, meta['compose-override'])
 
         for name, service in compose['services'].items():
+            fully_qualified_name = meta['app-author'] + '.' + meta['app-name'] + '.' + name
             if 'image' not in service:
-                service['image'] = meta['app-author'] + '.' + name + ':' + meta['app-version']
-            service['container_name'] = name
+                service['image'] = fully_qualified_name + ':' + meta['app-version']
+            service['container_name'] = fully_qualified_name
             service['platform'] = self._extract_target_platform(meta)
         return compose
 
     def _generate_image(self, compose_cmd, args, meta):
         # Generate build dir
         project_dir = args.project_dir
         build_dir = os.path.join(project_dir, 'build')
```

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.0.9/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/container_command.py` & `auterion-cli-1.0.9/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/device_command.py` & `auterion-cli-1.0.9/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/info_command.py` & `auterion-cli-1.0.9/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/report_command.py` & `auterion-cli-1.0.9/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/commands/utils.py` & `auterion-cli-1.0.9/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/main.py` & `auterion-cli-1.0.9/auterioncli/main.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/auterioncli/meta_util.py` & `auterion-cli-1.0.9/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.0.8/setup.py` & `auterion-cli-1.0.9/setup.py`

 * *Files identical despite different names*

