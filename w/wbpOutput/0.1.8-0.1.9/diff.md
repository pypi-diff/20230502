# Comparing `tmp/wbpOutput-0.1.8.tar.gz` & `tmp/wbpOutput-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpOutput-0.1.8.tar", last modified: Sun Apr 30 09:18:53 2023, max compression
+gzip compressed data, was "wbpOutput-0.1.9.tar", last modified: Tue May  2 10:25:08 2023, max compression
```

## Comparing `wbpOutput-0.1.8.tar` & `wbpOutput-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.406018 wbpOutput-0.1.8/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.408018 wbpOutput-0.1.8/Lib/wbpOutput/
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/outputwin.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/Lib/wbpOutput/preferences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1616 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 09:18:53.000000 wbpOutput-0.1.8/Lib/wbpOutput.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1616 2023-04-30 09:18:53.410019 wbpOutput-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1701 2023-04-30 09:18:53.411019 wbpOutput-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-30 09:18:51.000000 wbpOutput-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:25:08.065629 wbpOutput-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:25:08.059628 wbpOutput-0.1.9/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:25:08.063629 wbpOutput-0.1.9/Lib/wbpOutput/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/Lib/wbpOutput/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5004 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/Lib/wbpOutput/outputwin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/Lib/wbpOutput/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 10:25:08.065629 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      342 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-02 10:25:08.000000 wbpOutput-0.1.9/Lib/wbpOutput.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-05-02 10:25:08.065629 wbpOutput-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2023-05-02 10:25:08.066629 wbpOutput-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-05-02 10:25:06.000000 wbpOutput-0.1.9/setup.py
```

### Comparing `wbpOutput-0.1.8/LICENSE` & `wbpOutput-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpOutput-0.1.8/Lib/wbpOutput/outputwin.py` & `wbpOutput-0.1.9/Lib/wbpOutput/outputwin.py`

 * *Files identical despite different names*

### Comparing `wbpOutput-0.1.8/Lib/wbpOutput/preferences.py` & `wbpOutput-0.1.9/Lib/wbpOutput/preferences.py`

 * *Files identical despite different names*

### Comparing `wbpOutput-0.1.8/Lib/wbpOutput.egg-info/PKG-INFO` & `wbpOutput-0.1.9/Lib/wbpOutput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpOutput
-Version: 0.1.8
+Version: 0.1.9
 Summary: Output panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpoutput
 Author: Andreas Eigendorf
 License: MIT
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpOutput
 
 Output panel for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpOutput-0.1.8/PKG-INFO` & `wbpOutput-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpOutput
-Version: 0.1.8
+Version: 0.1.9
 Summary: Output panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpoutput
 Author: Andreas Eigendorf
 License: MIT
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.8
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpOutput
 
 Output panel for [Workbench](https://pypi.org/project/wbBase/) applications.
```

### Comparing `wbpOutput-0.1.8/setup.cfg` & `wbpOutput-0.1.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.8
+current_version = 0.1.9
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -43,40 +43,40 @@
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.8
+python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.55
+	wbBase>=0.1.56
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = output = wbpOutput
 
 [bumpversion:file:Lib/wbpOutput/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.4
+min_version = 4.5
 env_list = 
 	py38
 	py39
 	py10
 
 [testenv]
 deps = 
 	pytest
 commands = 
-	pytest
+	pytest --cov=wbpUItools --cov-report html:coverage.html
 
 [tool:pytest]
 junit_family = legacy
 testpaths = 
 	tests
 
 [egg_info]
```

