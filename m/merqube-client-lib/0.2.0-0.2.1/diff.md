# Comparing `tmp/merqube_client_lib-0.2.0.tar.gz` & `tmp/merqube_client_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.2.0.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.2.1.tar", max compression
```

## Comparing `merqube_client_lib-0.2.0.tar` & `merqube_client_lib-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      207 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0    10949 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/merqube_client_lib/types.py
--rw-r--r--   0        0        0     1562 2023-05-02 19:28:24.404784 merqube_client_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0    10949 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/merqube_client_lib/types.py
+-rw-r--r--   0        0        0     1567 2023-05-02 19:34:55.877713 merqube_client_lib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 merqube_client_lib-0.2.1/PKG-INFO
```

### Comparing `merqube_client_lib-0.2.0/LICENSE` & `merqube_client_lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.0/merqube_client_lib/session.py` & `merqube_client_lib-0.2.1/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.2.0/pyproject.toml` & `merqube_client_lib-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.2.0"
+version = "0.2.1"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10,<4.0"
 requests = "*"
 pydantic = {"version" = "^1.10.5"}
 numpy = "1.24.1"
 pandas = "1.5.2"
 Flask = "2.2.2"
 Flask-Cors = "3.0.10"
 cachetools = "5.2.1"
```

