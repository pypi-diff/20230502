# Comparing `tmp/halborn_ctf-0.1.2.tar.gz` & `tmp/halborn_ctf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halborn_ctf-0.1.2.tar", last modified: Tue May  2 13:04:37 2023, max compression
+gzip compressed data, was "halborn_ctf-0.1.4.tar", last modified: Tue May  2 18:12:19 2023, max compression
```

## Comparing `halborn_ctf-0.1.2.tar` & `halborn_ctf-0.1.4.tar`

### file list

```diff
@@ -1,55 +1,60 @@
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.904547 halborn_ctf-0.1.2/
--rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.coveragerc
--rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/.readthedocs.yml
--rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/AUTHORS.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/CHANGELOG.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/LICENSE.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 13:04:37.904622 halborn_ctf-0.1.2/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1689 2023-05-02 09:58:35.000000 halborn_ctf-0.1.2/README.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.899038 halborn_ctf-0.1.2/docs/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/Makefile
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.899362 halborn_ctf-0.1.2/docs/_static/
--rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/_static/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/authors.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/changelog.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-02 08:35:26.000000 halborn_ctf-0.1.2/docs/conf.py
--rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/contributing.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     2329 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/index.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/license.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       39 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/docs/readme.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.2/docs/requirements.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/pyproject.toml
--rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-02 13:04:37.904984 halborn_ctf-0.1.2/setup.cfg
--rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/setup.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.895088 halborn_ctf-0.1.2/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.900896 halborn_ctf-0.1.2/src/halborn_ctf/
--rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.2/src/halborn_ctf/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.2/src/halborn_ctf/cli.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1087 2023-04-30 06:40:27.000000 halborn_ctf-0.1.2/src/halborn_ctf/functions.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.902655 halborn_ctf-0.1.2/src/halborn_ctf/network/
--rw-r--r--   0 fr0zn      (501) staff       (20)       93 2023-04-28 14:02:28.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1158 2023-04-30 06:48:19.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/_generic.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.903348 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/__init__.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.903913 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1260 2023-04-30 11:23:23.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1279 2023-05-01 07:09:26.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_utils.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.2/src/halborn_ctf/network/filters/json_rpc.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.2/src/halborn_ctf/shell.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     3604 2023-05-02 09:22:21.000000 halborn_ctf-0.1.2/src/halborn_ctf/state.py
--rw-r--r--   0 fr0zn      (501) staff       (20)    17750 2023-05-02 13:04:03.000000 halborn_ctf-0.1.2/src/halborn_ctf/templates.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.902280 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2184 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1141 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/SOURCES.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/dependency_links.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/entry_points.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/not-zip-safe
--rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/requires.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-02 13:04:37.000000 halborn_ctf-0.1.2/src/halborn_ctf.egg-info/top_level.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 13:04:37.904348 halborn_ctf-0.1.2/tests/
--rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/tests/conftest.py
--rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.2/tests/test_skeleton.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.2/tox.ini
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.601361 halborn_ctf-0.1.4/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.coveragerc
+-rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/.readthedocs.yml
+-rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/AUTHORS.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/CHANGELOG.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/LICENSE.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-02 18:12:19.601444 halborn_ctf-0.1.4/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.4/README.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.594621 halborn_ctf-0.1.4/docs/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/Makefile
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.594998 halborn_ctf-0.1.4/docs/_static/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/_static/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/authors.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/changelog.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-02 08:35:26.000000 halborn_ctf-0.1.4/docs/conf.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/contributing.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1649 2023-05-02 13:58:34.000000 halborn_ctf-0.1.4/docs/index.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/license.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       39 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/docs/readme.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.590304 halborn_ctf-0.1.4/docs/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.595776 halborn_ctf-0.1.4/docs/src/getting_started/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-02 17:58:39.000000 halborn_ctf-0.1.4/docs/src/getting_started/examples.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.4/docs/src/getting_started/installation.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     8664 2023-05-02 18:10:20.000000 halborn_ctf-0.1.4/docs/src/getting_started/quick_start.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/pyproject.toml
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-02 18:12:19.601840 halborn_ctf-0.1.4/setup.cfg
+-rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/setup.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.590451 halborn_ctf-0.1.4/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.597601 halborn_ctf-0.1.4/src/halborn_ctf/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.4/src/halborn_ctf/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.4/src/halborn_ctf/cli.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:03:03.000000 halborn_ctf-0.1.4/src/halborn_ctf/functions.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.599183 halborn_ctf-0.1.4/src/halborn_ctf/network/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/_generic.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.600112 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/__init__.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.600687 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_utils.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.4/src/halborn_ctf/network/filters/json_rpc.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.4/src/halborn_ctf/shell.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     3598 2023-05-02 15:27:02.000000 halborn_ctf-0.1.4/src/halborn_ctf/state.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)    20343 2023-05-02 18:11:40.000000 halborn_ctf-0.1.4/src/halborn_ctf/templates.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.598846 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1262 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/SOURCES.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/dependency_links.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/entry_points.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/not-zip-safe
+-rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/requires.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-02 18:12:19.000000 halborn_ctf-0.1.4/src/halborn_ctf.egg-info/top_level.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-02 18:12:19.601165 halborn_ctf-0.1.4/tests/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/tests/conftest.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.4/tests/test_skeleton.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.4/tox.ini
```

### Comparing `halborn_ctf-0.1.2/.coveragerc` & `halborn_ctf-0.1.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/.gitignore` & `halborn_ctf-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/.readthedocs.yml` & `halborn_ctf-0.1.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/CONTRIBUTING.rst` & `halborn_ctf-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/LICENSE.txt` & `halborn_ctf-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/PKG-INFO` & `halborn_ctf-0.1.4/src/halborn_ctf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: halborn_ctf
-Version: 0.1.2
+Name: halborn-ctf
+Version: 0.1.4
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
@@ -39,15 +39,14 @@
         :alt: Twitter
         :target: https://twitter.com/halborn_ctf
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
-|
 
 ===========
 halborn_ctf
 ===========
 
 
     Add a short description here!
```

### Comparing `halborn_ctf-0.1.2/README.rst` & `halborn_ctf-0.1.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         :alt: Twitter
         :target: https://twitter.com/halborn_ctf
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
-|
 
 ===========
 halborn_ctf
 ===========
 
 
     Add a short description here!
```

### Comparing `halborn_ctf-0.1.2/docs/Makefile` & `halborn_ctf-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/docs/conf.py` & `halborn_ctf-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/setup.cfg` & `halborn_ctf-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/setup.py` & `halborn_ctf-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/__init__.py` & `halborn_ctf-0.1.4/src/halborn_ctf/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/cli.py` & `halborn_ctf-0.1.4/src/halborn_ctf/cli.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/functions.py` & `halborn_ctf-0.1.4/src/halborn_ctf/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,13 +26,25 @@
 
 def periodic(*, every: int):
     """It allows executing a function as a periodic function in a thread on the background.
 
     Args:
         every (int): The amount of seconds to wait to execute the function again. It should be bigger than 0.
 
+    Example:
+
+        .. code::
+
+            @periodic(every=1)
+            def function():
+                print("HI")
+
+            function() # Does start printing "HI" every 1 second
+
+            function.stop() # Does stop the function execution
+
     Raises:
         ValueError: If the ``every`` parameter is set to 0.
     """
     def decorator(function):
         return _PeriodicFunction(function, every=every)
     return decorator
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/_generic.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/_generic.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,7 +26,15 @@
             with socket.create_connection((host, port), timeout=timeout):
                 _logger.info('Port "{}" found'.format(port))
                 break
         except OSError as ex:
             time.sleep(0.01)
             if time.perf_counter() - start_time >= timeout:
                 TimeoutError('Waited too long for port "{}" on host "{}" to start accepting connections.'.format(port, host))
+
+from contextlib import closing
+
+def find_free_port():
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.bind(('', 0))
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return s.getsockname()[1]
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/__init__.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
     def request(self, flow):
         json_dump = json.loads(flow.request.content)
         is_filtered = False
         if ctx.options.methods:
             _allmethods = json.loads(ctx.options.methods)
             for _method in _allmethods:
-                if re.search(_method, json_dump['method']) is not None:
-                    is_filtered = True
-                    break
+                if _method.strip() != '':
+                    if re.search(_method, json_dump['method']) is not None:
+                        is_filtered = True
+                        break
 
         if is_filtered:
             status = 200
             content = {
                     "jsonrpc": "2.0",
                     "id": json_dump['id'],
                     "error": {
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
     def request(self, flow):
         json_dump = json.loads(flow.request.content)
         is_whitelisted = False
         if ctx.options.methods:
             _allmethods = json.loads(ctx.options.methods)
             for _method in _allmethods:
-                if re.search(_method, json_dump['method']) is not None:
-                    is_whitelisted = True
-                    break
+                if _method.strip() != '':
+                    if re.search(_method, json_dump['method']) is not None:
+                        is_whitelisted = True
+                        break
 
         if not is_whitelisted:
             status = 200
             content = {
                     "jsonrpc": "2.0",
                     "id": json_dump['id'],
                     "error": {
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/_utils.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/_utils.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/network/filters/json_rpc.py` & `halborn_ctf-0.1.4/src/halborn_ctf/network/filters/json_rpc.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/shell.py` & `halborn_ctf-0.1.4/src/halborn_ctf/shell.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/state.py` & `halborn_ctf-0.1.4/src/halborn_ctf/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def __init__(self, *args, **kw):
         _dict = args[0]
         for k in _dict.keys():
             if type(_dict[k]) == dict:
                 _dict[k] = State(_dict[k])
-        super(State,self).__init__(*args, **kw)
+        super(State,self).__init__(_dict)
 
     def __getattr__(self, key):
         return self.get(key, None)
 
     # def __setitem__(self, key, value):
     #     super().__setitem__(key, value)
         # raise NotImplementedError()
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf/templates.py` & `halborn_ctf-0.1.4/src/halborn_ctf/templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 import zipfile
 import sys
 from io import BytesIO
 import glob
 import pickle
 import signal
 from urllib.parse import urljoin
-from typing import TypedDict, NotRequired
+from typing import TypedDict, NotRequired, Callable
 from enum import Enum
 
 from .state import State
 
 from abc import ABC, abstractmethod
 
+from .network import find_free_port
+
 # https://stackoverflow.com/questions/320232/ensuring-subprocesses-are-dead-on-exiting-python-program
 class _CleanChildProcesses:
   def __enter__(self):
     logging.info("pid=%d  pgid=%d" % (os.getpid(), os.getpgid(0)))
 
     try:
         os.setpgrp() # create new process group, become its leader
@@ -62,30 +64,46 @@
       os.killpg(0, signal.SIGINT) # kill all processes in my group
     except KeyboardInterrupt:
       # SIGINT is delievered to this process as well as the child processes.
       # Ignore it so that the existing exception, if any, is returned. This
       # leaves us with a clean exit code if there was no exception.
       pass
 
+class MappingInfoFilter(TypedDict):
+    """Dictionary data type to store the details for a filter used on a mapping.
+    """
+
+    method: Callable
+    """ (Callable): The function that runs the filter.
+    """
+    args: NotRequired[list]
+    """ (list, optional): The list of arguments for the filter function.
+    """
+    kwargs: NotRequired[str]
+    """ (dict, optional): The kwargs for the filter function, only used by default on custom filters and will be passed on the script inside ``ctx.options.[HERE]``.
+    """
 
 class MappingInfo(TypedDict):
     """Dictionary data type to store the details for a path mapping
     """
 
     port: int
-    """ port (int): The port to redirect to.
+    """ (int): The port to redirect to.
     """
     host: NotRequired[str]
-    """ host (str): The host to redirect to. Defaults to ``'127.0.0.1'``.
+    """ (str, optional): The host to redirect to. Defaults to ``'127.0.0.1'``.
     """
     path: NotRequired[str]
-    """ path (str): The path to redirect to. Defaults to ``'/'``.
+    """ (str, optional): The path to redirect to. Defaults to ``'/'``.
     """
     methods: list[str]
-    """ methods (list[str]): The allowd methods. Defaults to ``["GET"]``.
+    """ (list[str], optional): The allowed methods. Defaults to ``["GET"]``.
+    """
+    filter: NotRequired[MappingInfoFilter]
+    """ (MappingInfoFilter, optional): Information containing a filter to execute.
     """
 
 class FlagType(Enum):
     NONE = 0
     """If no flag is present
     """
     STATIC = 1
@@ -99,15 +117,15 @@
     """Generic CTF challenge template
 
     Each created/deployed challenge does have two steps defined, :obj:`build` and :obj:`run`. The ``build`` step is only executed once
     when the challenge is created and uploaded into the platform for playing. The ``run`` step is always executed for each player request
     to deploy a new challenge.
 
     This template does also expose the challenge by using an HTTP server. The server does allow registering routes to it by using
-    the :obj:`path_mapping` attribute.
+    the :obj:`PATH_MAPPING` attribute.
 
     An attribute named :obj:`state` can be used to store any sort of object that will persiste between the ``build`` and ``run`` steps. Furthermore,
     this attribute can be used to store anything that would be used across the different functions. The `state_public` property will be exposed
     under the `/state` path on the challenge domain.
 
     The following routes will be exposed under ``localhost:8080``:
 
@@ -120,29 +138,28 @@
     - ``/files``: Does download the files listed under the "files" function as a zip file named by :attr:`CHALLENGE_NAME`.
 
     Note:
         Only if :attr:`HAS_FILES` == ``True``.
 
     """
 
-    CHALLENGE_NAME = os.environ.get('CHALLENGE_NAME', 'challenge')
+    CHALLENGE_NAME = 'challenge'
     """ (str): The name of the challenge.
     """
 
     FLAG_TYPE = FlagType.NONE
     """ (FlagType): The type of flag. Set to :obj:`FlagType.NONE` if using a solver unless using manual flag input on the CTF platform.
     """
 
     HAS_FILES = False
     """ (bool): If the challenge has downloadable files. A "files" function must be defined returning a list of files that
     will be downloable from the challenge container. Glob patterns can be used (:mod:`glob`)::
 
         def files(self):
             return [
-                "challenge.py",
                 "filter.py",
                 "folder/test.sol",
                 "folder2/**",
                 "folder3/*.sol",
             ]
 
     Note:
@@ -157,25 +174,81 @@
         def solver(self):
             pass
 
     Note:
         This function will be executed each time the user requests the `/solved` route.
     """
 
+    PATH_MAPPING = {}
+    """
+    (dict[str, MappingInfo]): Mapping used internally to register the challenge URL's paths.
+    It does contain a mapping of ``path`` to ``MappingInfo`` dictionary details.
+
+    Example:
+        Have the challenge ``/`` path expose the anvil service which is running internally on port ``8545``::
+
+            PATH_MAPPING = {
+                '/': {
+                        'host': '127.0.0.1', # optional. Defaults to '127.0.0.1'
+                        'port': 8545,
+                        'path': '/', # optional. Defaults to '/'
+                        'methods': ['POST'] # optional. Defaults to ['GET']
+                }
+            }
+
+        A request to http://challenge/ will be proxied to http://127.0.0.1:8545/
+
+        Redirect all request to the service running on port ``9999`` and under ``/service``::
+
+            PATH_MAPPING = {
+                '/<path:path>': {
+                        'port': 9999,
+                        'path': '/service',
+                        'methods': ['GET', 'POST', 'HEAD']
+                }
+            }
+
+        A request to http://challenge/my_path/file will be proxied to http://127.0.0.1:9999/service/my_path/file. But not http://challenge/.
+
+        It allows to use filters::
+
+            PATH_MAPPING = {
+                '/': {
+                        'port': 8545,
+                        'path': '/',
+                        'methods': ['POST'],
+                        'filter': {
+                            'method': network.filters.json_rpc.filter_methods,
+                            'args': [],
+
+                            # Custom filter
+                            # 'method': network.filters.run_script,
+                            # 'args': ['filter.py'],
+                            # 'kwargs': {}
+                        }
+                }
+            }
+
+    Note:
+        There is no need to specify any of the required field for the filter such as ``listen_port``, ``to_port``, ``to_host`` as those will
+        be extracted from the mapping itself and a random listening port used and remapped.
+    """
+
     def __init__(self) -> None:
         super().__init__()
 
         self._app = flask.Flask('Challenge')
-        self._log = logging.getLogger('GenericChallenge')
+        self.log = logging.getLogger(self.CHALLENGE_NAME)
 
         CORS(self._app)
 
         self._ready = False
         self._state_set = False
         self._state = State({})
+        self._state_public_set = False
         self._state_public = State({})
 
         #     'public': State({}),
         #     'ready': False,
         # })
 
         if self.HAS_SOLVER:
@@ -209,32 +282,32 @@
                 pass
 
         if not self.HAS_SOLVER and self.FLAG_TYPE == FlagType.NONE:
             raise ValueError("HAS_SOLVER == False and FLAG_TYPE == NONE")
 
         self._path_mapping: dict[str, MappingInfo] = {}
 
-    @property
-    def ready(self):
-        """(bool): Allows setting the challenge as ready to be played.
-
-            Example::
-
-                def run(self):
-                    ...
-                    self.ready = True
-
-        """
-        return self._ready
-
-    @ready.setter
-    def ready(self, value):
-        # if self._ready:
-        #     raise ValueError('Challenge ready already')
-        self._ready = value
+    # @property
+    # def ready(self):
+    #     """(bool): Allows setting the challenge as ready to be played.
+
+    #         Example::
+
+    #             def run(self):
+    #                 ...
+    #                 self.ready = True
+
+    #     """
+    #     return self._ready
+
+    # @ready.setter
+    # def ready(self, value):
+    #     # if self._ready:
+    #     #     raise ValueError('Challenge ready already')
+    #     self._ready = value
 
     @property
     def solved(self):
         """(bool): Returns and allows to set if the challenge is solved or not. Only functional if :obj:`HAS_SOLVER` is set.
 
             Example::
 
@@ -242,24 +315,25 @@
                     ...
                     self.solved = True
 
         """
 
         if not self.HAS_SOLVER:
             raise ValueError('Challenge !HAS_SOLVER')
+        return self._solved
 
     @solved.setter
     def solved(self, value):
         if not self.HAS_SOLVER:
             raise ValueError('Challenge !HAS_SOLVER')
         self._solved = value
 
     @property
     def solved_msg(self):
-        """(bool) Returns and allows to set a message or hint for the player. Only functional if :obj:`HAS_SOLVER` is set.
+        """(str): Returns and allows to set a message or hint for the player. Only functional if :obj:`HAS_SOLVER` is set.
             Example::
 
                 def solver(self):
                     ...
                     if self.solved:
                         self.solved_msg = "You are the best hacker!"
                     else:
@@ -273,47 +347,14 @@
     @solved_msg.setter
     def solved_msg(self, value):
         if not self.HAS_SOLVER:
             raise ValueError('Challenge !HAS_SOLVER')
         self._solved_msg = value
 
     @property
-    def path_mapping(self):
-        """(dict[str, MappingInfo]): Mapping used internally to register the challenge URL's paths.
-            It does contain a mapping of ``path`` to ``MappingInfo`` dictionary details.
-
-            Example:
-                Have the challenge ``/`` path expose the anvil service which is running internally on port ``8545``::
-
-                    self.path_mapping = {
-                        '/': {
-                                'host': '127.0.0.1', # optional. Defaults to '127.0.0.1'
-                                'port': 8545,
-                                'path': '/', # optional. Defaults to '/'
-                                'methods': ['POST'] # optional. Defaults to ['GET']
-                        }
-                    }
-
-                Redirect all request to the service running on port ``8080`` and under ``/service``::
-
-                    self.path_mapping = {
-                        '/<path:path>': {
-                                'port': 8080,
-                                'path': '/service',
-                                'methods': ['GET', 'POST', 'HEAD']
-                        }
-                    }
-        """
-        return self._path_mapping
-
-    @path_mapping.setter
-    def path_mapping(self, value):
-        self._path_mapping = value
-
-    @property
     def state(self):
         """(State): Extended dictionary to store variables that can be accessed during challenge execution.
 
         The challenge :obj:`build` step will pickle this variable for the :obj:`run` method to have the same state.
 
         Example:
             Initializing the state::
@@ -335,28 +376,30 @@
         return self._state
 
     @state.setter
     def state(self, value):
         if self._state_set:
             raise ValueError("State already set, use state.update instead")
         self._state._merge(value)
+        # self._state = State(value)
         self._state_set = True
 
     @property
     def state_public(self):
         """(State): It will expose the state content into the challenge ``/state`` route. Refer to :obj:`state`.
         """
         return self._state_public
 
     @state_public.setter
     def state_public(self, value):
-        if self._state_set:
-            raise ValueError("State already set, use state.update instead")
-        self._state._merge(value)
-        self._state_set = True
+        if self._state_public_set:
+            raise ValueError("State already set, use state_public.update instead")
+        self._state_public._merge(value)
+        # self._state_public_set = State(value)
+        self._state_public_set = True
 
     def _app_info_handler(self):
         if not self.ready:
             return Response("Challenge not ready", status=503)
 
         return {
             'ready': self.ready,
@@ -388,15 +431,15 @@
             return Response("Challenge not ready", status=503)
 
         # If not solved, we check on the solver
         if not self.solved:
             try:
                 self.solver()
             except Exception as e:
-                self._log.exception(e)
+                self.log.exception(e)
 
         response = {
             'solved': self.solved
         }
 
         if self.solved_msg:
             response['msg'] = self.solved_msg
@@ -404,24 +447,24 @@
             response['msg'] = 'Solved' if self.solved else 'Not solved'
 
         if self.solved and self.FLAG_TYPE == FlagType.DYNAMIC:
             response['flag'] = os.environ.get('FLAG', 'HAL{PLACEHOLDER}')
 
         return response
 
-    def _generic_path_handler(self, path, path_data: MappingInfo):
+    def _generic_path_handler(self, port, host, path):
 
-        port = path_data['port']
-        host = path_data.get('host', '127.0.0.1')
-        proxy_path = path_data.get('path', '/')
+        # port = path_data['port']
+        # host = path_data.get('host', '127.0.0.1')
+        # proxy_path = path_data.get('path', '/')
 
         def _handler(**kwargs):
 
             # Important to add the final '/'
-            full_path = urljoin(proxy_path, '/' + kwargs.get('path', ''))
+            full_path = urljoin(path, '/' + kwargs.get('path', ''))
             full_url = f'http://{host}:{port}{full_path}'
 
             try:
                 resp = requests.request(
                     method=request.method,
                     url=full_url,
                     headers={key: value for (key, value)
@@ -439,19 +482,34 @@
                 return Response(resp, resp.status_code, headers)
             except ConnectionError:
                 return Response("Could not connect with server on port {}".format(None), 503)
 
         return _handler
 
     def _register_challenge_paths(self):
-        for i, values in enumerate(self.path_mapping.items()):
+        for i, values in enumerate(self.PATH_MAPPING.items()):
             path, path_data = values
             methods = path_data.get('methods', ['GET'])
+            host = path_data.get('host', '127.0.0.1')
+            port = path_data['port']
             # TODO: Verify methods and path_data
-            self._app.add_url_rule(path, 'mapping-{}'.format(i), self._generic_path_handler(path, path_data), methods=methods)
+            _filter = path_data.get('filter', None)
+            if _filter and _filter['method']:
+                _filter_args = _filter.get('args', [])
+                _filter_kwargs = _filter.get('kwargs', {})
+
+                random_port = find_free_port()
+
+                # The filter should listen on random port and redirect to host:port
+                _filter['method'](*_filter_args, **_filter_kwargs, listen_port=random_port, to_port=port, to_host=host)
+
+                # The path mapping should redirect to 127.0.0.1:random_port
+                self._app.add_url_rule(path, 'mapping-{}'.format(i), self._generic_path_handler(port=random_port, host='127.0.0.1', path=path), methods=methods)
+            else:
+                self._app.add_url_rule(path, 'mapping-{}'.format(i), self._generic_path_handler(port=port, host=host, path=path), methods=methods)
 
     def _flask_run(self):
         cli = sys.modules['flask.cli']
         cli.show_server_banner = lambda *x: None
 
         self._app.run(host='0.0.0.0', port=os.environ.get('PORT', 8080), use_reloader=False, debug=False)
 
@@ -474,24 +532,30 @@
             f = open('/tmp/state_public.dump', 'bw')
             pickle.dump(self._state_public, f)
 
     def _run(self):
         with _CleanChildProcesses():
 
             f = open('/tmp/state.dump', 'br')
-            self._state = pickle.load(f)
+            tmp = pickle.load(f)
+            self._state._merge(tmp)
 
             f = open('/tmp/state_public.dump', 'br')
-            self._state_public = pickle.load(f)
+            # TODO: Do a merge instead of replace
+            tmp = pickle.load(f)
+            self._state_public._merge(tmp)
 
             self._register_flask_paths()
-            self._register_challenge_paths()
 
             self.run()
 
+            self._register_challenge_paths()
+
+            self.ready = True
+
             self._flask_run()
 
 
     @abstractmethod
     def build(self):
         """All the static funtionality that should be executed during the build phase of the challenge container. The running container will
         have everything executed here pre-bundled as this funcionality is only executed once for all running instances.
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf.egg-info/PKG-INFO` & `halborn_ctf-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: halborn-ctf
-Version: 0.1.2
+Name: halborn_ctf
+Version: 0.1.4
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
@@ -39,15 +39,14 @@
         :alt: Twitter
         :target: https://twitter.com/halborn_ctf
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 
-|
 
 ===========
 halborn_ctf
 ===========
 
 
     Add a short description here!
```

### Comparing `halborn_ctf-0.1.2/src/halborn_ctf.egg-info/SOURCES.txt` & `halborn_ctf-0.1.4/src/halborn_ctf.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
+docs/src/getting_started/examples.rst
+docs/src/getting_started/installation.rst
+docs/src/getting_started/quick_start.rst
 src/halborn_ctf/__init__.py
 src/halborn_ctf/cli.py
 src/halborn_ctf/functions.py
 src/halborn_ctf/shell.py
 src/halborn_ctf/state.py
 src/halborn_ctf/templates.py
 src/halborn_ctf.egg-info/PKG-INFO
```

### Comparing `halborn_ctf-0.1.2/tests/test_skeleton.py` & `halborn_ctf-0.1.4/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.2/tox.ini` & `halborn_ctf-0.1.4/tox.ini`

 * *Files identical despite different names*

