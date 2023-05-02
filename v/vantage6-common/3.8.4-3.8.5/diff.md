# Comparing `tmp/vantage6-common-3.8.4.tar.gz` & `tmp/vantage6-common-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-3.8.4.tar", last modified: Tue Apr 25 13:31:02 2023, max compression
+gzip compressed data, was "vantage6-common-3.8.5.tar", last modified: Tue May  2 14:03:44 2023, max compression
```

## Comparing `vantage6-common-3.8.4.tar` & `vantage6-common-3.8.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:02.574133 vantage6-common-3.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 13:31:02.574133 vantage6-common-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:31:02.574133 vantage6-common-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:02.570133 vantage6-common-3.8.4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:02.570133 vantage6-common-3.8.4/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:02.570133 vantage6-common-3.8.4/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 13:30:46.000000 vantage6-common-3.8.4/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:02.570133 vantage6-common-3.8.4/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 13:31:02.000000 vantage6-common-3.8.4/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 13:31:02.000000 vantage6-common-3.8.4/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:31:02.000000 vantage6-common-3.8.4/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 13:31:02.000000 vantage6-common-3.8.4/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 13:31:02.000000 vantage6-common-3.8.4/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.155713 vantage6-common-3.8.5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-02 14:03:31.000000 vantage6-common-3.8.5/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.159713 vantage6-common-3.8.5/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-02 14:03:44.000000 vantage6-common-3.8.5/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 14:03:44.000000 vantage6-common-3.8.5/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:44.000000 vantage6-common-3.8.5/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-02 14:03:44.000000 vantage6-common-3.8.5/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 14:03:44.000000 vantage6-common-3.8.5/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-3.8.4/PKG-INFO` & `vantage6-common-3.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.5 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.4/setup.py` & `vantage6-common-3.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/__init__.py` & `vantage6-common-3.8.5/vantage6/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/_version.py` & `vantage6-common-3.8.5/vantage6/common/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = ((( 3, 8, 4, 'final', __build__, 0)))
+version_info = ((( 3, 8, 5, 'final', __build__, 0)))
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = f'' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = f'' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-common-3.8.4/vantage6/common/colors.py` & `vantage6-common-3.8.5/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/configuration_manager.py` & `vantage6-common-3.8.5/vantage6/common/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/context.py` & `vantage6-common-3.8.5/vantage6/common/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/docker/addons.py` & `vantage6-common-3.8.5/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/docker/network_manager.py` & `vantage6-common-3.8.5/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/encryption.py` & `vantage6-common-3.8.5/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/globals.py` & `vantage6-common-3.8.5/vantage6/common/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/task_status.py` & `vantage6-common-3.8.5/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6/common/utest.py` & `vantage6-common-3.8.5/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.8.4/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-3.8.5/vantage6_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 3.8.5 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.8.4/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-3.8.5/vantage6_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

