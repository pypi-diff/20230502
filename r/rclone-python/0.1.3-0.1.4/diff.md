# Comparing `tmp/rclone-python-0.1.3.tar.gz` & `tmp/rclone-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.3.tar", last modified: Tue Sep  6 13:43:18 2022, max compression
+gzip compressed data, was "rclone-python-0.1.4.tar", last modified: Tue May  2 16:51:38 2023, max compression
```

## Comparing `rclone-python-0.1.3.tar` & `rclone-python-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:43:18.685378 rclone-python-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-09-06 13:43:05.000000 rclone-python-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-09-06 13:43:18.685378 rclone-python-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2523 2022-09-06 13:43:05.000000 rclone-python-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:43:18.685378 rclone-python-0.1.3/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-06 13:43:05.000000 rclone-python-0.1.3/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11834 2022-09-06 13:43:05.000000 rclone-python-0.1.3/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-06 13:43:05.000000 rclone-python-0.1.3/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-09-06 13:43:05.000000 rclone-python-0.1.3/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:43:18.685378 rclone-python-0.1.3/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2970 2022-09-06 13:43:18.000000 rclone-python-0.1.3/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-09-06 13:43:18.000000 rclone-python-0.1.3/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 13:43:18.000000 rclone-python-0.1.3/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-06 13:43:18.000000 rclone-python-0.1.3/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-06 13:43:18.000000 rclone-python-0.1.3/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 13:43:18.685378 rclone-python-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-06 13:43:05.000000 rclone-python-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.092476 rclone-python-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 16:51:26.000000 rclone-python-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 16:51:38.092476 rclone-python-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-02 16:51:26.000000 rclone-python-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.088476 rclone-python-0.1.4/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-02 16:51:26.000000 rclone-python-0.1.4/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:51:38.092476 rclone-python-0.1.4/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 16:51:38.000000 rclone-python-0.1.4/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:51:38.092476 rclone-python-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-02 16:51:26.000000 rclone-python-0.1.4/setup.py
```

### Comparing `rclone-python-0.1.3/LICENSE` & `rclone-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.3/PKG-INFO` & `rclone-python-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.3/README.md` & `rclone-python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.3/rclone_python/rclone.py` & `rclone-python-0.1.4/rclone_python/rclone.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
     Purges the specified folder. This means that unlike with delete, also all the folders are removed.
     :param args: List of additional arguments/ flags.
     :param path: The path of the folder that should be purged.
     """
     if args is None:
         args = []
 
-    command = f'rclone purge {path}'
+    command = f'rclone purge "{path}"'
     process = utils.run_cmd(command, args)
     if process.returncode == 0:
         logging.info(f'Successfully purged {path}')
     else:
         raise Exception(
             f'Purging path \"{path}\" failed with error message:\n{process.stderr}')
 
@@ -167,15 +167,15 @@
     but not the folder structure itself.
     :param args: List of additional arguments/ flags.
     :param path: The path of the folder that should be deleted.
     """
     if args is None:
         args = []
 
-    command = f'rclone delete {path}'
+    command = f'rclone delete "{path}"'
     process = utils.run_cmd(command, args)
 
     if process.returncode == 0:
         logging.info(f'Successfully deleted {path}')
     else:
         raise Exception(f'Deleting path \"{path}\" failed with error message:\n{process.stderr}')
 
@@ -192,18 +192,18 @@
     :param dirs_only: If true, only dirs will be returned.
     :param args: List of additional arguments/ flags.
     :return: List of dicts containing file properties.
     """
     if args is None:
         args = []
 
-    command = f'rclone lsjson {path}'
+    command = f'rclone lsjson "{path}"'
 
     # add optional parameters
-    if max_depth:
+    if max_depth is not None:
         args.append(f"--max-depth {max_depth}")
     if dirs_only:
         args.append(f"--dirs-only")
     if files_only:
         args.append('--files-only')
 
     process = utils.run_cmd(command, args)
@@ -237,17 +237,17 @@
 
     # add global rclone flags
     if ignore_existing:
         command += ' --ignore-existing'
     command += ' --progress'
 
     # in path
-    command += f' {in_path}'
+    command += f' "{in_path}"'
     # out path
-    command += f' {out_path}'
+    command += f' "{out_path}"'
 
     # optional named arguments/flags
     command += utils.args2string(args)
 
     # execute the upload command
     process = _rclone_progress(command, prog_title, listener=listener, show_progress=show_progress)
```

### Comparing `rclone-python-0.1.3/rclone_python/utils.py` & `rclone-python-0.1.4/rclone_python/utils.py`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.3/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.4/rclone_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rclone-python-0.1.3/setup.py` & `rclone-python-0.1.4/setup.py`

 * *Files identical despite different names*

