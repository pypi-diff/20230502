# Comparing `tmp/pycrtsh-0.3.8.tar.gz` & `tmp/pycrtsh-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrtsh-0.3.8.tar", last modified: Sat Apr 16 00:12:26 2022, max compression
+gzip compressed data, was "pycrtsh-0.3.9.tar", last modified: Mon Jun 27 17:46:40 2022, max compression
```

## Comparing `pycrtsh-0.3.8.tar` & `pycrtsh-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-04-16 00:12:26.030853 pycrtsh-0.3.8/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     1060 2021-03-28 19:41:49.000000 pycrtsh-0.3.8/LICENSE
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5581 2022-04-16 00:12:26.030853 pycrtsh-0.3.8/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5118 2022-04-15 09:07:49.000000 pycrtsh-0.3.8/README.md
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-04-16 00:12:26.030853 pycrtsh-0.3.8/pycrtsh/
--rw-r--r--   0 etienne   (1000) etienne   (1000)       74 2022-04-12 16:02:33.000000 pycrtsh-0.3.8/pycrtsh/__init__.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     9022 2022-04-16 00:08:43.000000 pycrtsh-0.3.8/pycrtsh/api.py
--rw-r--r--   0 etienne   (1000) etienne   (1000)     2103 2021-03-28 19:41:49.000000 pycrtsh-0.3.8/pycrtsh/cli.py
-drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-04-16 00:12:26.030853 pycrtsh-0.3.8/pycrtsh.egg-info/
--rw-r--r--   0 etienne   (1000) etienne   (1000)     5581 2022-04-16 00:12:25.000000 pycrtsh-0.3.8/pycrtsh.egg-info/PKG-INFO
--rw-r--r--   0 etienne   (1000) etienne   (1000)      264 2022-04-16 00:12:26.000000 pycrtsh-0.3.8/pycrtsh.egg-info/SOURCES.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2022-04-16 00:12:25.000000 pycrtsh-0.3.8/pycrtsh.egg-info/dependency_links.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       44 2022-04-16 00:12:25.000000 pycrtsh-0.3.8/pycrtsh.egg-info/entry_points.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       60 2022-04-16 00:12:25.000000 pycrtsh-0.3.8/pycrtsh.egg-info/requires.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)        8 2022-04-16 00:12:25.000000 pycrtsh-0.3.8/pycrtsh.egg-info/top_level.txt
--rw-r--r--   0 etienne   (1000) etienne   (1000)       38 2022-04-16 00:12:26.030853 pycrtsh-0.3.8/setup.cfg
--rw-r--r--   0 etienne   (1000) etienne   (1000)      828 2022-04-16 00:12:15.000000 pycrtsh-0.3.8/setup.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-06-27 17:46:40.274372 pycrtsh-0.3.9/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     1060 2021-03-28 19:41:49.000000 pycrtsh-0.3.9/LICENSE
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5581 2022-06-27 17:46:40.270372 pycrtsh-0.3.9/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5118 2022-04-15 09:07:49.000000 pycrtsh-0.3.9/README.md
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-06-27 17:46:40.270372 pycrtsh-0.3.9/pycrtsh/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       74 2022-04-12 16:02:33.000000 pycrtsh-0.3.9/pycrtsh/__init__.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     9022 2022-04-16 00:08:43.000000 pycrtsh-0.3.9/pycrtsh/api.py
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     2103 2022-04-19 13:01:34.000000 pycrtsh-0.3.9/pycrtsh/cli.py
+drwxr-xr-x   0 etienne   (1000) etienne   (1000)        0 2022-06-27 17:46:40.270372 pycrtsh-0.3.9/pycrtsh.egg-info/
+-rw-r--r--   0 etienne   (1000) etienne   (1000)     5581 2022-06-27 17:46:38.000000 pycrtsh-0.3.9/pycrtsh.egg-info/PKG-INFO
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      264 2022-06-27 17:46:39.000000 pycrtsh-0.3.9/pycrtsh.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        1 2022-06-27 17:46:38.000000 pycrtsh-0.3.9/pycrtsh.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       44 2022-06-27 17:46:39.000000 pycrtsh-0.3.9/pycrtsh.egg-info/entry_points.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       60 2022-06-27 17:46:39.000000 pycrtsh-0.3.9/pycrtsh.egg-info/requires.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)        8 2022-06-27 17:46:39.000000 pycrtsh-0.3.9/pycrtsh.egg-info/top_level.txt
+-rw-r--r--   0 etienne   (1000) etienne   (1000)       38 2022-06-27 17:46:40.274372 pycrtsh-0.3.9/setup.cfg
+-rw-r--r--   0 etienne   (1000) etienne   (1000)      828 2022-06-27 17:46:13.000000 pycrtsh-0.3.9/setup.py
```

### Comparing `pycrtsh-0.3.8/LICENSE` & `pycrtsh-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrtsh-0.3.8/PKG-INFO` & `pycrtsh-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrtsh
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python library to request crt.sh certificate information
 Home-page: https://github.com/Te-k/pycrtsh
 Author: Tek
 Author-email: tek@randhome.io
 License: MIT
 Keywords: security
 Platform: UNKNOWN
```

### Comparing `pycrtsh-0.3.8/README.md` & `pycrtsh-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pycrtsh-0.3.8/pycrtsh/api.py` & `pycrtsh-0.3.9/pycrtsh/api.py`

 * *Files identical despite different names*

### Comparing `pycrtsh-0.3.8/pycrtsh/cli.py` & `pycrtsh-0.3.9/pycrtsh/cli.py`

 * *Files identical despite different names*

### Comparing `pycrtsh-0.3.8/pycrtsh.egg-info/PKG-INFO` & `pycrtsh-0.3.9/pycrtsh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrtsh
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python library to request crt.sh certificate information
 Home-page: https://github.com/Te-k/pycrtsh
 Author: Tek
 Author-email: tek@randhome.io
 License: MIT
 Keywords: security
 Platform: UNKNOWN
```

### Comparing `pycrtsh-0.3.8/setup.py` & `pycrtsh-0.3.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pycrtsh',
-    version='0.3.8',
+    version='0.3.9',
     description='Python library to request crt.sh certificate information',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Te-k/pycrtsh',
     author='Tek',
     author_email='tek@randhome.io',
     keywords='security',
-    install_requires=['requests', 'lxml==4.6.5', 'beautifulsoup4==4.10.0', 'python-dateutil'],
+    install_requires=['requests', 'lxml==4.6.5', 'beautifulsoup4>=4.11.1', 'python-dateutil'],
     license='MIT',
     packages=['pycrtsh'],
     entry_points= {
         'console_scripts': [ 'certsh=pycrtsh.cli:main' ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

