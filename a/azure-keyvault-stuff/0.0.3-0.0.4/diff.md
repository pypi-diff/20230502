# Comparing `tmp/azure-keyvault-stuff-0.0.3.tar.gz` & `tmp/azure-keyvault-stuff-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-keyvault-stuff-0.0.3.tar", last modified: Fri Apr 28 14:34:54 2023, max compression
+gzip compressed data, was "azure-keyvault-stuff-0.0.4.tar", last modified: Tue May  2 09:15:40 2023, max compression
```

## Comparing `azure-keyvault-stuff-0.0.3.tar` & `azure-keyvault-stuff-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 14:34:54.664193 azure-keyvault-stuff-0.0.3/
--rw-rw-rw-   0        0        0     1094 2023-04-28 12:59:23.000000 azure-keyvault-stuff-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1422 2023-04-28 14:34:54.663189 azure-keyvault-stuff-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-28 14:29:57.000000 azure-keyvault-stuff-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 14:34:54.665188 azure-keyvault-stuff-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1207 2023-04-28 14:34:50.000000 azure-keyvault-stuff-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 14:34:54.638188 azure-keyvault-stuff-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 14:34:54.661268 azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/
--rw-rw-rw-   0        0        0     1422 2023-04-28 14:34:54.000000 azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-28 14:34:54.000000 azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 14:34:54.000000 azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-28 14:34:54.000000 azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 09:15:40.510059 azure-keyvault-stuff-0.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-04-28 12:59:23.000000 azure-keyvault-stuff-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1384 2023-05-02 09:15:40.507050 azure-keyvault-stuff-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-05-02 09:06:45.000000 azure-keyvault-stuff-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-02 09:15:40.511049 azure-keyvault-stuff-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-02 09:09:42.000000 azure-keyvault-stuff-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 09:15:40.494051 azure-keyvault-stuff-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 09:15:40.504054 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/
+-rw-rw-rw-   0        0        0     1384 2023-05-02 09:15:40.000000 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-02 09:15:40.000000 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 09:15:40.000000 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 09:15:40.000000 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1798 2023-04-28 12:56:45.000000 azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.py
```

### Comparing `azure-keyvault-stuff-0.0.3/LICENSE` & `azure-keyvault-stuff-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-keyvault-stuff-0.0.3/PKG-INFO` & `azure-keyvault-stuff-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-stuff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Key Vault Helper Package
 Home-page: https://github.com/george-oconnor/azure-keyvault-stuff
 Author: george.oconnor (George O' Connor)
 Author-email: <george@georgestools.com>
-Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials,azure.identity.DefaultAzureCredential()
+Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,20 +18,20 @@
 
 A package that provides functionality for interacting with an Azure Keyvault
 
 ## Installation
 
 Run the following to install the package:
 
-``python -m pip install azure-keyring-stuff``
+``python -m pip install azure-keyvault-stuff``
 
 ## Usage
 
 ```python
-from azure_keyring_stuff import getClient, getSecret, setSecret, deleteSecret
+from azure_keyvault_stuff import getClient, getSecret, setSecret, deleteSecret
 from azure.identity import DefaultAzureCredential
 
 client = getClient(vault_name="VAULT_NAME", credential=DefaultAzureCredential())
 
 secret = getSecret(client=client, secret_name="SECRET_NAME")
 
 new_secret = setSecret(client=client, secret_name="SECRET_NAME", secret_value="SECRET_VALUE")
```

### Comparing `azure-keyvault-stuff-0.0.3/README.md` & `azure-keyvault-stuff-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 A package that provides functionality for interacting with an Azure Keyvault
 
 ## Installation
 
 Run the following to install the package:
 
-``python -m pip install azure-keyring-stuff``
+``python -m pip install azure-keyvault-stuff``
 
 ## Usage
 
 ```python
-from azure_keyring_stuff import getClient, getSecret, setSecret, deleteSecret
+from azure_keyvault_stuff import getClient, getSecret, setSecret, deleteSecret
 from azure.identity import DefaultAzureCredential
 
 client = getClient(vault_name="VAULT_NAME", credential=DefaultAzureCredential())
 
 secret = getSecret(client=client, secret_name="SECRET_NAME")
 
 new_secret = setSecret(client=client, secret_name="SECRET_NAME", secret_value="SECRET_VALUE")
```

### Comparing `azure-keyvault-stuff-0.0.3/setup.py` & `azure-keyvault-stuff-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Azure Key Vault Helper Package'
 LONG_DESCRIPTION = 'A package that provides helper functions for interacting with Azure Key Vault.'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setting up
@@ -16,15 +16,15 @@
     author_email="<george@georgestools.com>",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["azure_keyvault_stuff"],
     package_dir={'': 'src'},
     install_requires=[],
-    keywords=['python', 'azure', 'keyvault', 'helper', 'secret', 'secrets', 'client', 'get', 'set', 'delete', 'vault', 'value', 'values', 'credential', 'credentials', 'azure.identity.DefaultAzureCredential()'],
+    keywords=['python', 'azure', 'keyvault', 'helper', 'secret', 'secrets', 'client', 'get', 'set', 'delete', 'vault', 'value', 'values', 'credential', 'credentials'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License"
     ]
```

### Comparing `azure-keyvault-stuff-0.0.3/src/azure_keyvault_stuff.egg-info/PKG-INFO` & `azure-keyvault-stuff-0.0.4/src/azure_keyvault_stuff.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-stuff
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Key Vault Helper Package
 Home-page: https://github.com/george-oconnor/azure-keyvault-stuff
 Author: george.oconnor (George O' Connor)
 Author-email: <george@georgestools.com>
-Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials,azure.identity.DefaultAzureCredential()
+Keywords: python,azure,keyvault,helper,secret,secrets,client,get,set,delete,vault,value,values,credential,credentials
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,20 +18,20 @@
 
 A package that provides functionality for interacting with an Azure Keyvault
 
 ## Installation
 
 Run the following to install the package:
 
-``python -m pip install azure-keyring-stuff``
+``python -m pip install azure-keyvault-stuff``
 
 ## Usage
 
 ```python
-from azure_keyring_stuff import getClient, getSecret, setSecret, deleteSecret
+from azure_keyvault_stuff import getClient, getSecret, setSecret, deleteSecret
 from azure.identity import DefaultAzureCredential
 
 client = getClient(vault_name="VAULT_NAME", credential=DefaultAzureCredential())
 
 secret = getSecret(client=client, secret_name="SECRET_NAME")
 
 new_secret = setSecret(client=client, secret_name="SECRET_NAME", secret_value="SECRET_VALUE")
```

