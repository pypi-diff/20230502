# Comparing `tmp/servicepytan-0.3.0.tar.gz` & `tmp/servicepytan-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicepytan-0.3.0.tar", last modified: Fri Nov 25 13:55:07 2022, max compression
+gzip compressed data, was "servicepytan-0.3.1.tar", last modified: Tue May  2 13:18:42 2023, max compression
```

## Comparing `servicepytan-0.3.0.tar` & `servicepytan-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-11-25 13:55:07.901344 servicepytan-0.3.0/
--rw-rw-rw-   0        0        0      174 2022-09-07 01:39:30.000000 servicepytan-0.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3724 2022-09-07 01:39:30.000000 servicepytan-0.3.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2022-09-07 01:39:30.000000 servicepytan-0.3.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1094 2022-09-07 01:39:30.000000 servicepytan-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      273 2022-09-07 01:39:30.000000 servicepytan-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2025 2022-11-25 13:55:07.901344 servicepytan-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2022-11-25 13:47:40.000000 servicepytan-0.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-25 13:55:07.877867 servicepytan-0.3.0/docs/
--rw-rw-rw-   0        0        0      654 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/Makefile
--rw-rw-rw-   0        0        0     2103 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/conf.py
--rw-rw-rw-   0        0        0     4259 2022-11-25 13:42:00.000000 servicepytan-0.3.0/docs/index.rst
--rwxrwxrwx   0        0        0      800 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/make.bat
--rw-rw-rw-   0        0        0       80 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/modules.rst
--rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.auth.rst
--rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.data.rst
--rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.dates.rst
--rw-rw-rw-   0        0        0      158 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.requests.rst
--rw-rw-rw-   0        0        0      358 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.rst
--rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.0/docs/servicepytan.utils.rst
-drwxrwxrwx   0        0        0        0 2022-11-25 13:55:07.886382 servicepytan-0.3.0/servicepytan/
--rw-rw-rw-   0        0        0      952 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/__init__.py
--rw-rw-rw-   0        0        0     1879 2022-09-07 01:39:30.000000 servicepytan-0.3.0/servicepytan/_dates.py
--rw-rw-rw-   0        0        0     4278 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/auth.py
--rw-rw-rw-   0        0        0     4669 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/data.py
--rw-rw-rw-   0        0        0     5271 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/reports.py
--rw-rw-rw-   0        0        0     4414 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/requests.py
--rw-rw-rw-   0        0        0      257 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/summary.py
--rw-rw-rw-   0        0        0     4895 2022-11-25 13:42:00.000000 servicepytan-0.3.0/servicepytan/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-25 13:55:07.897331 servicepytan-0.3.0/servicepytan.egg-info/
--rw-rw-rw-   0        0        0     2025 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      809 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-10-25 17:52:15.000000 servicepytan-0.3.0/servicepytan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-25 13:55:07.000000 servicepytan-0.3.0/servicepytan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      407 2022-11-25 13:55:07.902342 servicepytan-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1553 2022-11-25 13:42:00.000000 servicepytan-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-25 13:55:07.900349 servicepytan-0.3.0/tests/
--rw-rw-rw-   0        0        0       43 2022-09-07 01:39:30.000000 servicepytan-0.3.0/tests/__init__.py
--rw-rw-rw-   0        0        0      920 2022-09-07 01:39:30.000000 servicepytan-0.3.0/tests/test_servicepytan.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.486563 servicepytan-0.3.1/
+-rw-rw-rw-   0        0        0      174 2022-09-07 01:39:30.000000 servicepytan-0.3.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3724 2022-09-07 01:39:30.000000 servicepytan-0.3.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2022-09-07 01:39:30.000000 servicepytan-0.3.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1094 2022-09-07 01:39:30.000000 servicepytan-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2022-09-07 01:39:30.000000 servicepytan-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2025 2023-05-02 13:18:42.486563 servicepytan-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1152 2022-11-25 13:47:40.000000 servicepytan-0.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.432902 servicepytan-0.3.1/docs/
+-rw-rw-rw-   0        0        0      654 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/Makefile
+-rw-rw-rw-   0        0        0     2103 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/conf.py
+-rw-rw-rw-   0        0        0     4259 2022-11-25 13:42:00.000000 servicepytan-0.3.1/docs/index.rst
+-rwxrwxrwx   0        0        0      800 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/make.bat
+-rw-rw-rw-   0        0        0       80 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/modules.rst
+-rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.auth.rst
+-rw-rw-rw-   0        0        0      146 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.data.rst
+-rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.dates.rst
+-rw-rw-rw-   0        0        0      158 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.requests.rst
+-rw-rw-rw-   0        0        0      358 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.rst
+-rw-rw-rw-   0        0        0      149 2022-09-07 01:39:30.000000 servicepytan-0.3.1/docs/servicepytan.utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.451059 servicepytan-0.3.1/servicepytan/
+-rw-rw-rw-   0        0        0      952 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/__init__.py
+-rw-rw-rw-   0        0        0     1879 2022-09-07 01:39:30.000000 servicepytan-0.3.1/servicepytan/_dates.py
+-rw-rw-rw-   0        0        0     4278 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/auth.py
+-rw-rw-rw-   0        0        0     4669 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/data.py
+-rw-rw-rw-   0        0        0     5475 2023-05-02 13:17:32.000000 servicepytan-0.3.1/servicepytan/reports.py
+-rw-rw-rw-   0        0        0     4414 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/requests.py
+-rw-rw-rw-   0        0        0      257 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/summary.py
+-rw-rw-rw-   0        0        0     4895 2022-11-25 13:42:00.000000 servicepytan-0.3.1/servicepytan/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.482137 servicepytan-0.3.1/servicepytan.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      809 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-10-25 17:52:15.000000 servicepytan-0.3.1/servicepytan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       62 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-02 13:18:42.000000 servicepytan-0.3.1/servicepytan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      407 2023-05-02 13:18:42.489408 servicepytan-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1553 2023-05-02 13:18:04.000000 servicepytan-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 13:18:42.485561 servicepytan-0.3.1/tests/
+-rw-rw-rw-   0        0        0       43 2022-09-07 01:39:30.000000 servicepytan-0.3.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      920 2022-09-07 01:39:30.000000 servicepytan-0.3.1/tests/test_servicepytan.py
```

### Comparing `servicepytan-0.3.0/CONTRIBUTING.rst` & `servicepytan-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/LICENSE` & `servicepytan-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/PKG-INFO` & `servicepytan-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicepytan
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Library to make it easier to interact with the ServiceTitan API v2
 Home-page: https://github.com/elliotpalmer/servicepytan
 Author: Elliot Palmer
 Author-email: elliot@ecoplumbers.com
 License: MIT license
 Keywords: servicepytan
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `servicepytan-0.3.0/README.rst` & `servicepytan-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/docs/Makefile` & `servicepytan-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/docs/conf.py` & `servicepytan-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/docs/index.rst` & `servicepytan-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/docs/make.bat` & `servicepytan-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/__init__.py` & `servicepytan-0.3.1/servicepytan/__init__.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/_dates.py` & `servicepytan-0.3.1/servicepytan/_dates.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/auth.py` & `servicepytan-0.3.1/servicepytan/auth.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/data.py` & `servicepytan-0.3.1/servicepytan/data.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/reports.py` & `servicepytan-0.3.1/servicepytan/reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,31 +59,36 @@
     return request_json_with_retry(url, conn=self.conn)
 
   def show_param_types(self):
     """show parameter types"""
     for param in self.metadata["parameters"]:
       dynamic_set_id = ""
       required = "[ ]"
+      accepted_values = []
       if param["isRequired"]:
         required = "[*]"
       if param['acceptValues']:
         dynamic_set_id = f" (dynamicSetId: {param['acceptValues']['dynamicSetId']})"
+        if param['acceptValues']['values']:
+          accepted_values = param['acceptValues']['values']
       print(f"{required} - {param['name']}: {param['dataType']}, {dynamic_set_id}")
+      for value in accepted_values:
+        print(f"  - {value}")
 
   def get_data(self, params="", page=1, page_size=5000):
     """get report data"""
     if params == "":
       params = self.params
     options = {"page": page, "pageSize": page_size, "includeTotal": True}
     endpoint = f"report-category/{self.category}/reports/{self.report_id}/data"
     url = endpoint_url("reporting",endpoint, conn=self.conn)
     return request_json_with_retry(url, options=options, json_payload=params, 
               conn=self.conn, request_type="POST")
   
-  def get_all_data(self, params="", page_size=5000):
+  def get_all_data(self, params="", page_size=5000, timeout_min=60):
     """get all report data"""
     page = 1
     data = []
     fields = []
     if params == "":
       params = self.params
     print("Getting first page of data...")
@@ -92,15 +97,15 @@
     fields.extend(response["fields"])
     total = response["totalCount"]
     has_more = response["hasMore"]
     print(f"Retrieved {len(data)} of {total} records...")
     requests_needed = math.ceil(total / page_size)
     mins_to_complete = requests_needed * 5
     updated_page_size = page_size
-    if mins_to_complete > 60 or requests_needed > 2:
+    if mins_to_complete > timeout_min:
       init_page_size = updated_page_size
       if page_size < 5000 and math.ceil(total / 5000) < 12:
         print("Setting page size to 5000 to speed up report retrieval...")
         updated_page_size = 5000
         requests_needed = 1 + math.ceil((total - init_page_size) / updated_page_size)
       else:
         print(f"This request will take at least {mins_to_complete/60} hours to complete.")
```

### Comparing `servicepytan-0.3.0/servicepytan/requests.py` & `servicepytan-0.3.1/servicepytan/requests.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan/utils.py` & `servicepytan-0.3.1/servicepytan/utils.py`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/servicepytan.egg-info/PKG-INFO` & `servicepytan-0.3.1/servicepytan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicepytan
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Library to make it easier to interact with the ServiceTitan API v2
 Home-page: https://github.com/elliotpalmer/servicepytan
 Author: Elliot Palmer
 Author-email: elliot@ecoplumbers.com
 License: MIT license
 Keywords: servicepytan
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `servicepytan-0.3.0/servicepytan.egg-info/SOURCES.txt` & `servicepytan-0.3.1/servicepytan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servicepytan-0.3.0/setup.py` & `servicepytan-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='servicepytan',
     name='servicepytan',
     packages=find_packages(include=['servicepytan', 'servicepytan.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/elliotpalmer/servicepytan',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

### Comparing `servicepytan-0.3.0/tests/test_servicepytan.py` & `servicepytan-0.3.1/tests/test_servicepytan.py`

 * *Files identical despite different names*

