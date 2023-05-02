# Comparing `tmp/halborn_ctf-0.1.1.tar.gz` & `tmp/halborn_ctf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halborn_ctf-0.1.1.tar", last modified: Tue May  2 12:52:44 2023, max compression
+gzip compressed data, was "halborn_ctf-0.1.2.tar", last modified: Tue May  2 13:04:37 2023, max compression
```

## Comparing `halborn_ctf-0.1.1.tar` & `halborn_ctf-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.725767 halborn_ctf-0.1.1/
--rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/.coveragerc
--rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/.readthedocs.yml
--rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.1/AUTHORS.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/CHANGELOG.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.1/LICENSE.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 12:52:44.725835 halborn_ctf-0.1.1/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1689 2023-05-02 09:58:35.000000 halborn_ctf-0.1.1/README.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.720451 halborn_ctf-0.1.1/docs/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/Makefile
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.720666 halborn_ctf-0.1.1/docs/_static/
--rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/authors.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/changelog.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-02 08:35:26.000000 halborn_ctf-0.1.1/docs/conf.py
--rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/contributing.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     2329 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/index.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/license.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       39 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/docs/readme.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.1/docs/requirements.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/pyproject.toml
--rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-02 12:52:44.726189 halborn_ctf-0.1.1/setup.cfg
--rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/setup.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.716692 halborn_ctf-0.1.1/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.722258 halborn_ctf-0.1.1/src/halborn_ctf/
--rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.1/src/halborn_ctf/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.1/src/halborn_ctf/cli.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1087 2023-04-30 06:40:27.000000 halborn_ctf-0.1.1/src/halborn_ctf/functions.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.723888 halborn_ctf-0.1.1/src/halborn_ctf/network/
--rw-r--r--   0 fr0zn      (501) staff       (20)       93 2023-04-28 14:02:28.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1158 2023-04-30 06:48:19.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/_generic.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.724652 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/__init__.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.725143 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_json_rpc/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1260 2023-04-30 11:23:23.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1279 2023-05-01 07:09:26.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_utils.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.1/src/halborn_ctf/network/filters/json_rpc.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.1/src/halborn_ctf/shell.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     3604 2023-05-02 09:22:21.000000 halborn_ctf-0.1.1/src/halborn_ctf/state.py
--rw-r--r--   0 fr0zn      (501) staff       (20)    17516 2023-05-02 12:51:24.000000 halborn_ctf-0.1.1/src/halborn_ctf/templates.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.723557 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1141 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/SOURCES.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/dependency_links.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/entry_points.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/not-zip-safe
--rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/requires.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-02 12:52:44.000000 halborn_ctf-0.1.1/src/halborn_ctf.egg-info/top_level.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 12:52:44.725552 halborn_ctf-0.1.1/tests/
--rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/tests/conftest.py
--rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.1/tests/test_skeleton.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.1/tox.ini
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.904547 halborn_ctf-0.1.2/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.coveragerc
+-rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.readthedocs.yml
+-rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/AUTHORS.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/LICENSE.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 13:04:37.904622 halborn_ctf-0.1.2/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1689 2023-05-02 09:58:35.000000 halborn_ctf-0.1.2/README.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.899038 halborn_ctf-0.1.2/docs/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/Makefile
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.899362 halborn_ctf-0.1.2/docs/_static/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/authors.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/changelog.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-02 08:35:26.000000 halborn_ctf-0.1.2/docs/conf.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/contributing.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2329 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/index.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/license.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       39 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/readme.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.2/docs/requirements.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/pyproject.toml
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-02 13:04:37.904984 halborn_ctf-0.1.2/setup.cfg
+-rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/setup.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.895088 halborn_ctf-0.1.2/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.900896 halborn_ctf-0.1.2/src/halborn_ctf/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.2/src/halborn_ctf/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.2/src/halborn_ctf/cli.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1087 2023-04-30 06:40:27.000000 halborn_ctf-0.1.2/src/halborn_ctf/functions.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.902655 halborn_ctf-0.1.2/src/halborn_ctf/network/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       93 2023-04-28 14:02:28.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1158 2023-04-30 06:48:19.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/_generic.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.903348 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/__init__.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.903913 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1260 2023-04-30 11:23:23.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1279 2023-05-01 07:09:26.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_utils.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/json_rpc.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.2/src/halborn_ctf/shell.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     3604 2023-05-02 09:22:21.000000 halborn_ctf-0.1.2/src/halborn_ctf/state.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)    17750 2023-05-02 13:04:03.000000 halborn_ctf-0.1.2/src/halborn_ctf/templates.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.902280 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1141 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/SOURCES.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/dependency_links.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/entry_points.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/not-zip-safe
+-rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/requires.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/top_level.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.904348 halborn_ctf-0.1.2/tests/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/tests/conftest.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/tests/test_skeleton.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/tox.ini
```

### Comparing `halborn_ctf-0.1.1/.coveragerc` & `halborn_ctf-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/.gitignore` & `halborn_ctf-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/.readthedocs.yml` & `halborn_ctf-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/CONTRIBUTING.rst` & `halborn_ctf-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/LICENSE.txt` & `halborn_ctf-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/PKG-INFO` & `halborn_ctf-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn_ctf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.1/README.rst` & `halborn_ctf-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/docs/Makefile` & `halborn_ctf-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/docs/conf.py` & `halborn_ctf-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/docs/index.rst` & `halborn_ctf-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/setup.cfg` & `halborn_ctf-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/setup.py` & `halborn_ctf-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/__init__.py` & `halborn_ctf-0.1.2/src/halborn_ctf/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/cli.py` & `halborn_ctf-0.1.2/src/halborn_ctf/cli.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/functions.py` & `halborn_ctf-0.1.2/src/halborn_ctf/functions.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/_generic.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/_generic.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/filters/__init__.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/filters/_utils.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_utils.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/network/filters/json_rpc.py` & `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/json_rpc.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/shell.py` & `halborn_ctf-0.1.2/src/halborn_ctf/shell.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/state.py` & `halborn_ctf-0.1.2/src/halborn_ctf/state.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf/templates.py` & `halborn_ctf-0.1.2/src/halborn_ctf/templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,15 +256,18 @@
     @property
     def solved_msg(self):
         """(bool) Returns and allows to set a message or hint for the player. Only functional if :obj:`HAS_SOLVER` is set.
             Example::
 
                 def solver(self):
                     ...
-                    self.solved = True
+                    if self.solved:
+                        self.solved_msg = "You are the best hacker!"
+                    else:
+                        self.solved_msg = "Keep trying :("
 
         """
 
         if not self.HAS_SOLVER:
             raise ValueError('Challenge !HAS_SOLVER')
 
     @solved_msg.setter
@@ -348,21 +351,24 @@
     def state_public(self, value):
         if self._state_set:
             raise ValueError("State already set, use state.update instead")
         self._state._merge(value)
         self._state_set = True
 
     def _app_info_handler(self):
-        if not self.state.ready:
+        if not self.ready:
             return Response("Challenge not ready", status=503)
 
-        return self.state.public
+        return {
+            'ready': self.ready,
+            'state': self.state_public,
+        }
 
     def _app_files_handler(self):
-        if not self.state.ready:
+        if not self.ready:
             return Response("Challenge not ready", status=503)
 
         name = self.CHALLENGE_NAME.replace(' ','_')
 
         fileName = f"{name}.zip"
         files = self.files() + ['challenge.py']
 
@@ -374,38 +380,34 @@
 
         memory_file.seek(0)
         return flask.send_file(memory_file,
                         download_name=fileName,
                         as_attachment=True)
 
     def _app_solved_handler(self):
-        if not self.state.ready:
+        if not self.ready:
             return Response("Challenge not ready", status=503)
 
-        _pre_state = self.state.get('solved', False)
-
         # If not solved, we check on the solver
-        if not _pre_state:
+        if not self.solved:
             try:
                 self.solver()
             except Exception as e:
                 self._log.exception(e)
 
-        _solved_state = self.state.get('solved', False)
         response = {
-            'solved': _solved_state
-            }
+            'solved': self.solved
+        }
 
-        _solved_message = self.state.get('solved_msg', None)
-        if _solved_message:
-            response['msg'] = _solved_message
+        if self.solved_msg:
+            response['msg'] = self.solved_msg
         else:
-            response['msg'] = 'Solved' if _solved_state else 'Not solved'
+            response['msg'] = 'Solved' if self.solved else 'Not solved'
 
-        if _solved_state and self.FLAG_TYPE == FlagType.DYNAMIC:
+        if self.solved and self.FLAG_TYPE == FlagType.DYNAMIC:
             response['flag'] = os.environ.get('FLAG', 'HAL{PLACEHOLDER}')
 
         return response
 
     def _generic_path_handler(self, path, path_data: MappingInfo):
 
         port = path_data['port']
@@ -462,23 +464,29 @@
         if self.HAS_SOLVER:
             self._app.add_url_rule('/solved', 'solved', self._app_solved_handler, methods=['GET'])
 
     def _build(self):
         with _CleanChildProcesses():
             self.build()
 
-            f = open('state.dump', 'bw')
-            pickle.dump(self.state, f)
+            f = open('/tmp/state.dump', 'bw')
+            pickle.dump(self._state, f)
+
+            f = open('/tmp/state_public.dump', 'bw')
+            pickle.dump(self._state_public, f)
 
     def _run(self):
         with _CleanChildProcesses():
 
-            f = open('state.dump', 'br')
+            f = open('/tmp/state.dump', 'br')
             self._state = pickle.load(f)
 
+            f = open('/tmp/state_public.dump', 'br')
+            self._state_public = pickle.load(f)
+
             self._register_flask_paths()
             self._register_challenge_paths()
 
             self.run()
 
             self._flask_run()
```

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf.egg-info/PKG-INFO` & `halborn_ctf-0.1.2/src/halborn_ctf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn-ctf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.1/src/halborn_ctf.egg-info/SOURCES.txt` & `halborn_ctf-0.1.2/src/halborn_ctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/tests/test_skeleton.py` & `halborn_ctf-0.1.2/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.1/tox.ini` & `halborn_ctf-0.1.2/tox.ini`

 * *Files identical despite different names*

