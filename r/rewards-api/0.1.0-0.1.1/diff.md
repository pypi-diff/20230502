# Comparing `tmp/rewards_api-0.1.0.tar.gz` & `tmp/rewards_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards_api-0.1.0.tar", last modified: Sat Apr 22 15:29:41 2023, max compression
+gzip compressed data, was "rewards_api-0.1.1.tar", last modified: Tue May  2 15:41:18 2023, max compression
```

## Comparing `rewards_api-0.1.0.tar` & `rewards_api-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 15:29:41.015581 rewards_api-0.1.0/PKG-INFO
--rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.1.0/README.md
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.1.0/pyproject.toml
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/rewards_api/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      214 2023-04-22 15:13:14.000000 rewards_api-0.1.0/rewards_api/__init__.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 15:14:35.000000 rewards_api-0.1.0/rewards_api/cli.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.1.0/rewards_api/cli_args.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1058 2023-04-22 15:12:26.000000 rewards_api-0.1.0/rewards_api/config.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    10809 2023-04-22 15:29:07.000000 rewards_api-0.1.0/rewards_api/main.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    11132 2023-04-22 15:11:49.000000 rewards_api-0.1.0/rewards_api/streamer.py
--rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.1.0/rewards_api/utils.py
-drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-04-22 15:29:41.015581 rewards_api-0.1.0/rewards_api.egg-info/
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/PKG-INFO
--rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/SOURCES.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/dependency_links.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/entry_points.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       99 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/requires.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-04-22 15:29:40.000000 rewards_api-0.1.0/rewards_api.egg-info/top_level.txt
--rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-04-22 15:29:41.015581 rewards_api-0.1.0/setup.cfg
--rw-rw-r--   0 anindya   (1000) anindya   (1000)     1054 2023-04-22 15:29:39.000000 rewards_api-0.1.0/setup.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 15:41:18.544470 rewards_api-0.1.1/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-05-02 15:41:18.544470 rewards_api-0.1.1/PKG-INFO
+-rw-r--r--   0 anindya   (1000) anindya   (1000)     5582 2023-04-21 05:26:09.000000 rewards_api-0.1.1/README.md
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      623 2023-04-21 14:36:16.000000 rewards_api-0.1.1/pyproject.toml
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 15:41:18.544470 rewards_api-0.1.1/rewards_api/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      214 2023-04-22 15:13:14.000000 rewards_api-0.1.1/rewards_api/__init__.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      239 2023-04-22 15:14:35.000000 rewards_api-0.1.1/rewards_api/cli.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      565 2023-04-22 00:31:16.000000 rewards_api-0.1.1/rewards_api/cli_args.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1058 2023-04-22 15:12:26.000000 rewards_api-0.1.1/rewards_api/config.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    10809 2023-04-22 15:29:07.000000 rewards_api-0.1.1/rewards_api/main.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    11132 2023-04-22 15:11:49.000000 rewards_api-0.1.1/rewards_api/streamer.py
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)    12496 2023-04-22 04:08:17.000000 rewards_api-0.1.1/rewards_api/utils.py
+drwxrwxr-x   0 anindya   (1000) anindya   (1000)        0 2023-05-02 15:41:18.544470 rewards_api-0.1.1/rewards_api.egg-info/
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     6078 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/PKG-INFO
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)      399 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)        1 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       63 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/entry_points.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       90 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/requires.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       12 2023-05-02 15:41:18.000000 rewards_api-0.1.1/rewards_api.egg-info/top_level.txt
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)       38 2023-05-02 15:41:18.544470 rewards_api-0.1.1/setup.cfg
+-rw-rw-r--   0 anindya   (1000) anindya   (1000)     1042 2023-05-02 15:41:17.000000 rewards_api-0.1.1/setup.py
```

### Comparing `rewards_api-0.1.0/PKG-INFO` & `rewards_api-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.1.0/README.md` & `rewards_api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/pyproject.toml` & `rewards_api-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api/cli_args.py` & `rewards_api-0.1.1/rewards_api/cli_args.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api/config.py` & `rewards_api-0.1.1/rewards_api/config.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api/main.py` & `rewards_api-0.1.1/rewards_api/main.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api/streamer.py` & `rewards_api-0.1.1/rewards_api/streamer.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api/utils.py` & `rewards_api-0.1.1/rewards_api/utils.py`

 * *Files identical despite different names*

### Comparing `rewards_api-0.1.0/rewards_api.egg-info/PKG-INFO` & `rewards_api-0.1.1/rewards_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: rewards api cli package for starting the local rewards server
 Home-page: https://github.com/rewards-ai/rewards-api/tree/latest
 Author: rewards.ai
 Author-email: proanindyadeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rewards_api-0.1.0/setup.py` & `rewards_api-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fhand:
     long_description = fhand.read()
 
 setuptools.setup(
     name="rewards_api",
-    version="0.1.0",
+    version="0.1.1",
     author="rewards.ai",
     author_email="proanindyadeep@gmail.com",
     description="rewards api cli package for starting the local rewards server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rewards-ai/rewards-api/tree/latest",
     
@@ -18,15 +18,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "rewards-envs", 
         "rewards-experimental", 
         "torch", "opencv-python", 
-        "flask", "flask_cors", "flasgger", 
+        "flask", "flask_cors", 
         "boto3", "Flask[async]"
         ],
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "start-rewards-server = rewards_api.cli:main",
```

