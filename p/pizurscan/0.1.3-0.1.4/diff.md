# Comparing `tmp/pizurscan-0.1.3.tar.gz` & `tmp/pizurscan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.3.tar", last modified: Mon May  1 13:02:13 2023, max compression
+gzip compressed data, was "pizurscan-0.1.4.tar", last modified: Tue May  2 09:21:23 2023, max compression
```

## Comparing `pizurscan-0.1.3.tar` & `pizurscan-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 13:02:13.407973 pizurscan-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 13:01:59.000000 pizurscan-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/pizurscan/
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/InputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/OutputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/PI_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/Scanners.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:01:59.000000 pizurscan-0.1.3/pizurscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/pizurscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 13:02:13.000000 pizurscan-0.1.3/pizurscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:02:13.407973 pizurscan-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 13:01:59.000000 pizurscan-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:02:13.407973 pizurscan-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-05-01 13:01:59.000000 pizurscan-0.1.3/tests/testclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:21:23.605000 pizurscan-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 09:21:23.605000 pizurscan-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 09:21:09.000000 pizurscan-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:21:23.601000 pizurscan-0.1.4/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-02 09:21:09.000000 pizurscan-0.1.4/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-02 09:21:09.000000 pizurscan-0.1.4/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-02 09:21:09.000000 pizurscan-0.1.4/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-02 09:21:09.000000 pizurscan-0.1.4/pizurscan/Scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 09:21:09.000000 pizurscan-0.1.4/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:21:23.605000 pizurscan-0.1.4/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 09:21:23.000000 pizurscan-0.1.4/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-02 09:21:23.000000 pizurscan-0.1.4/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:21:23.000000 pizurscan-0.1.4/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 09:21:23.000000 pizurscan-0.1.4/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 09:21:23.000000 pizurscan-0.1.4/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:21:23.605000 pizurscan-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-02 09:21:09.000000 pizurscan-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:21:23.605000 pizurscan-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-05-02 09:21:09.000000 pizurscan-0.1.4/tests/testclasses.py
```

### Comparing `pizurscan-0.1.3/PKG-INFO` & `pizurscan-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.3/README.md` & `pizurscan-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.3/pizurscan/InputProcessor.py` & `pizurscan-0.1.4/pizurscan/InputProcessor.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.3/pizurscan/OutputProcessor.py` & `pizurscan-0.1.4/pizurscan/OutputProcessor.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.3/pizurscan/PI_commands.py` & `pizurscan-0.1.4/pizurscan/PI_commands.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.3/pizurscan.egg-info/PKG-INFO` & `pizurscan-0.1.4/pizurscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.3/setup.py` & `pizurscan-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pizurscan",
-    version="0.1.3",
+    version="0.1.4",
     description="Library to interface PI controllers and Zurich lock-in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pizur-scanner.readthedocs.io/",
     author="Giacomo Rizzi",
     author_email="rizzigiacomo@pm.me",
     license="MIT",
@@ -30,9 +30,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: Microsoft :: Windows"
     ],
     packages=["pizurscan"],
     include_package_data=True,
-    install_requires=["numpy","json","math"]
+    install_requires=["numpy"]
 )
```

### Comparing `pizurscan-0.1.3/tests/testclasses.py` & `pizurscan-0.1.4/tests/testclasses.py`

 * *Files identical despite different names*

