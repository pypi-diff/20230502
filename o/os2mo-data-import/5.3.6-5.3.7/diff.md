# Comparing `tmp/os2mo_data_import-5.3.6.tar.gz` & `tmp/os2mo_data_import-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2mo_data_import-5.3.6.tar", max compression
+gzip compressed data, was "os2mo_data_import-5.3.7.tar", max compression
```

## Comparing `os2mo_data_import-5.3.6.tar` & `os2mo_data_import-5.3.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0        0        0        0 2023-05-02 02:21:42.113141 os2mo_data_import-5.3.6/LICENSES/
--rw-r--r--   0        0        0    11696 2023-05-02 02:21:42.114141 os2mo_data_import-5.3.6/README.rst
--rw-r--r--   0        0        0      332 2023-05-02 02:21:42.114141 os2mo_data_import-5.3.6/mox_helpers/__init__.py
--rw-r--r--   0        0        0     7243 2023-05-02 02:21:42.115141 os2mo_data_import-5.3.6/mox_helpers/mox_helper.py
--rw-r--r--   0        0        0    20756 2023-05-02 02:21:42.115141 os2mo_data_import-5.3.6/mox_helpers/mox_util.py
--rw-r--r--   0        0        0     2736 2023-05-02 02:21:42.115141 os2mo_data_import-5.3.6/mox_helpers/payloads.py
--rw-r--r--   0        0        0       40 2023-05-02 02:21:42.115141 os2mo_data_import-5.3.6/mox_helpers/requirements.txt
--rw-r--r--   0        0        0      899 2023-05-02 02:21:42.115141 os2mo_data_import-5.3.6/mox_helpers/utils.py
--rw-r--r--   0        0        0      397 2023-05-02 02:21:42.116141 os2mo_data_import-5.3.6/os2mo_data_import/__init__.py
--rw-r--r--   0        0        0     3799 2023-05-02 02:21:42.116141 os2mo_data_import-5.3.6/os2mo_data_import/caching_import.py
--rw-r--r--   0        0        0     1300 2023-05-02 02:21:42.116141 os2mo_data_import-5.3.6/os2mo_data_import/defaults.py
--rw-r--r--   0        0        0    19484 2023-05-02 02:21:42.116141 os2mo_data_import-5.3.6/os2mo_data_import/helpers.py
--rw-r--r--   0        0        0    22987 2023-05-02 02:21:42.129143 os2mo_data_import-5.3.6/os2mo_data_import/mora_data_types.py
--rw-r--r--   0        0        0    13436 2023-05-02 02:21:42.129143 os2mo_data_import-5.3.6/os2mo_data_import/mox_data_types.py
--rw-r--r--   0        0        0       99 2023-05-02 02:21:42.129143 os2mo_data_import-5.3.6/os2mo_data_import/tests/__init__.py
--rw-r--r--   0        0        0     1650 2023-05-02 02:21:42.129143 os2mo_data_import-5.3.6/os2mo_data_import/tests/test_utilities.py
--rw-r--r--   0        0        0    27431 2023-05-02 02:21:42.132143 os2mo_data_import-5.3.6/os2mo_data_import/utilities.py
--rw-r--r--   0        0        0      332 2023-05-02 02:21:42.132143 os2mo_data_import-5.3.6/os2mo_helpers/__init__.py
--rw-r--r--   0        0        0    30138 2023-05-02 02:21:42.132143 os2mo_data_import-5.3.6/os2mo_helpers/mora_helpers.py
--rw-r--r--   0        0        0       41 2023-05-02 02:21:42.132143 os2mo_data_import-5.3.6/os2mo_helpers/requirements.txt
--rw-r--r--   0        0        0     1169 2023-05-02 02:21:42.133143 os2mo_data_import-5.3.6/os2mo_helpers/settings.py
--rw-r--r--   0        0        0       99 2023-05-02 02:21:42.133143 os2mo_data_import-5.3.6/os2mo_helpers/tests/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-02 02:21:42.133143 os2mo_data_import-5.3.6/os2mo_helpers/tests/test_morahelpers.py
--rw-r--r--   0        0        0     1054 2023-05-02 02:21:44.241339 os2mo_data_import-5.3.6/pyproject.toml
--rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.6/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-02 02:23:30.064176 os2mo_data_import-5.3.7/LICENSES/
+-rw-r--r--   0        0        0    11696 2023-05-02 02:23:30.064176 os2mo_data_import-5.3.7/README.rst
+-rw-r--r--   0        0        0      332 2023-05-02 02:23:30.065176 os2mo_data_import-5.3.7/mox_helpers/__init__.py
+-rw-r--r--   0        0        0     7243 2023-05-02 02:23:30.065176 os2mo_data_import-5.3.7/mox_helpers/mox_helper.py
+-rw-r--r--   0        0        0    20756 2023-05-02 02:23:30.065176 os2mo_data_import-5.3.7/mox_helpers/mox_util.py
+-rw-r--r--   0        0        0     2736 2023-05-02 02:23:30.065176 os2mo_data_import-5.3.7/mox_helpers/payloads.py
+-rw-r--r--   0        0        0       40 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/mox_helpers/requirements.txt
+-rw-r--r--   0        0        0      899 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/mox_helpers/utils.py
+-rw-r--r--   0        0        0      397 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/os2mo_data_import/__init__.py
+-rw-r--r--   0        0        0     3799 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/os2mo_data_import/caching_import.py
+-rw-r--r--   0        0        0     1300 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/os2mo_data_import/defaults.py
+-rw-r--r--   0        0        0    19484 2023-05-02 02:23:30.066176 os2mo_data_import-5.3.7/os2mo_data_import/helpers.py
+-rw-r--r--   0        0        0    22987 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_data_import/mora_data_types.py
+-rw-r--r--   0        0        0    13436 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_data_import/mox_data_types.py
+-rw-r--r--   0        0        0       99 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_data_import/tests/__init__.py
+-rw-r--r--   0        0        0     1650 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_data_import/tests/test_utilities.py
+-rw-r--r--   0        0        0    27431 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_data_import/utilities.py
+-rw-r--r--   0        0        0      332 2023-05-02 02:23:30.067176 os2mo_data_import-5.3.7/os2mo_helpers/__init__.py
+-rw-r--r--   0        0        0    30138 2023-05-02 02:23:30.068177 os2mo_data_import-5.3.7/os2mo_helpers/mora_helpers.py
+-rw-r--r--   0        0        0       41 2023-05-02 02:23:30.068177 os2mo_data_import-5.3.7/os2mo_helpers/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-05-02 02:23:30.068177 os2mo_data_import-5.3.7/os2mo_helpers/settings.py
+-rw-r--r--   0        0        0       99 2023-05-02 02:23:30.068177 os2mo_data_import-5.3.7/os2mo_helpers/tests/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-02 02:23:30.068177 os2mo_data_import-5.3.7/os2mo_helpers/tests/test_morahelpers.py
+-rw-r--r--   0        0        0     1054 2023-05-02 02:23:31.259287 os2mo_data_import-5.3.7/pyproject.toml
+-rw-r--r--   0        0        0    13094 1970-01-01 00:00:00.000000 os2mo_data_import-5.3.7/PKG-INFO
```

### Comparing `os2mo_data_import-5.3.6/README.rst` & `os2mo_data_import-5.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/mox_helpers/mox_helper.py` & `os2mo_data_import-5.3.7/mox_helpers/mox_helper.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/mox_helpers/mox_util.py` & `os2mo_data_import-5.3.7/mox_helpers/mox_util.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/mox_helpers/payloads.py` & `os2mo_data_import-5.3.7/mox_helpers/payloads.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/mox_helpers/utils.py` & `os2mo_data_import-5.3.7/mox_helpers/utils.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/caching_import.py` & `os2mo_data_import-5.3.7/os2mo_data_import/caching_import.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/defaults.py` & `os2mo_data_import-5.3.7/os2mo_data_import/defaults.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/helpers.py` & `os2mo_data_import-5.3.7/os2mo_data_import/helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/mora_data_types.py` & `os2mo_data_import-5.3.7/os2mo_data_import/mora_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/mox_data_types.py` & `os2mo_data_import-5.3.7/os2mo_data_import/mox_data_types.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/tests/test_utilities.py` & `os2mo_data_import-5.3.7/os2mo_data_import/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_data_import/utilities.py` & `os2mo_data_import-5.3.7/os2mo_data_import/utilities.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_helpers/mora_helpers.py` & `os2mo_data_import-5.3.7/os2mo_helpers/mora_helpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_helpers/settings.py` & `os2mo_data_import-5.3.7/os2mo_helpers/settings.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/os2mo_helpers/tests/test_morahelpers.py` & `os2mo_data_import-5.3.7/os2mo_helpers/tests/test_morahelpers.py`

 * *Files identical despite different names*

### Comparing `os2mo_data_import-5.3.6/pyproject.toml` & `os2mo_data_import-5.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "os2mo_data_import"
-version = "5.3.6"
+version = "5.3.7"
 description = "A set of tools for OS2MO data import and export"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.rst"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo_data_import"
 keywords = ["os2mo", "dipex"]
 packages = [
@@ -33,12 +33,12 @@
 pytest-split = "^0.8.0"
 ra-utils = "^1.13.0"
 parameterized = "^0.9.0"
 pre-commit = "^3.2.2"
 
 [tool.poetry.dev-dependencies]
 freezegun = "^1.2.0"
-black = "^22.1.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `os2mo_data_import-5.3.6/PKG-INFO` & `os2mo_data_import-5.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2mo-data-import
-Version: 5.3.6
+Version: 5.3.7
 Summary: A set of tools for OS2MO data import and export
 Home-page: https://git.magenta.dk/rammearkitektur/os2mo_data_import
 License: MPL-2.0
 Keywords: os2mo,dipex
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```

