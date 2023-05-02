# Comparing `tmp/pymultigit-0.0.83.tar.gz` & `tmp/pymultigit-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultigit-0.0.83.tar", last modified: Thu Apr 27 10:32:44 2023, max compression
+gzip compressed data, was "pymultigit-0.0.84.tar", last modified: Tue May  2 11:09:05 2023, max compression
```

## Comparing `pymultigit-0.0.83.tar` & `pymultigit-0.0.84.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 10:32:44.869476 pymultigit-0.0.83/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-27 10:32:34.000000 pymultigit-0.0.83/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-04-27 10:32:44.869476 pymultigit-0.0.83/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-04-27 10:32:34.000000 pymultigit-0.0.83/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 10:32:44.869476 pymultigit-0.0.83/pymultigit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:38:18.000000 pymultigit-0.0.83/pymultigit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2662 2023-04-27 10:32:06.000000 pymultigit-0.0.83/pymultigit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     8637 2023-04-24 06:19:06.000000 pymultigit-0.0.83/pymultigit/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5084 2022-10-17 03:51:11.000000 pymultigit-0.0.83/pymultigit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      208 2023-04-27 10:32:34.000000 pymultigit-0.0.83/pymultigit/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 10:32:44.869476 pymultigit-0.0.83/pymultigit/utils/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-04-24 06:06:42.000000 pymultigit-0.0.83/pymultigit/utils/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      797 2023-04-24 06:05:04.000000 pymultigit-0.0.83/pymultigit/utils/subprocess.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-27 10:32:44.869476 pymultigit-0.0.83/pymultigit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      407 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-27 10:32:44.000000 pymultigit-0.0.83/pymultigit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-27 10:32:44.870476 pymultigit-0.0.83/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1652 2023-04-27 10:32:34.000000 pymultigit-0.0.83/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 11:09:05.913732 pymultigit-0.0.84/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-05-02 11:08:46.000000 pymultigit-0.0.84/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-05-02 11:09:05.913732 pymultigit-0.0.84/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-05-02 11:08:45.000000 pymultigit-0.0.84/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 11:09:05.913732 pymultigit-0.0.84/pymultigit/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:34:03.000000 pymultigit-0.0.84/pymultigit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2662 2023-05-02 09:28:38.000000 pymultigit-0.0.84/pymultigit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     8940 2023-05-02 11:08:19.000000 pymultigit-0.0.84/pymultigit/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5359 2023-05-02 11:04:28.000000 pymultigit-0.0.84/pymultigit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      208 2023-05-02 11:08:45.000000 pymultigit-0.0.84/pymultigit/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 11:09:05.913732 pymultigit-0.0.84/pymultigit/utils/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-05-02 09:28:38.000000 pymultigit-0.0.84/pymultigit/utils/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      797 2023-05-02 09:28:38.000000 pymultigit-0.0.84/pymultigit/utils/subprocess.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-02 11:09:05.913732 pymultigit-0.0.84/pymultigit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1411 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      407 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-05-02 11:09:05.000000 pymultigit-0.0.84/pymultigit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-05-02 11:09:05.913732 pymultigit-0.0.84/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1652 2023-05-02 11:08:45.000000 pymultigit-0.0.84/setup.py
```

### Comparing `pymultigit-0.0.83/LICENSE` & `pymultigit-0.0.84/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.83/PKG-INFO` & `pymultigit-0.0.84/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.83
+Version: 0.0.84
 Summary: Pymultigit helps you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.83
+version: 0.0.84
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.83/pymultigit/configs.py` & `pymultigit-0.0.84/pymultigit/configs.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.83/pymultigit/core.py` & `pymultigit-0.0.84/pymultigit/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,25 @@
         return
     check_call_ve([
         "pydmt",
         "build",
     ])
 
 
+def do_build_pydmt_build_venv() -> None:
+    if disable():
+        return
+    if not os.path.isfile(".pydmt.config"):
+        if ConfigOutput.print_not:
+            print("not a pydmt folder (.pydmt.config not there)")
+        return
+    args = ["pydmt", "build_venv"]
+    subprocess.check_call(args)
+
+
 def do_build_venv_make() -> None:
     if disable():
         return
     if not os.path.isfile("Makefile") or not os.path.isdir(".venv/default"):
         if ConfigOutput.print_not:
             print("not a make venv folder (either Makefile or .venv/default is not there)")
         return
```

### Comparing `pymultigit-0.0.83/pymultigit/main.py` & `pymultigit-0.0.84/pymultigit/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 import pylogconf.core
 
 
 from pymultigit.configs import ConfigDebug, ConfigGrep, ConfigMain, ConfigOutput
 from pymultigit.core import do_count, is_dirty, has_untracked_files, non_synchronized_with_upstream, \
     do_for_all_projects, do_clean, do_status, do_dirty, do_pull, do_grep, do_local_branch, \
     do_remote_branch, print_projects_that_return_data, do_github_branch, do_check_workflow_exists_for_makefile, \
-    do_build_bootstrap, do_build_pydmt, do_build_make, do_build_venv_make, do_build_venv_pydmt
+    do_build_bootstrap, do_build_pydmt, do_build_make, do_build_venv_make, do_build_venv_pydmt, \
+    do_build_pydmt_build_venv
+
 from pymultigit.static import DESCRIPTION, APP_NAME, VERSION_STR
 
 
 @register_endpoint(
     configs=[ConfigDebug],
     description="Show the status of multiple git repositories",
 )
@@ -173,14 +175,26 @@
 
 
 @register_endpoint(
     configs=[
         ConfigDebug,
         ConfigMain,
         ConfigOutput,
+    ],
+    description="create pydmt virtual env",
+)
+def build_pydmt_build_venv() -> None:
+    do_for_all_projects(do_build_pydmt_build_venv)
+
+
+@register_endpoint(
+    configs=[
+        ConfigDebug,
+        ConfigMain,
+        ConfigOutput,
     ],
     description="run pydmt build on repos, inside venv",
 )
 def build_venv_pydmt() -> None:
     do_for_all_projects(do_build_venv_pydmt)
```

### Comparing `pymultigit-0.0.83/pymultigit/utils/subprocess.py` & `pymultigit-0.0.84/pymultigit/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.83/pymultigit.egg-info/PKG-INFO` & `pymultigit-0.0.84/pymultigit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.83
+Version: 0.0.84
 Summary: Pymultigit helps you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
 Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.83
+version: 0.0.84
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.83/setup.py` & `pymultigit-0.0.84/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pymultigit",
-    version="0.0.83",
+    version="0.0.84",
     packages=[
         "pymultigit",
         "pymultigit.utils",
     ],
     # from here all is optional
     description="Pymultigit helps you deal with multiple git repositories",
     long_description=get_readme(),
```

