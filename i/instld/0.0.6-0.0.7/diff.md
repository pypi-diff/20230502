# Comparing `tmp/instld-0.0.6.tar.gz` & `tmp/instld-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instld-0.0.6.tar", last modified: Sun Apr 30 12:01:48 2023, max compression
+gzip compressed data, was "instld-0.0.7.tar", last modified: Tue May  2 10:54:59 2023, max compression
```

## Comparing `instld-0.0.6.tar` & `instld-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.033189 instld-0.0.6/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.6/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 12:01:48.032925 instld-0.0.6/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)     1445 2023-04-09 18:09:35.000000 instld-0.0.6/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.031282 instld-0.0.6/installed/
--rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.6/installed/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     1326 2023-04-29 21:56:56.000000 instld-0.0.6/installed/context_manager.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.6/installed/empty_logger.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.6/installed/errors.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      415 2023-04-29 21:55:47.000000 instld-0.0.6/installed/proxy_module.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      726 2023-04-30 11:58:19.000000 instld-0.0.6/installed/runner.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.032106 instld-0.0.6/instld.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)     2029 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      340 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-04-30 12:01:47.000000 instld-0.0.6/instld.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-30 12:01:48.033266 instld-0.0.6/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      865 2023-04-30 11:59:06.000000 instld-0.0.6/setup.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.028558 instld-0.0.6/tests/
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-30 12:01:48.032539 instld-0.0.6/tests/units/
--rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.6/tests/units/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.6/tests/units/test_errors.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-02 10:54:59.969127 instld-0.0.7/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-02 20:16:05.000000 instld-0.0.7/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9899 2023-05-02 10:54:59.968618 instld-0.0.7/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9325 2023-05-02 10:50:31.000000 instld-0.0.7/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-02 10:54:59.966004 instld-0.0.7/installed/
+-rw-r--r--   0 pomponchik   (501) staff       (20)      107 2023-04-29 15:51:00.000000 instld-0.0.7/installed/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1101 2023-05-02 05:39:10.000000 instld-0.0.7/installed/context.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1838 2023-05-02 09:21:50.000000 instld-0.0.7/installed/context_manager.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      239 2023-04-30 11:52:44.000000 instld-0.0.7/installed/empty_logger.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       50 2023-04-29 15:42:44.000000 instld-0.0.7/installed/errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       43 2023-05-01 17:48:12.000000 instld-0.0.7/installed/lock.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     4043 2023-05-02 09:00:29.000000 instld-0.0.7/installed/proxy_module.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1040 2023-05-02 09:23:26.000000 instld-0.0.7/installed/runner.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-02 10:54:59.966847 instld-0.0.7/instld.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     9899 2023-05-02 10:54:59.000000 instld-0.0.7/instld.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      440 2023-05-02 10:54:59.000000 instld-0.0.7/instld.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-05-02 10:54:59.000000 instld-0.0.7/instld.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       16 2023-05-02 10:54:59.000000 instld-0.0.7/instld.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-05-02 10:54:59.969198 instld-0.0.7/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      855 2023-05-02 09:50:03.000000 instld-0.0.7/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-02 10:54:59.961897 instld-0.0.7/tests/
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-05-02 10:54:59.968312 instld-0.0.7/tests/units/
+-rw-r--r--   0 pomponchik   (501) staff       (20)        0 2023-04-29 15:45:14.000000 instld-0.0.7/tests/units/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      217 2023-05-02 06:02:42.000000 instld-0.0.7/tests/units/test_context.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)       52 2023-04-29 15:52:00.000000 instld-0.0.7/tests/units/test_errors.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1459 2023-05-02 09:22:37.000000 instld-0.0.7/tests/units/test_proxy_module.py
```

### Comparing `instld-0.0.6/LICENSE` & `instld-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `instld-0.0.6/installed/context_manager.py` & `instld-0.0.7/installed/context_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import os
 import sys
 import tempfile
+import subprocess
 
-from threading import Lock
 from io import StringIO
 from contextlib import contextmanager
 
 from installed.errors import InstallingPackageError
+from installed.context import Context
+from installed.runner import run_python as standard_runner
+from installed.lock import lock
 
 
-lock = Lock()
-
 @contextmanager
 def search_path(base_dir, logger, runner):
     path_to_venv = os.path.join(base_dir, 'venv')
     sys_path = os.path.join(path_to_venv, 'lib')
 
-    runner(['-m', 'venv', path_to_venv], logger)
+    standard_runner(['-m', 'venv', path_to_venv], logger, True, [])
 
     for maybe_directory in os.listdir(path=sys_path):
         maybe_directory_full = os.path.join(sys_path, maybe_directory)
         if maybe_directory.startswith('python') and os.path.isdir(maybe_directory_full):
             sys_path = os.path.join(sys_path, maybe_directory, 'site-packages')
             break
 
@@ -29,17 +30,25 @@
 
     yield sys_path
 
     with lock:
         del sys.path[sys.path.index(sys_path)]
 
 @contextmanager
-def pip_context(packages_names, logger, runner):
+def pip_context(packages_names, options, logger, runner, catch_output):
     with tempfile.TemporaryDirectory() as directory:
         with search_path(directory, logger, runner) as where:
+            outputs = []
             try:
                 for package_name in packages_names:
-                    runner(['-m', 'pip', 'install', f'--target={where}', package_name], logger)
+                    runner(['-m', 'pip', 'install', f'--target={where}', *options, package_name], logger, catch_output, outputs)
             except subprocess.CalledProcessError as e:
-                raise InstallingPackageError from e
+                new_error = InstallingPackageError()
+                if len(outputs) == 2:
+                    new_error.stdout = outputs[0]
+                    new_error.stderr = outputs[1]
+                else:
+                    new_error.stdout = ''
+                    new_error.stderr = ''
+                raise new_error from e
 
-            yield
+            yield Context(where, logger)
```

### Comparing `instld-0.0.6/setup.py` & `instld-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = []
 
 setup(
     name="instld",
-    version="0.0.6",
+    version="0.0.7",
     author="Evgeniy Blinov",
     author_email="zheni-b@yandex.ru",
-    description="The simplest package management from the source code",
+    description="The simplest package management in runtime",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pomponchik/installed",
     packages=find_packages(exclude=["tests"]),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3.7",
```

