# Comparing `tmp/acquire-3.6.dev6.tar.gz` & `tmp/acquire-3.6.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquire-3.6.dev6.tar", last modified: Mon May  1 10:59:54 2023, max compression
+gzip compressed data, was "acquire-3.6.dev7.tar", last modified: Tue May  2 12:42:54 2023, max compression
```

## Comparing `acquire-3.6.dev6.tar` & `acquire-3.6.dev7.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-01 10:59:41.000000 acquire-3.6.dev6/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 10:59:41.000000 acquire-3.6.dev6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 10:59:41.000000 acquire-3.6.dev6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-01 10:59:54.687075 acquire-3.6.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 10:59:41.000000 acquire-3.6.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75219 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/acquire.py
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/dynamic/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/handles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/dynamic/windows/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/esxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/outputs/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/tools/decrypter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/acquire/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/uploaders/plugin_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-01 10:59:41.000000 acquire-3.6.dev6/acquire/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.683075 acquire-3.6.dev6/acquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 10:59:54.000000 acquire-3.6.dev6/acquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 10:59:44.000000 acquire-3.6.dev6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 10:59:54.687075 acquire-3.6.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:54.687075 acquire-3.6.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_acquire_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_esxi_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_file_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_minio_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-01 10:59:41.000000 acquire-3.6.dev6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-02 12:42:39.000000 acquire-3.6.dev7/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-02 12:42:39.000000 acquire-3.6.dev7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-02 12:42:39.000000 acquire-3.6.dev7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-02 12:42:54.400156 acquire-3.6.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 12:42:39.000000 acquire-3.6.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.392156 acquire-3.6.dev7/acquire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75961 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/acquire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/dynamic/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/dynamic/windows/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/esxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/outputs/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/tools/decrypter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/acquire/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/uploaders/plugin_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-02 12:42:39.000000 acquire-3.6.dev7/acquire/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.396156 acquire-3.6.dev7/acquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 12:42:54.000000 acquire-3.6.dev7/acquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 12:42:44.000000 acquire-3.6.dev7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:42:54.400156 acquire-3.6.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:54.400156 acquire-3.6.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_acquire_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_esxi_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_file_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_minio_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-02 12:42:39.000000 acquire-3.6.dev7/tox.ini
```

### Comparing `acquire-3.6.dev6/LICENSE` & `acquire-3.6.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/PKG-INFO` & `acquire-3.6.dev7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev6
+Version: 3.6.dev7
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev6/README.md` & `acquire-3.6.dev7/README.md`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/acquire.py` & `acquire-3.6.dev7/acquire/acquire.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     create_argument_parser,
     format_output_name,
     get_formatted_exception,
     get_user_name,
     get_utc_now,
     get_utc_now_str,
     is_user_admin,
+    normalize_path,
     parse_acquire_args,
     persist_execution_report,
 )
 
 try:
     from acquire.version import version
 except ImportError:
@@ -1634,21 +1635,25 @@
         log.warning("========================================== WARNING ==========================================")
 
 
 def acquire_target(target: Target, args: argparse.Namespace, output_ts: Optional[str] = None):
     output_ts = output_ts or get_utc_now_str()
     if args.log_to_dir:
         log_file = args.log_path.joinpath(format_output_name("Unknown", output_ts, "log"))
+        # This will also rename the log file on disk, which was opened in main(), if the name is different
         reconfigure_log_file(log, log_file, delay=True)
     else:
         log_file = args.log_path
 
     files = []
+    skip_list = set()
     if log_file:
         files.append(log_file)
+        if target.path.name == "local":
+            skip_list.add(normalize_path(target, log_file, resolve=True))
 
     print_disks_overview(target)
     print_volumes_overview(target)
 
     if not target._os_plugin:
         log.error("Error: Unable to detect OS")
         return files
@@ -1719,39 +1724,48 @@
         # Remove local-only modules from the modules list
         modules_selected = dict(modules_selected.items() - local_only_modules.items())
 
     log_file_handler = get_file_handler(log)
     # Prepare log file and output file names
     if log_file_handler and args.log_to_dir:
         log_file = format_output_name(target.name, output_ts, "log")
+        # This will also rename the log file on disk, which was opened and written previously.
         log_file_handler.set_filename(log_file)
-        log.info("Logging to file %s", Path(log_file_handler.baseFilename).resolve())
+        log_path = Path(log_file_handler.baseFilename).resolve()
+        log.info("Logging to file %s", log_path)
         files = [log_file_handler.baseFilename]
+        if target.path.name == "local":
+            skip_list = {normalize_path(target, log_path, resolve=True)}
 
     output_path = args.output
     if output_path.is_dir():
         output_dir = format_output_name(target.name, output_ts)
-        output_path = output_path.joinpath(output_dir).resolve()
+        output_path = output_path.joinpath(output_dir)
+    output_path = output_path.resolve()
 
     output = OUTPUTS[args.output_type](
         output_path,
         compress=args.compress,
         encrypt=args.encrypt,
         public_key=args.public_key,
     )
     files.append(output.path)
+    if target.path.name == "local":
+        skip_list.add(normalize_path(target, output.path, resolve=True))
 
     log.info("Writing output to %s", output.path)
+    if skip_list:
+        log.info("Skipping own files: %s", ", ".join(skip_list))
     log.info("")
 
     dir_base = "fs"
     if target.os != "windows":
         dir_base = "fs/$rootfs$"
 
-    with Collector(target, output, base=dir_base) as collector:
+    with Collector(target, output, base=dir_base, skip_list=skip_list) as collector:
         # Acquire specified files
         if args.file or args.directory or args.glob:
             log.info("*** Acquiring specified paths")
             spec = []
 
             if args.file:
                 for path in args.file:
```

### Comparing `acquire-3.6.dev6/acquire/collector.py` & `acquire-3.6.dev7/acquire/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     FileNotFoundError,
     NotADirectoryError,
     NotASymlinkError,
     SymlinkRecursionError,
 )
 from dissect.target.helpers import fsutil
 
-from acquire.utils import StrEnum, get_formatted_exception
+from acquire.utils import StrEnum, get_formatted_exception, normalize_path
 
 if TYPE_CHECKING:
     from acquire.outputs.base import Output
 
 log = logging.getLogger(__name__)
 
 
@@ -175,18 +175,19 @@
         return serialize_path(path) in self.seen_paths
 
 
 class Collector:
     METADATA_BASE = "$metadata$"
     COMMAND_OUTPUT_BASE = f"{METADATA_BASE}/command-output"
 
-    def __init__(self, target: Target, output: Output, base="fs"):
+    def __init__(self, target: Target, output: Output, base: str = "fs", skip_list: Optional[set] = None):
         self.target = target
         self.output = output
         self.base = base
+        self.skip_list = skip_list or set()
 
         self.report = CollectionReport()
         self.bound_module_name = None
 
         self.output.init(self.target)
 
     def __enter__(self) -> Collector:
@@ -379,14 +380,19 @@
         module_name = self.bound_module_name or module_name
         if not module_name:
             raise ValueError("Module name must be provided or Collector needs to be bound to a module")
 
         if not isinstance(path, fsutil.TargetPath):
             path = self.target.fs.path(path)
 
+        if self.skip_list and normalize_path(self.target, path) in self.skip_list:
+            self.report.add_path_failed(module_name, path)
+            log.error("- Skipping collection of %s, path is on the skip list", path)
+            return
+
         try:
             # If a path does not exist, is_dir(), is_file() and is_symlink() will return False (and not raise an
             # exception), so we need to explicitly trigger an exception for this using path.get().
             path.get()
             is_dir = path.is_dir()
             is_file = path.is_file()
             is_symlink = path.is_symlink()
```

### Comparing `acquire-3.6.dev6/acquire/crypt.py` & `acquire-3.6.dev7/acquire/crypt.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/dynamic/windows/collect.py` & `acquire-3.6.dev7/acquire/dynamic/windows/collect.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/dynamic/windows/handles.py` & `acquire-3.6.dev7/acquire/dynamic/windows/handles.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/dynamic/windows/named_objects.py` & `acquire-3.6.dev7/acquire/dynamic/windows/named_objects.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/dynamic/windows/ntdll.py` & `acquire-3.6.dev7/acquire/dynamic/windows/ntdll.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/dynamic/windows/types.py` & `acquire-3.6.dev7/acquire/dynamic/windows/types.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/esxi.py` & `acquire-3.6.dev7/acquire/esxi.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/hashes.py` & `acquire-3.6.dev7/acquire/hashes.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/log.py` & `acquire-3.6.dev7/acquire/log.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/outputs/base.py` & `acquire-3.6.dev7/acquire/outputs/base.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/outputs/dir.py` & `acquire-3.6.dev7/acquire/outputs/dir.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/outputs/tar.py` & `acquire-3.6.dev7/acquire/outputs/tar.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/tools/decrypter.py` & `acquire-3.6.dev7/acquire/tools/decrypter.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/uploaders/minio.py` & `acquire-3.6.dev7/acquire/uploaders/minio.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/uploaders/plugin.py` & `acquire-3.6.dev7/acquire/uploaders/plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/uploaders/plugin_registry.py` & `acquire-3.6.dev7/acquire/uploaders/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/acquire/utils.py` & `acquire-3.6.dev7/acquire/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import argparse
 import ctypes
 import datetime
 import getpass
 import json
 import os
+import pathlib
+import re
 import sys
 import textwrap
 import traceback
 from enum import Enum
 from io import SEEK_SET, UnsupportedOperation
 from pathlib import Path
 from stat import S_IRGRP, S_IROTH, S_IRUSR
 from typing import Any, Optional
 
+from dissect.target import Target
 from dissect.util.stream import AlignedStream
 
 from acquire.outputs import OUTPUTS
 from acquire.uploaders.plugin_registry import UploaderRegistry
 
 try:
     # Windows systems do not have the fcntl module.
@@ -388,7 +391,26 @@
         name = f"{name}.{ext}"
     return name
 
 
 def persist_execution_report(path: Path, report_data: dict) -> Path:
     with open(path, "w") as f:
         f.write(json.dumps(report_data, sort_keys=True, indent=4))
+
+
+SYSVOL_SUBST = re.compile(r"^(/\?\?/)?[cC]:")
+
+
+def normalize_path(target: Target, path: pathlib.Path, resolve: bool = False) -> str:
+    if resolve:
+        path = path.resolve()
+
+    path = path.as_posix()
+
+    if not target.fs.case_sensitive:
+        path = path.lower()
+
+    if target.os == "windows":
+        # As dissect.target always maps c: onto sysvol, we can do this substitution here.
+        path = SYSVOL_SUBST.sub("sysvol", path)
+
+    return path
```

### Comparing `acquire-3.6.dev6/acquire.egg-info/PKG-INFO` & `acquire-3.6.dev7/acquire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acquire
-Version: 3.6.dev6
+Version: 3.6.dev7
 Summary: A tool to quickly gather forensic artifacts from disk images or a live system into a lightweight container
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/acquire
 Project-URL: repository, https://github.com/fox-it/acquire
 Classifier: Programming Language :: Python :: 3
```

### Comparing `acquire-3.6.dev6/acquire.egg-info/SOURCES.txt` & `acquire-3.6.dev7/acquire.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 acquire/tools/__init__.py
 acquire/tools/decrypter.py
 acquire/uploaders/__init__.py
 acquire/uploaders/minio.py
 acquire/uploaders/plugin.py
 acquire/uploaders/plugin_registry.py
 tests/__init__.py
+tests/conftest.py
 tests/test_acquire_command.py
 tests/test_collector.py
 tests/test_esxi_memory.py
 tests/test_file_sorting.py
 tests/test_minio_uploader.py
 tests/test_plugin.py
 tests/test_utils.py
```

### Comparing `acquire-3.6.dev6/pyproject.toml` & `acquire-3.6.dev7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_acquire_command.py` & `acquire-3.6.dev7/tests/test_acquire_command.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_collector.py` & `acquire-3.6.dev7/tests/test_collector.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dissect.target import Target
 from dissect.target.exceptions import (
     FileNotFoundError,
     NotADirectoryError,
     NotASymlinkError,
     SymlinkRecursionError,
 )
-from dissect.target.filesystem import VirtualFile, VirtualFilesystem, VirtualSymlink
+from dissect.target.filesystem import VirtualFilesystem
 
 from acquire.collector import Collector
 
 
 def test_collector() -> None:
     target = Target("local")
 
@@ -33,36 +33,14 @@
         collector.collect_dir("C:", module_name="test")
         collector.collect_dir("D:", module_name="test")
 
         assert not mock_log.info.call_args.args[0] == "- Collecting file %s: Skipped (DEDUP)"
 
 
 @pytest.fixture
-def mock_file() -> Mock:
-    return Mock()
-
-
-@pytest.fixture
-def mock_fs(mock_file) -> VirtualFilesystem:
-    fs = VirtualFilesystem(case_sensitive=False)
-    fs.makedirs("/foo/bar")
-    fs.map_file_entry("/foo/bar/some-file", VirtualFile(fs, "some-file", mock_file))
-    fs.map_file_entry("/foo/bar/some-symlink", VirtualSymlink(fs, "some-symlink", "/foo/bar/some_file"))
-    return fs
-
-
-@pytest.fixture
-def mock_target(mock_fs) -> Target:
-    target = Target()
-    target.fs.mount("/", mock_fs)
-    target.filesystems.add(mock_fs)
-    return target
-
-
-@pytest.fixture
 def mock_collector(mock_target) -> Collector:
     collector = Collector(mock_target, Mock())
     return collector
 
 
 MOCK_SEEN_PATHS = set()
 MOCK_MODULE_NAME = "DUMMY"
@@ -102,41 +80,91 @@
             module_name=MOCK_MODULE_NAME,
         )
         mock_collector.collect_file.assert_called()
 
 
 def test_collector_collect_path_symlink(mock_collector) -> None:
     with patch.object(mock_collector, "collect_symlink", autospec=True):
-        mock_collector.collect_path(
-            "/foo/bar/some-symlink",
-            follow=False,
-            seen_paths=MOCK_SEEN_PATHS,
-            module_name=MOCK_MODULE_NAME,
-        )
-        mock_collector.collect_symlink.assert_called()
+        with patch.object(mock_collector, "collect_file", autospec=True):
+            mock_collector.collect_path(
+                "/foo/bar/some-symlink",
+                follow=False,
+                seen_paths=MOCK_SEEN_PATHS,
+                module_name=MOCK_MODULE_NAME,
+            )
+            mock_collector.collect_symlink.assert_called()
+            mock_collector.collect_file.assert_not_called()
 
 
 def test_collector_collect_path_symlink_follow(mock_collector) -> None:
     with patch.object(mock_collector, "collect_symlink", autospec=True):
-        mock_collector.collect_path(
+        with patch.object(mock_collector, "collect_file", autospec=True):
+            mock_collector.collect_path(
+                "/foo/bar/some-symlink",
+                follow=True,
+                seen_paths=MOCK_SEEN_PATHS,
+                module_name=MOCK_MODULE_NAME,
+            )
+            mock_collector.collect_symlink.assert_called()
+            mock_collector.collect_file.assert_called()
+
+
+@pytest.mark.parametrize(
+    "path, symlink_called, file_called",
+    [
+        (
+            "/foo/bar/own-file",
+            False,
+            False,
+        ),
+        (
+            "/foo/own-symlink",
+            True,
+            False,
+        ),
+        (
+            "/foo/bar/some-file",
+            False,
+            True,
+        ),
+        (
             "/foo/bar/some-symlink",
-            follow=True,
-            seen_paths=MOCK_SEEN_PATHS,
-            module_name=MOCK_MODULE_NAME,
-        )
-        mock_collector.collect_symlink.assert_called()
+            True,
+            True,
+        ),
+    ],
+)
+def test_collector_collect_path_skip_list(mock_collector, path, symlink_called, file_called) -> None:
+    with patch.object(mock_collector, "skip_list", new={"/foo/bar/own-file"}):
+        with patch.object(mock_collector, "collect_symlink", autospec=True):
+            with patch.object(mock_collector, "collect_file", autospec=True):
+                mock_collector.collect_path(
+                    path,
+                    follow=True,
+                    seen_paths=MOCK_SEEN_PATHS,
+                    module_name=MOCK_MODULE_NAME,
+                )
+                if symlink_called:
+                    mock_collector.collect_symlink.assert_called()
+                else:
+                    mock_collector.collect_symlink.assert_not_called()
+
+                if file_called:
+                    mock_collector.collect_file.assert_called()
+                else:
+                    mock_collector.collect_file.assert_not_called()
 
 
 def test_collector_collect_glob(mock_collector) -> None:
     with patch.object(mock_collector, "collect_file", autospec=True):
         mock_collector.collect_glob(
             "/foo/bar/*",
             module_name=MOCK_MODULE_NAME,
         )
-        mock_collector.collect_file.assert_called_once()
+        assert len(mock_collector.collect_file.mock_calls) == 3
         assert mock_collector.collect_file.call_args.kwargs.get("module_name", None) == MOCK_MODULE_NAME
 
 
 def test_collector_collect_path_non_existing_file(mock_collector) -> None:
     with patch("acquire.collector.log", autospec=True) as mock_log:
         with patch.object(mock_collector, "report", autospec=True) as mock_report:
             mock_collector.collect_path(
```

### Comparing `acquire-3.6.dev6/tests/test_esxi_memory.py` & `acquire-3.6.dev7/tests/test_esxi_memory.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_file_sorting.py` & `acquire-3.6.dev7/tests/test_file_sorting.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_minio_uploader.py` & `acquire-3.6.dev7/tests/test_minio_uploader.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_plugin.py` & `acquire-3.6.dev7/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `acquire-3.6.dev6/tests/test_utils.py` & `acquire-3.6.dev7/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import argparse
 import pathlib
 from unittest.mock import MagicMock, patch
 
 import pytest
+from dissect.target import Target
 
 from acquire.acquire import MODULES, PROFILES
 from acquire.utils import (
     check_and_set_acquire_args,
     check_and_set_log_args,
     create_argument_parser,
+    normalize_path,
 )
 
 
 def get_args(**kwargs):
     default_args = {
         "no_log": True,
         "log": None,
@@ -286,7 +288,95 @@
         "cagent_certificate": cagent_certificate,
     }
     args = get_args(config=config)
     check_and_set_acquire_args(args, MagicMock())
 
     assert args.cagent_key == cagent_key
     assert args.cagent_certificate == cagent_certificate
+
+
+@pytest.mark.parametrize(
+    "path, resolve, norm_path, case_sensitive, os",
+    [
+        (
+            pathlib.Path("/foo/bar"),
+            False,
+            "/foo/bar",
+            True,
+            "dummy",
+        ),
+        (
+            pathlib.Path("/foo/BAR"),
+            False,
+            "/foo/bar",
+            False,
+            "dummy",
+        ),
+        (
+            pathlib.Path("/foo/BAR"),
+            False,
+            "/foo/BAR",
+            True,
+            "dummy",
+        ),
+        (
+            pathlib.Path("/foo/../bar"),
+            False,
+            "/foo/../bar",
+            True,
+            "dummy",
+        ),
+        (
+            pathlib.Path("/foo/../foo/bar"),
+            True,
+            "/foo/bar",
+            True,
+            "dummy",
+        ),
+        (
+            pathlib.PureWindowsPath("c:\\foo\\bar"),
+            False,
+            "sysvol/foo/bar",
+            False,
+            "windows",
+        ),
+        (
+            pathlib.PureWindowsPath("C:\\foo\\bar"),
+            False,
+            "sysvol/foo/bar",
+            False,
+            "windows",
+        ),
+        (
+            pathlib.PureWindowsPath("\\??\\C:\\foo\\bar"),
+            False,
+            "sysvol/foo/bar",
+            False,
+            "windows",
+        ),
+        (
+            pathlib.PureWindowsPath("\\??\\c:\\foo\\bar"),
+            False,
+            "sysvol/foo/bar",
+            False,
+            "windows",
+        ),
+        (
+            pathlib.PureWindowsPath("D:\\foo\\bar"),
+            False,
+            "d:/foo/bar",
+            False,
+            "windows",
+        ),
+    ],
+)
+def test_utils_normalize_path(
+    mock_target: Target,
+    path: pathlib.Path,
+    resolve: bool,
+    norm_path: str,
+    case_sensitive: bool,
+    os: str,
+) -> None:
+    with patch.object(mock_target, "os", new=os):
+        with patch.object(mock_target.fs, "_case_sensitive", new=case_sensitive):
+            assert normalize_path(mock_target, path, resolve=resolve) == norm_path
```

### Comparing `acquire-3.6.dev6/tox.ini` & `acquire-3.6.dev7/tox.ini`

 * *Files identical despite different names*

