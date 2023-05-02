# Comparing `tmp/nextcode-platform-kit-1.1.6.dev4.tar.gz` & `tmp/nextcode-platform-kit-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode-platform-kit-1.1.6.dev4.tar", last modified: Fri Apr 28 14:18:12 2023, max compression
+gzip compressed data, was "nextcode-platform-kit-1.1.7.tar", last modified: Tue May  2 16:46:12 2023, max compression
```

## Comparing `nextcode-platform-kit-1.1.6.dev4.tar` & `nextcode-platform-kit-1.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.053300 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      928 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      790 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.058301 nextcode-platform-kit-1.1.6.dev4/platkit/
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-28 14:18:11.000000 nextcode-platform-kit-1.1.6.dev4/platkit/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13791 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6141 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/csautils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.058301 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8609 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/flasksetup.py
--rw-rw-rw-   0 root         (0) root         (0)     2702 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/librarypatches.py
--rw-rw-rw-   0 root         (0) root         (0)     4902 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/logsetup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.059301 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/logstash_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/middleware/reverse_proxied.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:18:12.060301 nextcode-platform-kit-1.1.6.dev4/platkit/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/models/responses.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)     5724 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/testcase.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/platkit/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 14:18:12.061301 nextcode-platform-kit-1.1.6.dev4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 14:17:40.000000 nextcode-platform-kit-1.1.6.dev4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.128226 nextcode-platform-kit-1.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      923 2023-05-02 16:46:12.128226 nextcode-platform-kit-1.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.121225 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-05-02 16:46:12.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      790 2023-05-02 16:46:12.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:46:12.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:46:11.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      204 2023-05-02 16:46:12.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-02 16:46:12.000000 nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.125226 nextcode-platform-kit-1.1.7/platkit/
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-02 16:46:11.000000 nextcode-platform-kit-1.1.7/platkit/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13791 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6141 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/csautils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.126226 nextcode-platform-kit-1.1.7/platkit/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/endpoints/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/flasksetup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/librarypatches.py
+-rw-rw-rw-   0 root         (0) root         (0)     4902 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/logsetup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.127226 nextcode-platform-kit-1.1.7/platkit/middleware/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/middleware/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/middleware/logstash_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/middleware/reverse_proxied.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:46:12.127226 nextcode-platform-kit-1.1.7/platkit/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/models/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)     5724 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/testcase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6175 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/platkit/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-02 16:46:12.128226 nextcode-platform-kit-1.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-05-02 16:45:38.000000 nextcode-platform-kit-1.1.7/setup.py
```

### Comparing `nextcode-platform-kit-1.1.6.dev4/PKG-INFO` & `nextcode-platform-kit-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev4
+Version: 1.1.7
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev4/README.md` & `nextcode-platform-kit-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/PKG-INFO` & `nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-platform-kit
-Version: 1.1.6.dev4
+Version: 1.1.7
 Summary: Flask setup packages
 Home-page: https://www.wuxinextcode.com
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `nextcode-platform-kit-1.1.6.dev4/nextcode_platform_kit.egg-info/SOURCES.txt` & `nextcode-platform-kit-1.1.7/nextcode_platform_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/auth.py` & `nextcode-platform-kit-1.1.7/platkit/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/cli.py` & `nextcode-platform-kit-1.1.7/platkit/cli.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/config.py` & `nextcode-platform-kit-1.1.7/platkit/config.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/csautils.py` & `nextcode-platform-kit-1.1.7/platkit/csautils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/endpoints/auth.py` & `nextcode-platform-kit-1.1.7/platkit/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/flasksetup.py` & `nextcode-platform-kit-1.1.7/platkit/flasksetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,16 +199,18 @@
             abort(
                 HTTPStatus.BAD_REQUEST,
                 message="You require API Major Version {} "
                 "but server has version {}. "
                 "Please upgrade your tool.".format(required_major_version, app_version),
             )
 
-    # special case for swagger documentation endpoints and prometheus metrics
+    # special case for swagger documentation endpoints and prometheus metrics and statically served files
     view = current_app.view_functions[request.endpoint]
+    if request.endpoint == "static":
+        return
     if view.__name__ in ("render_doc", "specs", "send_static_file", "prometheus_metrics"):
         return
     if hasattr(view, "view_class"):
         exempt = [f.upper() for f in getattr(view.view_class, "login_not_required", [])]
         if request.method.upper() in exempt:
             return
```

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/librarypatches.py` & `nextcode-platform-kit-1.1.7/platkit/librarypatches.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/logsetup.py` & `nextcode-platform-kit-1.1.7/platkit/logsetup.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/middleware/logstash_formatter.py` & `nextcode-platform-kit-1.1.7/platkit/middleware/logstash_formatter.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/middleware/reverse_proxied.py` & `nextcode-platform-kit-1.1.7/platkit/middleware/reverse_proxied.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/models/responses.py` & `nextcode-platform-kit-1.1.7/platkit/models/responses.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/testcase.py` & `nextcode-platform-kit-1.1.7/platkit/testcase.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/platkit/utils.py` & `nextcode-platform-kit-1.1.7/platkit/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode-platform-kit-1.1.6.dev4/setup.py` & `nextcode-platform-kit-1.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     url="https://www.wuxinextcode.com",
     description="Flask setup packages",
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     install_requires=[
         "click",
         "cryptography",
-        "Flask",
+        "Flask>=2.2.0",
         "Flask-Auth",
         "Flask-HTTPAuth",
         "flask-restx",
         "hjson",
         "logstash-formatter",
         "prometheus-flask-exporter",
         "PyJWT>=2.0.0",
```

