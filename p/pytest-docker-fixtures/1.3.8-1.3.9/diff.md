# Comparing `tmp/pytest-docker-fixtures-1.3.8.tar.gz` & `tmp/pytest-docker-fixtures-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-docker-fixtures-1.3.8.tar", last modified: Fri Jul  3 02:05:37 2020, max compression
+gzip compressed data, was "dist/pytest-docker-fixtures-1.3.9.tar", last modified: Fri Jul 10 12:16:01 2020, max compression
```

## Comparing `pytest-docker-fixtures-1.3.8.tar` & `pytest-docker-fixtures-1.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/
--rw-r--r--   0 nathan     (501) staff       (20)     5396 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/PKG-INFO
-drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/
--rw-r--r--   0 nathan     (501) staff       (20)     2840 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/__init__.py
--rw-r--r--   0 nathan     (501) staff       (20)     3028 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/images.py
-drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/
--rw-r--r--   0 nathan     (501) staff       (20)     3954 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/_base.py
--rw-r--r--   0 nathan     (501) staff       (20)      817 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/pg.py
--rw-r--r--   0 nathan     (501) staff       (20)      955 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/cockroach.py
--rw-r--r--   0 nathan     (501) staff       (20)        0 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/__init__.py
--rw-r--r--   0 nathan     (501) staff       (20)     1062 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/etcd.py
--rw-r--r--   0 nathan     (501) staff       (20)      216 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/redis.py
--rw-r--r--   0 nathan     (501) staff       (20)      496 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/rabbitmq.py
--rw-r--r--   0 nathan     (501) staff       (20)      420 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/kafka.py
--rw-r--r--   0 nathan     (501) staff       (20)     1067 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/es.py
--rw-r--r--   0 nathan     (501) staff       (20)      400 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/minio.py
--rw-r--r--   0 nathan     (501) staff       (20)      755 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/mysql.py
--rw-r--r--   0 nathan     (501) staff       (20)       14 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/MANIFEST.in
-drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/
--rw-r--r--   0 nathan     (501) staff       (20)     5396 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/PKG-INFO
--rw-r--r--   0 nathan     (501) staff       (20)        1 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/zip-safe
--rw-r--r--   0 nathan     (501) staff       (20)      869 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/SOURCES.txt
--rw-r--r--   0 nathan     (501) staff       (20)      132 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/requires.txt
--rw-r--r--   0 nathan     (501) staff       (20)       23 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/top_level.txt
--rw-r--r--   0 nathan     (501) staff       (20)        1 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/dependency_links.txt
--rw-r--r--   0 nathan     (501) staff       (20)     1264 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/setup.py
--rw-r--r--   0 nathan     (501) staff       (20)      287 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/setup.cfg
--rw-r--r--   0 nathan     (501) staff       (20)      959 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/README.rst
--rw-r--r--   0 nathan     (501) staff       (20)     2121 2020-07-03 02:05:37.000000 pytest-docker-fixtures-1.3.8/CHANGELOG.rst
+drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/
+-rw-r--r--   0 nathan     (501) staff       (20)     5551 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/PKG-INFO
+drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/
+-rw-r--r--   0 nathan     (501) staff       (20)     2840 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/__init__.py
+-rw-r--r--   0 nathan     (501) staff       (20)     3100 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/images.py
+drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/
+-rw-r--r--   0 nathan     (501) staff       (20)     3954 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/_base.py
+-rw-r--r--   0 nathan     (501) staff       (20)      817 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/pg.py
+-rw-r--r--   0 nathan     (501) staff       (20)      955 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/cockroach.py
+-rw-r--r--   0 nathan     (501) staff       (20)        0 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/__init__.py
+-rw-r--r--   0 nathan     (501) staff       (20)     1062 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/etcd.py
+-rw-r--r--   0 nathan     (501) staff       (20)      216 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/redis.py
+-rw-r--r--   0 nathan     (501) staff       (20)      496 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/rabbitmq.py
+-rw-r--r--   0 nathan     (501) staff       (20)      420 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/kafka.py
+-rw-r--r--   0 nathan     (501) staff       (20)     1067 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/es.py
+-rw-r--r--   0 nathan     (501) staff       (20)      400 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/minio.py
+-rw-r--r--   0 nathan     (501) staff       (20)      755 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/mysql.py
+-rw-r--r--   0 nathan     (501) staff       (20)       14 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/MANIFEST.in
+drwxr-xr-x   0 nathan     (501) staff       (20)        0 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/
+-rw-r--r--   0 nathan     (501) staff       (20)     5551 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/PKG-INFO
+-rw-r--r--   0 nathan     (501) staff       (20)        1 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/zip-safe
+-rw-r--r--   0 nathan     (501) staff       (20)      869 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan     (501) staff       (20)      132 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/requires.txt
+-rw-r--r--   0 nathan     (501) staff       (20)       23 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/top_level.txt
+-rw-r--r--   0 nathan     (501) staff       (20)        1 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan     (501) staff       (20)     1264 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/setup.py
+-rw-r--r--   0 nathan     (501) staff       (20)      287 2020-07-10 12:16:01.000000 pytest-docker-fixtures-1.3.9/setup.cfg
+-rw-r--r--   0 nathan     (501) staff       (20)      959 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/README.rst
+-rw-r--r--   0 nathan     (501) staff       (20)     2220 2020-07-10 12:16:00.000000 pytest-docker-fixtures-1.3.9/CHANGELOG.rst
```

### Comparing `pytest-docker-fixtures-1.3.8/PKG-INFO` & `pytest-docker-fixtures-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-docker-fixtures
-Version: 1.3.8
+Version: 1.3.9
 Summary: pytest docker fixtures
 Home-page: https://github.com/guillotinaweb/pytest-docker-fixtures
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: BSD
 Description: Introduction
         ============
@@ -56,14 +56,21 @@
             from pytest_docker_fixtures import images
             images.configure(
                 'elasticsearch',
                 'docker.elastic.co/elasticsearch/elasticsearch-platinum', '6.2.4',
                 env={},
                 options={})
         
+        1.3.9 (2020-07-10)
+        ------------------
+        
+        - Fix passing options to image configuration
+          [gitcarbs]
+        
+        
         1.3.8 (2020-07-02)
         ------------------
         
         - Stop hardcoding db, user, and password in Postgresql.check()
           [marshalium]
         
         
@@ -218,11 +225,11 @@
 Keywords: pytest,fixtures,docker
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: pg
 Provides-Extra: mysql
 Provides-Extra: kafka
 Provides-Extra: rabbitmq
+Provides-Extra: pg
```

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/__init__.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/images.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
               env=None, options=None, max_wait_s=None):
     if full is not None:
         image, _, version = full.partition(':')
     if image is not None:
         settings[name]['image'] = image
     if version is not None:
         settings[name]['version'] = version
+    if options is not None:
+        settings[name]['options'] = options
     if env is not None:
         if 'env' not in settings[name]:
             settings[name]['env'] = {}
         settings[name]['env'].update(env)
     if max_wait_s:
         settings[name]['max_wait_s'] = max_wait_s
```

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/_base.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/_base.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/pg.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/pg.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/cockroach.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/cockroach.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/etcd.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/etcd.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/es.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/es.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures/containers/mysql.py` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures/containers/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/PKG-INFO` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-docker-fixtures
-Version: 1.3.8
+Version: 1.3.9
 Summary: pytest docker fixtures
 Home-page: https://github.com/guillotinaweb/pytest-docker-fixtures
 Author: Nathan Van Gheem
 Author-email: vangheem@gmail.com
 License: BSD
 Description: Introduction
         ============
@@ -56,14 +56,21 @@
             from pytest_docker_fixtures import images
             images.configure(
                 'elasticsearch',
                 'docker.elastic.co/elasticsearch/elasticsearch-platinum', '6.2.4',
                 env={},
                 options={})
         
+        1.3.9 (2020-07-10)
+        ------------------
+        
+        - Fix passing options to image configuration
+          [gitcarbs]
+        
+        
         1.3.8 (2020-07-02)
         ------------------
         
         - Stop hardcoding db, user, and password in Postgresql.check()
           [marshalium]
         
         
@@ -218,11 +225,11 @@
 Keywords: pytest,fixtures,docker
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: pg
 Provides-Extra: mysql
 Provides-Extra: kafka
 Provides-Extra: rabbitmq
+Provides-Extra: pg
```

### Comparing `pytest-docker-fixtures-1.3.8/pytest_docker_fixtures.egg-info/SOURCES.txt` & `pytest-docker-fixtures-1.3.9/pytest_docker_fixtures.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/setup.py` & `pytest-docker-fixtures-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='pytest-docker-fixtures',
-    version='1.3.8',
+    version='1.3.9',
     description='pytest docker fixtures',
     long_description=(open('README.rst').read() + '\n' +
                       open('CHANGELOG.rst').read()),
     keywords=['pytest', 'fixtures', 'docker'],
     author='Nathan Van Gheem',
     author_email='vangheem@gmail.com',
     classifiers=[
```

### Comparing `pytest-docker-fixtures-1.3.8/README.rst` & `pytest-docker-fixtures-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-docker-fixtures-1.3.8/CHANGELOG.rst` & `pytest-docker-fixtures-1.3.9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.3.9 (2020-07-10)
+------------------
+
+- Fix passing options to image configuration
+  [gitcarbs]
+
+
 1.3.8 (2020-07-02)
 ------------------
 
 - Stop hardcoding db, user, and password in Postgresql.check()
   [marshalium]
```

