# Comparing `tmp/cerbos-0.5.0.tar.gz` & `tmp/cerbos-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerbos-0.5.0.tar", last modified: Tue Jan  3 15:03:24 2023, max compression
+gzip compressed data, was "cerbos-0.6.0.tar", last modified: Tue May  2 07:52:54 2023, max compression
```

## Comparing `cerbos-0.5.0.tar` & `cerbos-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-03 15:03:00.698857 cerbos-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-01-03 15:03:00.698857 cerbos-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/sdk/_async/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-01-03 15:03:23.582763 cerbos-0.5.0/cerbos/sdk/_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/sdk/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-01-03 15:03:00.698857 cerbos-0.5.0/cerbos/sdk/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-01-03 15:03:00.702857 cerbos-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/_schemas/leave_request.json
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/_schemas/principal.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/_schemas/purchase_order.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/_schemas/salary_record.json
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/derived_roles/common_roles.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/derived_roles/derived_roles_01.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/derived_roles/derived_roles_02.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/derived_roles/derived_roles_03.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/principal_policies/policy_01.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/principal_policies/policy_02.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/principal_policies/policy_02_acme.hr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/principal_policies/policy_02_acme.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_01.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_02.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_03.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_04.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_05.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.hr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/store/tests/policy_04_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16690 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-01-03 15:03:00.702857 cerbos-0.5.0/tests/test_plan_response.py
--rw-------   0 runner    (1001) docker     (123)     3438 2023-01-03 15:03:24.442761 cerbos-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 07:52:27.167645 cerbos-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2999 2023-05-02 07:52:27.167645 cerbos-0.6.0/README.md
+-rw-r--r--   0        0        0      167 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/__init__.py
+-rw-r--r--   0        0        0    12680 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/_async/client.py
+-rw-r--r--   0        0        0    12492 2023-05-02 07:52:53.752997 cerbos-0.6.0/cerbos/sdk/_sync/client.py
+-rw-r--r--   0        0        0      485 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/client.py
+-rw-r--r--   0        0        0      759 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/container.py
+-rw-r--r--   0        0        0     6262 2023-05-02 07:52:27.167645 cerbos-0.6.0/cerbos/sdk/model.py
+-rw-r--r--   0        0        0     1800 2023-05-02 07:52:27.167645 cerbos-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1303 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/check.py
+-rw-r--r--   0        0        0     2017 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      578 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/leave_request.json
+-rw-r--r--   0        0        0     1030 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/principal.json
+-rw-r--r--   0        0        0      402 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/purchase_order.json
+-rw-r--r--   0        0        0      387 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/_schemas/salary_record.json
+-rw-r--r--   0        0        0      451 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/common_roles.yaml
+-rw-r--r--   0        0        0      323 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_01.yaml
+-rw-r--r--   0        0        0      492 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_02.yaml
+-rw-r--r--   0        0        0      599 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/derived_roles/derived_roles_03.yaml
+-rw-r--r--   0        0        0      484 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_01.yaml
+-rw-r--r--   0        0        0      300 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02.yaml
+-rw-r--r--   0        0        0      226 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02_acme.hr.yaml
+-rw-r--r--   0        0        0      499 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/principal_policies/policy_02_acme.yaml
+-rw-r--r--   0        0        0     1587 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_01.yaml
+-rw-r--r--   0        0        0      624 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_02.yaml
+-rw-r--r--   0        0        0      526 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_03.yaml
+-rw-r--r--   0        0        0      689 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_04.yaml
+-rw-r--r--   0        0        0      377 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05.yaml
+-rw-r--r--   0        0        0      704 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml
+-rw-r--r--   0        0        0     1138 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.yaml
+-rw-r--r--   0        0        0      535 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.yaml
+-rw-r--r--   0        0        0      450 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/store/tests/policy_04_test.yaml
+-rw-r--r--   0        0        0    16690 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     2061 2023-05-02 07:52:27.167645 cerbos-0.6.0/tests/test_plan_response.py
+-rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 cerbos-0.6.0/PKG-INFO
```

### Comparing `cerbos-0.5.0/LICENSE` & `cerbos-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/README.md` & `cerbos-0.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 ```python
 with CerbosClient("unix+https:///var/cerbos.sock", debug=True, tls_verify=False) as c:
   ...
 ```
 
 **Testing with [TestContainers](https://github.com/testcontainers/testcontainers-python)**
 
+NOTE: Requires `cerbos[testcontainers]` dependency to be installed.
+
 ```python
 from cerbos.sdk.client import CerbosClient
 from cerbos.sdk.container import CerbosContainer
 
 container = CerbosContainer()
 policy_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "store")
 container.with_volume_mapping(policy_dir, "/policies")
```

### Comparing `cerbos-0.5.0/cerbos/sdk/_async/client.py` & `cerbos-0.6.0/cerbos/sdk/_async/client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/cerbos/sdk/_sync/client.py` & `cerbos-0.6.0/cerbos/sdk/_sync/client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/cerbos/sdk/container.py` & `cerbos-0.6.0/cerbos/sdk/container.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/cerbos/sdk/model.py` & `cerbos-0.6.0/cerbos/sdk/model.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/pyproject.toml` & `cerbos-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,38 +11,40 @@
     "Intended Audience :: Developers",
     "Topic :: Security",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
     "dataclasses-json>=0.5.7",
     "requests-toolbelt>=0.9.1",
-    "testcontainers>=3.5.3",
     "httpx[http2]>=0.22.0",
     "anyio>=3.6.1",
     "tenacity>=8.1.0",
 ]
 requires-python = ">=3.8"
 dynamic = []
-version = "0.5.0"
+version = "0.6.0"
 
 [project.urls]
 Homepage = "https://cerbos.dev"
 
 [project.optional-dependencies]
+testcontainers = [
+    "testcontainers>=3.5.3",
+]
 
 [tool.pdm.version]
 use_scm = true
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black>=22.3.0",
     "isort>=5.10.1",
 ]
 test = [
-    "pytest>=7.1.1",
+    "pytest>=7.3.1",
 ]
 tools = [
     "unasync>=0.5.0",
     "setuptools>=63.2.0",
 ]
 
 [tool.pdm.scripts.pre_build]
```

### Comparing `cerbos-0.5.0/tests/check.py` & `cerbos-0.6.0/tests/check.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/conftest.py` & `cerbos-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/_schemas/leave_request.json` & `cerbos-0.6.0/tests/store/_schemas/leave_request.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/_schemas/principal.json` & `cerbos-0.6.0/tests/store/_schemas/principal.json`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/derived_roles/derived_roles_03.yaml` & `cerbos-0.6.0/tests/store/derived_roles/derived_roles_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_01.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_01.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_02.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_02.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_03.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_03.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_04.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_04.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.uk.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.hr.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.hr.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/store/resource_policies/policy_05_acme.yaml` & `cerbos-0.6.0/tests/store/resource_policies/policy_05_acme.yaml`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/test_client.py` & `cerbos-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/tests/test_plan_response.py` & `cerbos-0.6.0/tests/test_plan_response.py`

 * *Files identical despite different names*

### Comparing `cerbos-0.5.0/PKG-INFO` & `cerbos-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: cerbos
-Version: 0.5.0
+Version: 0.6.0
 Summary: SDK for working with Cerbos: an open core, language-agnostic, scalable authorization solution
 License: Apache-2.0
 Author-email: Cerbos Developers <sdk+python@cerbos.dev>
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: testcontainers
 Project-URL: Homepage, https://cerbos.dev
 Description-Content-Type: text/markdown
 
 Cerbos Python SDK
 =================
 
 Python client for accessing [Cerbos](https://cerbos.dev).
@@ -93,14 +94,16 @@
 ```python
 with CerbosClient("unix+https:///var/cerbos.sock", debug=True, tls_verify=False) as c:
   ...
 ```
 
 **Testing with [TestContainers](https://github.com/testcontainers/testcontainers-python)**
 
+NOTE: Requires `cerbos[testcontainers]` dependency to be installed.
+
 ```python
 from cerbos.sdk.client import CerbosClient
 from cerbos.sdk.container import CerbosContainer
 
 container = CerbosContainer()
 policy_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), "store")
 container.with_volume_mapping(policy_dir, "/policies")
```

