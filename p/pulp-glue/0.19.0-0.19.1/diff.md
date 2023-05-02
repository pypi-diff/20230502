# Comparing `tmp/pulp-glue-0.19.0.tar.gz` & `tmp/pulp-glue-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.19.0.tar", last modified: Fri Apr 14 15:26:02 2023, max compression
+gzip compressed data, was "pulp-glue-0.19.1.tar", last modified: Tue May  2 20:10:31 2023, max compression
```

## Comparing `pulp-glue-0.19.0.tar` & `pulp-glue-0.19.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/certguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/certguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/context.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:26:02.512465 pulp-glue-0.19.0/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:26:02.000000 pulp-glue-0.19.0/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:26:02.516465 pulp-glue-0.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 15:25:50.000000 pulp-glue-0.19.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.016944 pulp-glue-0.19.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 20:10:31.016944 pulp-glue-0.19.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.004944 pulp-glue-0.19.1/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.008944 pulp-glue-0.19.1/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/ansible/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.008944 pulp-glue-0.19.1/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/certguard/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.012944 pulp-glue-0.19.1/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/common/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.012944 pulp-glue-0.19.1/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/container/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.012944 pulp-glue-0.19.1/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.012944 pulp-glue-0.19.1/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/file/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.016944 pulp-glue-0.19.1/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/python/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.016944 pulp-glue-0.19.1/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/rpm/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:10:31.008944 pulp-glue-0.19.1/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 20:10:30.000000 pulp-glue-0.19.1/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-02 20:10:30.000000 pulp-glue-0.19.1/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:10:30.000000 pulp-glue-0.19.1/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-02 20:10:30.000000 pulp-glue-0.19.1/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 20:10:30.000000 pulp-glue-0.19.1/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:10:31.016944 pulp-glue-0.19.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-02 20:10:18.000000 pulp-glue-0.19.1/setup.py
```

### Comparing `pulp-glue-0.19.0/PKG-INFO` & `pulp-glue-0.19.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.19.0
+Version: 0.19.1
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.19.0/pulp_glue/ansible/context.py` & `pulp-glue-0.19.1/pulp_glue/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/certguard/context.py` & `pulp-glue-0.19.1/pulp_glue/certguard/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/common/context.py` & `pulp-glue-0.19.1/pulp_glue/common/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/common/i18n.py` & `pulp-glue-0.19.1/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/common/openapi.py` & `pulp-glue-0.19.1/pulp_glue/common/openapi.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/container/context.py` & `pulp-glue-0.19.1/pulp_glue/container/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/core/context.py` & `pulp-glue-0.19.1/pulp_glue/core/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/file/context.py` & `pulp-glue-0.19.1/pulp_glue/file/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/python/context.py` & `pulp-glue-0.19.1/pulp_glue/python/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue/rpm/context.py` & `pulp-glue-0.19.1/pulp_glue/rpm/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.19.1/pulp_glue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.19.0
+Version: 0.19.1
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Home-page: https://github.com/pulp/pulp-cli
 Author: Pulp Team
 Author-email: pulp-list@redhat.com
 License: GPLv2+
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-0.19.0/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.19.1/pulp_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.19.0/setup.py` & `pulp-glue-0.19.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     name="pulp-glue",
     description="Version agnostic glue library to talk to pulpcore's REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Pulp Team",
     author_email="pulp-list@redhat.com",
     url="https://github.com/pulp/pulp-cli",
-    version="0.19.0",
+    version="0.19.1",
     packages=plugin_packages,
     package_data={"": ["py.typed"]},
     python_requires=">=3.6",
     install_requires=[
         "packaging",
         "setuptools",
         "requests~=2.24",
```

