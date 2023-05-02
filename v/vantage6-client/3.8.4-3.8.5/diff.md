# Comparing `tmp/vantage6-client-3.8.4.tar.gz` & `tmp/vantage6-client-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-3.8.4.tar", last modified: Tue Apr 25 13:31:03 2023, max compression
+gzip compressed data, was "vantage6-client-3.8.5.tar", last modified: Tue May  2 14:03:44 2023, max compression
```

## Comparing `vantage6-client-3.8.4.tar` & `vantage6-client-3.8.5.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.246178 vantage6-client-3.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.246178 vantage6-client-3.8.4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    81359 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/algorithm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/vantage6/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/dispatch_rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-04-25 13:30:46.000000 vantage6-client-3.8.4/vantage6/tools/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:31:03.250179 vantage6-client-3.8.4/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-25 13:31:03.000000 vantage6-client-3.8.4/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-25 13:31:03.000000 vantage6-client-3.8.4/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:31:03.000000 vantage6-client-3.8.4/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 13:31:03.000000 vantage6-client-3.8.4/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 13:31:03.000000 vantage6-client-3.8.4/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.775720 vantage6-client-3.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.775720 vantage6-client-3.8.5/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    81359 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/algorithm_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/vantage6/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/dispatch_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-05-02 14:03:31.000000 vantage6-client-3.8.5/vantage6/tools/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:03:44.779720 vantage6-client-3.8.5/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-02 14:03:44.000000 vantage6-client-3.8.5/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-02 14:03:44.000000 vantage6-client-3.8.5/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:03:44.000000 vantage6-client-3.8.5/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-02 14:03:44.000000 vantage6-client-3.8.5/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-02 14:03:44.000000 vantage6-client-3.8.5/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-3.8.4/PKG-INFO` & `vantage6-client-3.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.5 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.4/setup.py` & `vantage6-client-3.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/tests/test_client.py` & `vantage6-client-3.8.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/tests/test_deserialization.py` & `vantage6-client-3.8.5/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/tests/test_docker_wrapper.py` & `vantage6-client-3.8.5/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/tests/test_serialization.py` & `vantage6-client-3.8.5/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/__init__.py` & `vantage6-client-3.8.5/vantage6/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/_version.py` & `vantage6-client-3.8.5/vantage6/client/_version.py`

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

### Comparing `vantage6-client-3.8.4/vantage6/client/algorithm_client.py` & `vantage6-client-3.8.5/vantage6/client/algorithm_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/deserialization.py` & `vantage6-client-3.8.5/vantage6/client/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/filter.py` & `vantage6-client-3.8.5/vantage6/client/filter.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/serialization.py` & `vantage6-client-3.8.5/vantage6/client/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/client/utils.py` & `vantage6-client-3.8.5/vantage6/client/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/deserialization.py` & `vantage6-client-3.8.5/vantage6/tools/deserialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/dispatch_rpc.py` & `vantage6-client-3.8.5/vantage6/tools/dispatch_rpc.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/mock_client.py` & `vantage6-client-3.8.5/vantage6/tools/mock_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/serialization.py` & `vantage6-client-3.8.5/vantage6/tools/serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/util.py` & `vantage6-client-3.8.5/vantage6/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6/tools/wrapper.py` & `vantage6-client-3.8.5/vantage6/tools/wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-3.8.4/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-3.8.5/vantage6_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 3.8.4
+Version: 3.8.5
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 3.8.5 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-client-3.8.4/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-3.8.5/vantage6_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 vantage6/client/filter.py
 vantage6/client/serialization.py
 vantage6/client/utils.py
 vantage6/tools/__init__.py
 vantage6/tools/data_format.py
 vantage6/tools/deserialization.py
 vantage6/tools/dispatch_rpc.py
+vantage6/tools/docker_wrapper.py
 vantage6/tools/exceptions.py
 vantage6/tools/mock_client.py
 vantage6/tools/serialization.py
 vantage6/tools/util.py
 vantage6/tools/wrapper.py
 vantage6_client.egg-info/PKG-INFO
 vantage6_client.egg-info/SOURCES.txt
```

