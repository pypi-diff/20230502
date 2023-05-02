# Comparing `tmp/sdk-api-0.2.0.tar.gz` & `tmp/sdk-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk-api-0.2.0.tar", last modified: Wed Feb 15 10:39:50 2023, max compression
+gzip compressed data, was "sdk-api-0.2.1.tar", last modified: Tue May  2 10:57:07 2023, max compression
```

## Comparing `sdk-api-0.2.0.tar` & `sdk-api-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-02-15 10:39:50.634850 sdk-api-0.2.0/
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)    11358 2023-02-02 15:25:13.000000 sdk-api-0.2.0/LICENSE
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     3775 2023-02-15 10:39:50.633850 sdk-api-0.2.0/PKG-INFO
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)      442 2023-02-05 13:42:49.000000 sdk-api-0.2.0/README.md
-drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-02-15 10:39:50.530998 sdk-api-0.2.0/docs/
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     3084 2023-02-15 10:34:58.000000 sdk-api-0.2.0/docs/README_PACKAGE.md
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     1349 2023-02-06 07:17:04.000000 sdk-api-0.2.0/pyproject.toml
-drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-02-15 10:39:50.574469 sdk-api-0.2.0/sdk/
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)       20 2023-02-02 15:24:51.000000 sdk-api-0.2.0/sdk/__init__.py
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     2669 2023-02-03 14:22:25.000000 sdk-api-0.2.0/sdk/_internal_utils.py
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)    14939 2023-02-15 10:29:31.000000 sdk-api-0.2.0/sdk/api.py
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     1159 2023-02-05 09:55:28.000000 sdk-api-0.2.0/sdk/config.py
-drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-02-15 10:39:50.621850 sdk-api-0.2.0/sdk_api.egg-info/
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)     3775 2023-02-15 10:39:50.000000 sdk-api-0.2.0/sdk_api.egg-info/PKG-INFO
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)      273 2023-02-15 10:39:50.000000 sdk-api-0.2.0/sdk_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)        1 2023-02-15 10:39:50.000000 sdk-api-0.2.0/sdk_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)      113 2023-02-15 10:39:50.000000 sdk-api-0.2.0/sdk_api.egg-info/requires.txt
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)        4 2023-02-15 10:39:50.000000 sdk-api-0.2.0/sdk_api.egg-info/top_level.txt
--rwxrwxrwx   0 ub422     (1000) ub422     (1000)       38 2023-02-15 10:39:50.635851 sdk-api-0.2.0/setup.cfg
+drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-05-02 10:57:07.276331 sdk-api-0.2.1/
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)    11358 2023-05-02 10:25:03.000000 sdk-api-0.2.1/LICENSE
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     4532 2023-05-02 10:57:07.273330 sdk-api-0.2.1/PKG-INFO
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)      518 2023-05-02 10:48:46.000000 sdk-api-0.2.1/README.md
+drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-05-02 10:57:07.065592 sdk-api-0.2.1/docs/
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     3841 2023-05-02 10:45:40.000000 sdk-api-0.2.1/docs/README_PACKAGE.md
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     1349 2023-05-02 10:53:02.000000 sdk-api-0.2.1/pyproject.toml
+drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-05-02 10:57:07.154176 sdk-api-0.2.1/sdk/
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)       20 2023-05-02 10:25:03.000000 sdk-api-0.2.1/sdk/__init__.py
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     2669 2023-05-02 10:25:03.000000 sdk-api-0.2.1/sdk/_internal_utils.py
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)    17078 2023-05-02 10:45:40.000000 sdk-api-0.2.1/sdk/api.py
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     1159 2023-05-02 10:25:03.000000 sdk-api-0.2.1/sdk/config.py
+drwxrwxrwx   0 ub422     (1000) ub422     (1000)        0 2023-05-02 10:57:07.250330 sdk-api-0.2.1/sdk_api.egg-info/
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)     4532 2023-05-02 10:57:06.000000 sdk-api-0.2.1/sdk_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)      273 2023-05-02 10:57:06.000000 sdk-api-0.2.1/sdk_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)        1 2023-05-02 10:57:06.000000 sdk-api-0.2.1/sdk_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)      113 2023-05-02 10:57:06.000000 sdk-api-0.2.1/sdk_api.egg-info/requires.txt
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)        4 2023-05-02 10:57:06.000000 sdk-api-0.2.1/sdk_api.egg-info/top_level.txt
+-rwxrwxrwx   0 ub422     (1000) ub422     (1000)       38 2023-05-02 10:57:07.277330 sdk-api-0.2.1/setup.cfg
```

### Comparing `sdk-api-0.2.0/LICENSE` & `sdk-api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdk-api-0.2.0/PKG-INFO` & `sdk-api-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python API wrapping services of the Superb Data Kraken (SDK)
 Author-email: "Team SDK | e:fs TechHub GmbH" <sdk@efs-techhub.com>
 Maintainer: David Eichiner
 Maintainer-email: david.eichiner@efs-techhub.com
 License: Apache-2.0
 Keywords: sdk,api,superb data kraken,data management,wrapper,api-wrapper
 Classifier: Programming Language :: Python :: 3
@@ -128,14 +128,44 @@
    }
 ]
 index_name = "index" 
 client.index_documents(documents, index_name)
 ``` 
 The (optional) field **_id** is parsed and used as document id to index to opensearch.
 
+List all indices filtered by organization, space and type accessible with given credentials
+
+``` python
+client.index_filter_by_space("my-organization", "my-space", "index-type")
+```
+
+use **.\*** instead of **my_space** to get indices from all spaces in the given organization
+
+**index_type** is either **ANALYSIS** or **MEASUREMENTS**
+
+
+Create an application index
+
+``` python
+application_index = {
+   "organizationName": "my-organization",
+   "spaceName": "my-space",
+   "customName": "my-application-index",
+   "indexType": "ANALYSIS",
+   "mappings": {}
+}
+client.application_index_create(application_index)
+```
+
+Delete an application index by name
+
+``` python
+client.application_index_delete("my-organization_my-space_analysis_my-application-index")
+```
+
 
 #### Storage
 
 List files in Storage
 
 ``` python
 files = client.storage_list_blobs(org_name, space_name)
```

### Comparing `sdk-api-0.2.0/docs/README_PACKAGE.md` & `sdk-api-0.2.1/sdk_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sdk-api
+Version: 0.2.1
+Summary: A Python API wrapping services of the Superb Data Kraken (SDK)
+Author-email: "Team SDK | e:fs TechHub GmbH" <sdk@efs-techhub.com>
+Maintainer: David Eichiner
+Maintainer-email: david.eichiner@efs-techhub.com
+License: Apache-2.0
+Keywords: sdk,api,superb data kraken,data management,wrapper,api-wrapper
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SDK-API
 
 **SDK-API** is a simple library to access various services of the *Superb Data Kraken (SDK)*  platform.
 It abstracts accessing services and resources of the SDK with a Python client object managing Authorization, Fetching and Indexing data.
 
 It is primarily intended for use in an Jupyter Hub environment within
 the platform itself, but can be configured for different environments as well.
@@ -110,14 +128,44 @@
    }
 ]
 index_name = "index" 
 client.index_documents(documents, index_name)
 ``` 
 The (optional) field **_id** is parsed and used as document id to index to opensearch.
 
+List all indices filtered by organization, space and type accessible with given credentials
+
+``` python
+client.index_filter_by_space("my-organization", "my-space", "index-type")
+```
+
+use **.\*** instead of **my_space** to get indices from all spaces in the given organization
+
+**index_type** is either **ANALYSIS** or **MEASUREMENTS**
+
+
+Create an application index
+
+``` python
+application_index = {
+   "organizationName": "my-organization",
+   "spaceName": "my-space",
+   "customName": "my-application-index",
+   "indexType": "ANALYSIS",
+   "mappings": {}
+}
+client.application_index_create(application_index)
+```
+
+Delete an application index by name
+
+``` python
+client.application_index_delete("my-organization_my-space_analysis_my-application-index")
+```
+
 
 #### Storage
 
 List files in Storage
 
 ``` python
 files = client.storage_list_blobs(org_name, space_name)
```

### Comparing `sdk-api-0.2.0/pyproject.toml` & `sdk-api-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires = ['setuptools']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdk-api"
 description = "A Python API wrapping services of the Superb Data Kraken (SDK)"
 requires-python = ">=3.7"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Team SDK | e:fs TechHub GmbH", email = "sdk@efs-techhub.com" },
 ]
 maintainers = [
     { email = "david.eichiner@efs-techhub.com" },
     { name = "David Eichiner" }
 ]
```

### Comparing `sdk-api-0.2.0/sdk/_internal_utils.py` & `sdk-api-0.2.1/sdk/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `sdk-api-0.2.0/sdk/api.py` & `sdk-api-0.2.1/sdk/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         :param chunk_size:
         :param documents:
             list of dictionaries to index
         :param index_name:
             index name to index documents to
         :return:
         """
-        url = f'https://{self._env.domain}/elastic/api/_bulk'
+        url = f'https://{self._env.domain}/elastic/api/'
         es = Elasticsearch(url, use_ssl=True, headers={"Authorization": "Bearer " + self._token_holder.get_token()}, timeout=timeout)
 
         # Create data for bulk api
         actions = [
             {
                 "_index": index_name,
                 "_id": entry.pop('_id') if '_id' in entry else None,
@@ -289,14 +289,62 @@
         ]
 
         # Bulk ingest data
         bulk(es, actions, chunk_size=chunk_size)
 
         # Close Elasticsearch
         es.close()
+    
+
+    def index_filter_by_space(self, organization_name: str, space_name: str, index_type: str) -> list:
+        """
+        Filtering index by organization, space and index type
+        :organization_name:
+            name of the organization
+        :space_name:
+            name of the space '*' for all spaces in the organization
+        :index_type:
+            type of the index, analysis or measurment
+        """
+        headers = {"Authorization": f"Bearer {self._token_holder.get_token()}"}
+        url = f'https://{self._env.domain}/search/{self._env.api_version}/index?filter={organization_name}_{space_name}_{index_type.lower()}.*'
+        #print(f"{organization_name}_{space_name}_{index_type.lower()}_.*")
+        response = requests.get(url, headers=headers)
+        res = response.json()
+        
+        return res
+
+    def application_index_create(self, application_index: dict) -> str:
+        """
+        Creates an application index
+        :application_index:
+            dictionary defining application index properties
+        :return:
+            response body of the http request
+        """
+        url = f'https://{self._env.domain}/metadata/{self._env.api_version}/application-index'
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f'Bearer {self._token_holder.get_token()}'
+        }
+        response = requests.post(url, json=application_index, headers=headers)
+        response.raise_for_status()
+        # not response.json(), because the endpoint gives me back a string. With json() i get a JSONDecoderError
+        return response.text
+    
+    def application_index_delete(self, application_index_name: str) -> None:
+        """
+        Deletes an application index by name
+        :application_index_name:
+            name of the application index
+        """
+        url = f'https://{self._env.domain}/metadata/{self._env.api_version}/application-index/{application_index_name}'
+        headers = {"Authorization": f'Bearer {self._token_holder.get_token()}'}
+        response = requests.delete(url, headers=headers)
+        response.raise_for_status()
 
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ storage ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     def storage_list_blobs(self, organization: str, space: str) -> List[str]:
         """
         Lists blobs in storage container
         :param organization:
         :param space:
```

### Comparing `sdk-api-0.2.0/sdk/config.py` & `sdk-api-0.2.1/sdk/config.py`

 * *Files identical despite different names*

