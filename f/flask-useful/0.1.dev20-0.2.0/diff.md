# Comparing `tmp/flask-useful-0.1.dev20.tar.gz` & `tmp/flask-useful-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-useful-0.1.dev20.tar", last modified: Fri Aug  6 11:31:21 2021, max compression
+gzip compressed data, was "flask-useful-0.2.0.tar", last modified: Tue May  2 16:20:15 2023, max compression
```

## Comparing `flask-useful-0.1.dev20.tar` & `flask-useful-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,46 @@
-drwxr-xr-x   0 kyzima-spb  (1000) kyzima-spb  (1000)        0 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)        5 2020-09-17 15:17:24.000000 flask-useful-0.1.dev20/.gitignore
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     1082 2020-07-22 17:56:33.000000 flask-useful-0.1.dev20/LICENSE
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      642 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/PKG-INFO
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)        0 2020-07-22 17:56:51.000000 flask-useful-0.1.dev20/README.rst
-drwxr-xr-x   0 kyzima-spb  (1000) kyzima-spb  (1000)        0 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/flask_useful/
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     2315 2021-04-06 13:51:43.000000 flask-useful-0.1.dev20/flask_useful/__init__.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      382 2020-07-25 19:44:45.000000 flask-useful-0.1.dev20/flask_useful/decorators.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     1582 2020-08-09 15:45:53.000000 flask-useful-0.1.dev20/flask_useful/flask_access.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     1329 2020-08-08 18:44:41.000000 flask-useful-0.1.dev20/flask_useful/sqla.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     3418 2021-08-06 11:18:00.000000 flask-useful-0.1.dev20/flask_useful/utils.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     5622 2021-08-06 11:21:27.000000 flask-useful-0.1.dev20/flask_useful/views.py
-drwxr-xr-x   0 kyzima-spb  (1000) kyzima-spb  (1000)        0 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/flask_useful/wtforms/
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)       26 2020-07-23 15:28:48.000000 flask-useful-0.1.dev20/flask_useful/wtforms/__init__.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     2865 2020-09-17 15:14:53.000000 flask-useful-0.1.dev20/flask_useful/wtforms/fields.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      311 2020-07-23 15:28:48.000000 flask-useful-0.1.dev20/flask_useful/wtforms/filters.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     2326 2021-02-27 22:15:31.000000 flask-useful-0.1.dev20/flask_useful/wtforms/validators.py
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      745 2020-09-17 15:12:58.000000 flask-useful-0.1.dev20/flask_useful/wtforms/widgets.py
-drwxr-xr-x   0 kyzima-spb  (1000) kyzima-spb  (1000)        0 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/flask_useful.egg-info/
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      642 2021-08-06 11:31:21.000000 flask-useful-0.1.dev20/flask_useful.egg-info/PKG-INFO
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)      526 2021-08-06 11:31:21.000000 flask-useful-0.1.dev20/flask_useful.egg-info/SOURCES.txt
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)        1 2021-08-06 11:31:21.000000 flask-useful-0.1.dev20/flask_useful.egg-info/dependency_links.txt
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)       11 2021-08-06 11:31:21.000000 flask-useful-0.1.dev20/flask_useful.egg-info/requires.txt
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)       13 2021-08-06 11:31:21.000000 flask-useful-0.1.dev20/flask_useful.egg-info/top_level.txt
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)       38 2021-08-06 11:31:21.439751 flask-useful-0.1.dev20/setup.cfg
--rw-r--r--   0 kyzima-spb  (1000) kyzima-spb  (1000)     1122 2020-09-17 15:20:47.000000 flask-useful-0.1.dev20/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.000060 flask-useful-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.000060 flask-useful-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.github/workflows/publish-stable.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.github/workflows/publish-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:20:03.000000 flask-useful-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 16:20:03.000000 flask-useful-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 16:20:15.004060 flask-useful-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 16:20:03.000000 flask-useful-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v1/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/examples/blueprints/routes/api/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/api/v2/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-02 16:20:03.000000 flask-useful-0.2.0/examples/blueprints/routes/docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/flask_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/sqla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful/wtforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-02 16:20:03.000000 flask-useful-0.2.0/flask_useful/wtforms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:20:15.004060 flask-useful-0.2.0/flask_useful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-02 16:20:15.000000 flask-useful-0.2.0/flask_useful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 16:20:14.000000 flask-useful-0.2.0/flask_useful.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-02 16:20:03.000000 flask-useful-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:20:15.004060 flask-useful-0.2.0/setup.cfg
```

### Comparing `flask-useful-0.1.dev20/LICENSE` & `flask-useful-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful/__init__.py` & `flask-useful-0.2.0/flask_useful/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,99 @@
-import inspect
+"""
+The module contains functions for automating the configuration of the application object.
+"""
 
+from __future__ import annotations
+
+import typing as t
+
+from flask import Blueprint, Flask
 from flask.cli import AppGroup
 from werkzeug.utils import find_modules, import_string
 
 
 __all__ = (
-    'register_blueprints', 'register_commands', 'register_extensions',
+    'register_blueprints',
+    'register_commands',
+    'register_extensions',
 )
 
 
-def get_import_prefix(app):
+AppOrBp = t.Union[Flask, Blueprint]
+
+
+def get_import_prefix(app: AppOrBp) -> str:
     if app.import_name == '__main__':
         return ''
     return f'{app.import_name}.'
 
 
-def register_blueprints(app, import_path, recursive=False):
-    """Registers Blueprint for the specified application.
+def get_import_path(app: AppOrBp, import_path: str) -> str:
+    """Returns the absolute path to import a module or package."""
+    prefix = get_import_prefix(app)
+    return (prefix + import_path).strip('.')
+
+
+def register_blueprints(
+    app: AppOrBp,
+    import_path: str,
+    recursive: bool = False,
+    include_packages: bool = False,
+) -> None:
+    """
+    Registers Blueprint for the specified application.
 
     The argument `import_path` must be a valid import name for the package that contains the modules.
     One module - one Blueprint.
     The variable named `bp` must contain an instance of Blueprint.
 
     If the `BLUEPRINT_DISABLED` attribute is set in the module, then Blueprint will be ignored.
     """
-    for name in find_modules(get_import_prefix(app) + import_path, recursive=recursive):
+    modules_names = list(find_modules(
+        get_import_path(app, import_path),
+        recursive=recursive,
+        include_packages=include_packages,
+    ))
+
+    for name in modules_names:
         mod = import_string(name)
 
         if hasattr(mod, 'bp') and not getattr(mod.bp, 'BLUEPRINT_DISABLED', False):
-            app.register_blueprint(mod.bp)
-
-            for url_prefix in getattr(mod.bp, 'BLUEPRINT_URL_PREFIXES', []):
-                app.register_blueprint(mod.bp, url_prefix=url_prefix)
+            if isinstance(mod.bp, Blueprint):
+                app.register_blueprint(mod.bp)
 
 
-def register_commands(app, import_name):
+def register_commands(app: Flask, import_name: str) -> None:
     """Initializes console commands found at the specified import path.
 
     If the __all__ attribute is specified in the module,
     it will be used to fund commands.
     Otherwise, the search is performed using the `dir` function.
 
     Command is an object inherited from `flask.cli.AppGroup`.
     """
-    m = import_string(get_import_prefix(app) + import_name)
+    m = import_string(get_import_path(app, import_name))
 
     for name in getattr(m, '__all__', dir(m)):
         prop = getattr(m, name)
 
         if isinstance(prop, AppGroup):
             app.cli.add_command(prop)
 
 
-def register_extensions(app, import_name):
+def register_extensions(app: Flask, import_name: str) -> None:
     """Initializes all Flask extensions found in the specified import path.
 
     If the __all__ attribute is specified in the module,
     it will be used to search for extension instances.
     Otherwise, the search is performed using the `dir` function.
 
     An extension is an object that has an init_app method.
     """
-    m = import_string(get_import_prefix(app) + import_name)
+    m = import_string(get_import_path(app, import_name))
 
     for name in getattr(m, '__all__', dir(m)):
         prop = getattr(m, name)
         init_app = getattr(prop, 'init_app', None)
 
         if callable(init_app):
             init_app(app)
```

### Comparing `flask-useful-0.1.dev20/flask_useful/flask_access.py` & `flask-useful-0.2.0/flask_useful/flask_access.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful/utils.py` & `flask-useful-0.2.0/flask_useful/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+from __future__ import annotations
+
 import re
+import typing as t
+
 from flask import (
     current_app,
     redirect,
     url_for,
     request,
     flash as _flash
 )
@@ -10,15 +14,15 @@
 
 __all__ = (
     'camel_to_list', 'camel_to_snake', 'snake_to_camel',
     'get_route_param_names', 'make_redirect', 'flash',
 )
 
 
-def camel_to_list(s: str, lower: bool = False) -> list[str]:
+def camel_to_list(s: str, lower: bool = False) -> t.List[str]:
     """Converts a camelcase string to a list."""
     lst = re.findall(r'([A-Z][a-z0-9]+)', s) or [s]
     return [w.lower() for w in lst] if lower else lst
 
 
 def camel_to_snake(name: str) -> str:
     """Converts a camelcase string to a snake case string."""
```

### Comparing `flask-useful-0.1.dev20/flask_useful/views.py` & `flask-useful-0.2.0/flask_useful/views.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful/wtforms/fields.py` & `flask-useful-0.2.0/flask_useful/wtforms/fields.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful/wtforms/validators.py` & `flask-useful-0.2.0/flask_useful/wtforms/validators.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful/wtforms/widgets.py` & `flask-useful-0.2.0/flask_useful/wtforms/widgets.py`

 * *Files identical despite different names*

### Comparing `flask-useful-0.1.dev20/flask_useful.egg-info/SOURCES.txt` & `flask-useful-0.2.0/flask_useful.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 .gitignore
 LICENSE
 README.rst
-setup.py
+pyproject.toml
+.github/workflows/publish-stable.yml
+.github/workflows/publish-test.yml
+examples/README.rst
+examples/blueprints/__init__.py
+examples/blueprints/routes/__init__.py
+examples/blueprints/routes/docs.py
+examples/blueprints/routes/api/__init__.py
+examples/blueprints/routes/api/v1/__init__.py
+examples/blueprints/routes/api/v1/users.py
+examples/blueprints/routes/api/v2/__init__.py
+examples/blueprints/routes/api/v2/users.py
 flask_useful/__init__.py
+flask_useful/app.py
 flask_useful/decorators.py
 flask_useful/flask_access.py
 flask_useful/sqla.py
 flask_useful/utils.py
 flask_useful/views.py
 flask_useful.egg-info/PKG-INFO
 flask_useful.egg-info/SOURCES.txt
```

