# Comparing `tmp/crc_jupyter_auth-1.0.4.tar.gz` & `tmp/crc_jupyter_auth-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc_jupyter_auth-1.0.4.tar", max compression
+gzip compressed data, was "crc_jupyter_auth-1.0.5.tar", max compression
```

## Comparing `crc_jupyter_auth-1.0.4.tar` & `crc_jupyter_auth-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34893 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/LICENSE.md
--rw-r--r--   0        0        0     4465 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/README.md
--rw-r--r--   0        0        0      170 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/crc_jupyter_auth/__init__.py
--rw-r--r--   0        0        0     6358 2023-04-14 16:50:49.714533 crc_jupyter_auth-1.0.4/crc_jupyter_auth/remote_user_auth.py
--rw-r--r--   0        0        0     1184 2023-04-14 16:51:07.638801 crc_jupyter_auth-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 crc_jupyter_auth-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34893 2023-05-02 19:40:04.394895 crc_jupyter_auth-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0     4465 2023-05-02 19:40:04.394895 crc_jupyter_auth-1.0.5/README.md
+-rw-r--r--   0        0        0      170 2023-05-02 19:40:04.394895 crc_jupyter_auth-1.0.5/crc_jupyter_auth/__init__.py
+-rw-r--r--   0        0        0     6398 2023-05-02 19:40:04.394895 crc_jupyter_auth-1.0.5/crc_jupyter_auth/remote_user_auth.py
+-rw-r--r--   0        0        0     1282 2023-05-02 19:40:04.782897 crc_jupyter_auth-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5839 1970-01-01 00:00:00.000000 crc_jupyter_auth-1.0.5/PKG-INFO
```

### Comparing `crc_jupyter_auth-1.0.4/LICENSE.md` & `crc_jupyter_auth-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crc_jupyter_auth-1.0.4/README.md` & `crc_jupyter_auth-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `crc_jupyter_auth-1.0.4/crc_jupyter_auth/remote_user_auth.py` & `crc_jupyter_auth-1.0.5/crc_jupyter_auth/remote_user_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
         Raises:
             NotImplementedError: Every time the method is called
         """
 
         # User account authentication is expected to be handled upstream
         # before the request reaches this class
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
 
 
 class RemoteUserLocalAuthenticator(AuthenticatorSettings, LocalAuthenticator):
     """Base class for authenticators that work with local Linux/UNIX users
 
     This class is similar to the ``RemoteUserAuthenticator`` class except it
     can check for local user accounts and attempt to create them if they don't
@@ -179,8 +179,8 @@
 
         Raises:
             NotImplementedError: Every time the method is called
         """
 
         # User account authentication is expected to be handled upstream
         # before the request reaches this class
-        raise NotImplementedError()
+        raise NotImplementedError()  # pragma: no cover
```

### Comparing `crc_jupyter_auth-1.0.4/pyproject.toml` & `crc_jupyter_auth-1.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crc_jupyter_auth"
-version = "1.0.4"  # Version is set dynamically by the CI tool on publication
+version = "1.0.5"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 license = "GPL-3.0-only"
 readme = "README.md"
 description = "Jupyter authentication plugin that checks for account existence and VPN roles."
 homepage = "https://github.com/pitt-crc/Jupyter-Authenticator"
 repository = "https://github.com/pitt-crc/Jupyter-Authenticator"
 documentation = "https://github.com/pitt-crc/Jupyter-Authenticator"
@@ -26,7 +26,13 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 jupyterhub = "*"
 tornado = "*"
 traitlets = "*"
+
+[tool.poetry.group.tests]
+optional = true
+
+[tool.poetry.group.tests.dependencies]
+coverage = "*"
```

### Comparing `crc_jupyter_auth-1.0.4/PKG-INFO` & `crc_jupyter_auth-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-jupyter-auth
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jupyter authentication plugin that checks for account existence and VPN roles.
 Home-page: https://github.com/pitt-crc/Jupyter-Authenticator
 License: GPL-3.0-only
 Keywords: Pitt,CRC,Jupyter,JupyterHub,JupyterLab,Authentication
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.7
 Classifier: Framework :: Jupyter
```

