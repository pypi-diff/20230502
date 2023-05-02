# Comparing `tmp/pysailfish-1.0.0.tar.gz` & `tmp/pysailfish-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysailfish-1.0.0.tar", max compression
+gzip compressed data, was "pysailfish-1.1.0.tar", max compression
```

## Comparing `pysailfish-1.0.0.tar` & `pysailfish-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,26 @@
--rw-r--r--   0        0        0     1137 2023-05-02 01:21:34.912388 pysailfish-1.0.0/README.md
--rw-r--r--   0        0        0      290 2023-05-02 01:22:30.129028 pysailfish-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.0.0/pysailfish/__init__.py
--rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.0.0/pysailfish/app/Mainpage.dox
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.0.0/pysailfish/app/__init__.py
--rw-r--r--   0        0        0      889 2023-05-02 01:21:34.924388 pysailfish-1.0.0/pysailfish/app/main.py
--rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.0.0/pysailfish/internal/__init__.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 pysailfish-1.0.0/setup.py
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 pysailfish-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-05-02 01:21:34.912388 pysailfish-1.1.0/README.md
+-rw-r--r--   0        0        0      290 2023-05-02 01:36:22.787974 pysailfish-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.884388 pysailfish-1.1.0/pysailfish/__init__.py
+-rw-r--r--   0        0        0     7671 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/app/EAs/MA_EA.py
+-rw-r--r--   0        0        0     1213 2023-05-02 01:28:29.628493 pysailfish-1.1.0/pysailfish/app/EAs/MT4ClientEA.py
+-rw-r--r--   0        0        0      401 2023-05-02 01:21:34.912388 pysailfish-1.1.0/pysailfish/app/Mainpage.dox
+-rw-r--r--   0        0        0        0 2023-05-02 01:23:53.313928 pysailfish-1.1.0/pysailfish/app/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-02 01:28:29.628493 pysailfish-1.1.0/pysailfish/app/main.py
+-rw-r--r--   0        0        0     2088 2023-05-02 01:28:29.628493 pysailfish-1.1.0/pysailfish/app/test_tcp_client.py
+-rw-r--r--   0        0        0     3450 2023-05-02 01:28:29.628493 pysailfish-1.1.0/pysailfish/app/test_tcp_server_client.py
+-rw-r--r--   0        0        0     5805 2023-05-02 01:28:29.628493 pysailfish-1.1.0/pysailfish/internal/DataCtrl/MT4DataCtrl/MT4DataCtrl.py
+-rw-r--r--   0        0        0    26775 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/MT4_EA.py
+-rw-r--r--   0        0        0     1741 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/account_information.py
+-rw-r--r--   0        0        0     1672 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/common_functions.py
+-rw-r--r--   0        0        0     4531 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/market_info.py
+-rw-r--r--   0        0        0     9675 2023-05-02 01:24:33.698340 pysailfish-1.1.0/pysailfish/internal/MT_EA/mt4_const.py
+-rw-r--r--   0        0        0    10493 2023-05-02 01:24:33.698340 pysailfish-1.1.0/pysailfish/internal/MT_EA/mt4_fun_num_map.py
+-rw-r--r--   0        0        0    18293 2023-05-02 01:33:23.550747 pysailfish-1.1.0/pysailfish/internal/MT_EA/object_functions.py
+-rw-r--r--   0        0        0      485 2023-05-02 01:24:33.698340 pysailfish-1.1.0/pysailfish/internal/MT_EA/predefined_variables.py
+-rw-r--r--   0        0        0    25760 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/technical_indicators.py
+-rw-r--r--   0        0        0    19884 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/timeseries_and_indicators_access.py
+-rw-r--r--   0        0        0     5219 2023-05-02 01:29:21.852922 pysailfish-1.1.0/pysailfish/internal/MT_EA/trade_functions.py
+-rw-r--r--   0        0        0     4456 2023-05-02 01:24:33.698340 pysailfish-1.1.0/pysailfish/internal/Network/TCPCast.py
+-rw-r--r--   0        0        0        0 2023-05-02 01:21:34.912388 pysailfish-1.1.0/pysailfish/internal/__init__.py
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 pysailfish-1.1.0/setup.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 pysailfish-1.1.0/PKG-INFO
```

### Comparing `pysailfish-1.0.0/README.md` & `pysailfish-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pysailfish-1.0.0/setup.py` & `pysailfish-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pysailfish', 'pysailfish.app', 'pysailfish.internal']
+['pysailfish',
+ 'pysailfish.app',
+ 'pysailfish.app.EAs',
+ 'pysailfish.internal',
+ 'pysailfish.internal.DataCtrl.MT4DataCtrl',
+ 'pysailfish.internal.MT_EA',
+ 'pysailfish.internal.Network']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['sfdevtools>=1.74.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysailfish',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': '',
     'long_description': '\n## pysailfish\n\n### How to publish to pypi\n```bash\n# set up pypi token\n$ poetry config pypi-token.pypi my-token\n\n# build the project\n$ poetry build\n\n# publish the project\n$ poetry publish\n\n# DONE\n```\n\n### How to use QC CLI\n[reference](https://www.quantconnect.com/docs/v2/lean-cli)\n```bash\n# Install lean\n$ poetry add lean\n$ poetry install\n\n# Login\n$ poetry run lean login --user-id xxx --api-token xxx\n\n# Initial workspace\n$ poetry run lean init\n\n# Pull projects\n$ poetry run lean cloud pull\n\n# Push projects\n$ poetry run lean cloud push\n```\n\n### kubernetes helm related\n```bash\n# check helm template\n$ helm template pysailfish ./chart --values=./chart/values.dev.yaml\n\n# install helm chart\n$ helm upgrade --wait --timeout=1200s --install --values ./chart/values.dev.yaml pysailfish ./chart\n\n# uninstall helm chart\n$ helm uninstall pysailfish\n```\n\n### GRPC related\n[reference](https://github.com/chelseafarley/PythonGrpc)\n```bash\n# generate python script from proto file\n$ cd pysailfish/app/grpc_api\n$ poetry run python -m grpc_tools.protoc -I protos --python_out=. --grpc_python_out=. protos/pysailfish.proto\n\n$ poetry add grpcio-tools',
     'author': 'SulfredLee',
     'author_email': 'sflee1112@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pysailfish-1.0.0/PKG-INFO` & `pysailfish-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysailfish
-Version: 1.0.0
+Version: 1.1.0
 Summary: 
 Author: SulfredLee
 Author-email: sflee1112@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

