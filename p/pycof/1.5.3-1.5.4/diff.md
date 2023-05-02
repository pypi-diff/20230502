# Comparing `tmp/pycof-1.5.3.tar.gz` & `tmp/pycof-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycof-1.5.3.tar", last modified: Thu Jan 26 16:13:12 2023, max compression
+gzip compressed data, was "pycof-1.5.4.tar", last modified: Tue May  2 11:43:45 2023, max compression
```

## Comparing `pycof-1.5.3.tar` & `pycof-1.5.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-01-26 16:13:12.886555 pycof-1.5.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.3/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-01-26 16:13:12.886555 pycof-1.5.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-01-26 16:13:12.886555 pycof-1.5.3/pycof/
--rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.3/pycof/data.py
--rw-r--r--   0 florian   (1000) florian   (1000)    30739 2023-01-01 14:48:35.000000 pycof-1.5.3/pycof/format.py
--rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.3/pycof/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11316 2022-09-11 09:44:36.000000 pycof-1.5.3/pycof/misc.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.3/pycof/sql.py
--rw-r--r--   0 florian   (1000) florian   (1000)    14352 2022-09-25 17:15:48.000000 pycof-1.5.3/pycof/sqlhelper.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-01-26 16:13:12.886555 pycof-1.5.3/pycof.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      286 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-01-26 16:13:12.000000 pycof-1.5.3/pycof.egg-info/top_level.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-01-26 16:13:12.886555 pycof-1.5.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      882 2022-09-25 17:55:08.000000 pycof-1.5.3/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)     1163 2023-01-26 16:13:12.000000 pycof-1.5.3/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.906039 pycof-1.5.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1071 2020-10-01 18:30:50.000000 pycof-1.5.4/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-05-02 11:43:45.906039 pycof-1.5.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     4067 2022-09-25 17:41:11.000000 pycof-1.5.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.895205 pycof-1.5.4/pycof/
+-rw-r--r--   0 florian   (1000) florian   (1000)      178 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14439 2023-01-26 16:12:36.000000 pycof-1.5.4/pycof/data.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    30739 2023-01-01 14:48:35.000000 pycof-1.5.4/pycof/format.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      182 2021-06-27 12:32:45.000000 pycof-1.5.4/pycof/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11316 2022-09-11 09:44:36.000000 pycof-1.5.4/pycof/misc.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10308 2022-09-25 17:49:57.000000 pycof-1.5.4/pycof/sql.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    14352 2022-09-25 17:15:48.000000 pycof-1.5.4/pycof/sqlhelper.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-02 11:43:45.895205 pycof-1.5.4/pycof.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     4540 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      300 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      313 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        6 2023-05-02 11:43:45.000000 pycof-1.5.4/pycof.egg-info/top_level.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-02 11:43:45.906039 pycof-1.5.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     1170 2023-03-12 10:48:27.000000 pycof-1.5.4/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     1216 2023-05-02 11:43:45.000000 pycof-1.5.4/setup_new.py
```

### Comparing `pycof-1.5.3/LICENSE` & `pycof-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/PKG-INFO` & `pycof-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.3/README.md` & `pycof-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof/data.py` & `pycof-1.5.4/pycof/data.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof/format.py` & `pycof-1.5.4/pycof/format.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof/misc.py` & `pycof-1.5.4/pycof/misc.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof/sql.py` & `pycof-1.5.4/pycof/sql.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof/sqlhelper.py` & `pycof-1.5.4/pycof/sqlhelper.py`

 * *Files identical despite different names*

### Comparing `pycof-1.5.3/pycof.egg-info/PKG-INFO` & `pycof-1.5.4/pycof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycof
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package for commonly used functions
 Home-page: https://www.florianfelice.com/pycof
 Author: Florian Felice
 Author-email: admin@florianfelice.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pycof-1.5.3/setup.py` & `pycof-1.5.4/setup_new.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="pycof",  # Replace with your own username
-    version="1.5.0",
+    name="pycof",
+    version="1.5.4",
     author="Florian Felice",
     author_email="admin@florianfelice.com",
     description="A package for commonly used functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/florianfelice/PYCOF",
+    url="https://www.florianfelice.com/pycof",
     packages=setuptools.find_packages(),
     install_requires=[
-        "pandas>=0.24.1",
-        "numpy>=1.16.3",
-        "psycopg2-binary>=2.7.4",
-        "pymysql>=0.9.3",
-        "tqdm>=4.35.0",
-        "sshtunnel>=0.3.1",
-    ],
+          "pandas>=0.24.1",
+          "numpy>=1.16.3",
+          "psycopg2-binary>=2.7.4",
+          "pymysql>=0.9.3",
+          "tqdm>=4.35.0",
+          "boto3>=1.16.19",
+          "xlrd>=1.2.0",
+          "matplotlib>=3.1.1",
+          "sshtunnel>=0.3.1",
+          "dateparser>=1.0.0",
+          "google-api-python-client>=1.12.8",
+          "google-auth-httplib2>=0.0.4",
+          "google-auth-oauthlib>=0.4.2",
+          "google-auth>=1.24.0",
+          "httplib2>=0.18.1",
+          "pyarrow>=11.0.0",
+          "bs4>=0.0.1"
+      ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
+)
```

