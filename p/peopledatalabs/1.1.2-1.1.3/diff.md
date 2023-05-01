# Comparing `tmp/peopledatalabs-1.1.2.tar.gz` & `tmp/peopledatalabs-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-1.1.2.tar", max compression
+gzip compressed data, was "peopledatalabs-1.1.3.tar", max compression
```

## Comparing `peopledatalabs-1.1.2.tar` & `peopledatalabs-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1073 2022-10-31 18:44:51.444963 peopledatalabs-1.1.2/LICENSE
--rw-r--r--   0        0        0    12222 2022-10-31 18:44:51.444963 peopledatalabs-1.1.2/README.md
--rw-r--r--   0        0        0     1639 2022-10-31 18:44:51.444963 peopledatalabs-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      109 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     5612 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     1635 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      762 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2812 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      744 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      984 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5069 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2445 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     2198 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      215 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4162 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      783 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2434 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1156 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      670 2022-10-31 18:44:51.448963 peopledatalabs-1.1.2/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    13638 1970-01-01 00:00:00.000000 peopledatalabs-1.1.2/setup.py
--rw-r--r--   0        0        0    13629 1970-01-01 00:00:00.000000 peopledatalabs-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/LICENSE
+-rw-r--r--   0        0        0    12222 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/README.md
+-rw-r--r--   0        0        0     1639 2023-05-01 23:34:09.985973 peopledatalabs-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     5612 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     1635 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      762 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2812 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      744 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      984 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5069 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2445 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      215 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4188 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      783 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2434 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1156 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      670 2023-05-01 23:34:09.989974 peopledatalabs-1.1.3/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    13629 1970-01-01 00:00:00.000000 peopledatalabs-1.1.3/PKG-INFO
```

### Comparing `peopledatalabs-1.1.2/LICENSE` & `peopledatalabs-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/README.md` & `peopledatalabs-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/pyproject.toml` & `peopledatalabs-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "1.1.2"
+version = "1.1.3"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
```

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-1.1.3/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/logger.py` & `peopledatalabs-1.1.3/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/main.py` & `peopledatalabs-1.1.3/src/peopledatalabs/main.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/models/__init__.py` & `peopledatalabs-1.1.3/src/peopledatalabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/models/company.py` & `peopledatalabs-1.1.3/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/models/person.py` & `peopledatalabs-1.1.3/src/peopledatalabs/models/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     name: Optional[Union[List[str], str]]
     phone: Optional[Union[List[str], str]]
     postal_code: Optional[Union[List[str], str]]
     profile: Optional[Union[List[str], str]]
     region: Optional[str]
     school: Optional[Union[List[str], str]]
     street_address: Optional[str]
+    pdl_id: Optional[str]
 
     @root_validator(pre=True)
     def at_least_one(cls, value):
         """
         Checks that at least one parameter is valued.
         """
         if not any(value.values()):
```

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/models/school.py` & `peopledatalabs-1.1.3/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/requests.py` & `peopledatalabs-1.1.3/src/peopledatalabs/requests.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/settings.py` & `peopledatalabs-1.1.3/src/peopledatalabs/settings.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/src/peopledatalabs/utils.py` & `peopledatalabs-1.1.3/src/peopledatalabs/utils.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.2/PKG-INFO` & `peopledatalabs-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 1.1.2
+Version: 1.1.3
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.7.2,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.2 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.3 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

