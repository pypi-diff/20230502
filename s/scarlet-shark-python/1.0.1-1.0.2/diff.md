# Comparing `tmp/scarlet-shark-python-1.0.1.tar.gz` & `tmp/scarlet-shark-python-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarlet-shark-python-1.0.1.tar", last modified: Fri Apr 28 12:03:09 2023, max compression
+gzip compressed data, was "scarlet-shark-python-1.0.2.tar", last modified: Tue May  2 10:03:42 2023, max compression
```

## Comparing `scarlet-shark-python-1.0.1.tar` & `scarlet-shark-python-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/scarlet_shark_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/scarlet_shark_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/scarlet_shark_python/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/scarlet_shark_python/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/scarlet_shark_python/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/scarlet_shark_python/clients/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/scarlet_shark_python/clients/v04_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 12:03:08.000000 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-28 12:03:09.000000 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:03:08.000000 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 12:03:08.000000 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 12:03:08.000000 scarlet-shark-python-1.0.1/scarlet_shark_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:03:09.077943 scarlet-shark-python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-28 12:02:55.000000 scarlet-shark-python-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/scarlet_shark_python/clients/v04_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 10:03:42.277817 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 10:03:42.000000 scarlet-shark-python-1.0.2/scarlet_shark_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 10:03:42.281817 scarlet-shark-python-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-02 10:03:29.000000 scarlet-shark-python-1.0.2/setup.py
```

### Comparing `scarlet-shark-python-1.0.1/LICENSE.txt` & `scarlet-shark-python-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.1/README.md` & `scarlet-shark-python-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.1/scarlet_shark_python/client.py` & `scarlet-shark-python-1.0.2/scarlet_shark_python/client.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.1/scarlet_shark_python/clients/abstract.py` & `scarlet-shark-python-1.0.2/scarlet_shark_python/clients/abstract.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.1/scarlet_shark_python/clients/v04_client.py` & `scarlet-shark-python-1.0.2/scarlet_shark_python/clients/v04_client.py`

 * *Files identical despite different names*

### Comparing `scarlet-shark-python-1.0.1/setup.py` & `scarlet-shark-python-1.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,27 @@
 from setuptools import setup, find_packages
 
 
 if sys.version_info.major == 3 and sys.version_info.minor < 3:
     print('Unfortunately, your python version is not supported!\n Please upgrade at least to python 3.3!')
     sys.exit(1)
 
+# read the contents of your README file
+from pathlib import Path
+pwd = Path(__file__).parent
+long_description = (pwd / "README.md").read_text()
+
 install_requires = [
     'requests==2.29.0'
 ]
 
 setup(name='scarlet-shark-python',
-      version='1.0.1',
+      version='1.0.2',
       description='Scarlet Shark REST API Python client',
-      long_description='file: README.md',
+      long_description=long_description,
       long_description_content_type='text/markdown',
       author='U+039b',
       author_email='esther@pts-project.org',
       url='https://github.com/PiRogueToolSuite/scarlet-shark-python',
       packages=find_packages(exclude=['*.tests', '*.tests.*', 'test*', 'tests']),
       install_requires=install_requires,
       classifiers=[
```

