# Comparing `tmp/klym-telemetry-0.1.1.tar.gz` & `tmp/klym-telemetry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klym-telemetry-0.1.1.tar", last modified: Mon May  1 22:06:15 2023, max compression
+gzip compressed data, was "klym-telemetry-0.1.2.tar", last modified: Tue May  2 00:53:30 2023, max compression
```

## Comparing `klym-telemetry-0.1.1.tar` & `klym-telemetry-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:06:15.404765 klym-telemetry-0.1.1/
--rw-rw-rw-   0        0        0     4076 2023-05-01 22:06:15.403759 klym-telemetry-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 22:06:15.385964 klym-telemetry-0.1.1/klym_telemetry/
--rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.1/klym_telemetry/__init__.py
--rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.1/klym_telemetry/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:06:15.402801 klym-telemetry-0.1.1/klym_telemetry/instrumenters/
--rw-rw-rw-   0        0        0      647 2023-05-01 21:12:52.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/base.py
--rw-rw-rw-   0        0        0      625 2023-04-27 14:15:23.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/celery.py
--rw-rw-rw-   0        0        0      625 2023-04-25 20:14:35.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/django.py
--rw-rw-rw-   0        0        0      992 2023-04-25 20:10:43.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/fastapi.py
--rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.1/klym_telemetry/instrumenters/postgres.py
--rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.1/klym_telemetry/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:06:15.393760 klym-telemetry-0.1.1/klym_telemetry.egg-info/
--rw-rw-rw-   0        0        0     4076 2023-05-01 22:06:15.000000 klym-telemetry-0.1.1/klym_telemetry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2023-05-01 22:06:15.000000 klym-telemetry-0.1.1/klym_telemetry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:06:15.000000 klym-telemetry-0.1.1/klym_telemetry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      406 2023-05-01 22:06:15.000000 klym-telemetry-0.1.1/klym_telemetry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-01 22:06:15.000000 klym-telemetry-0.1.1/klym_telemetry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:06:15.404765 klym-telemetry-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1684 2023-05-01 22:06:03.000000 klym-telemetry-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:53:30.188262 klym-telemetry-0.1.2/
+-rw-rw-rw-   0        0        0     4076 2023-05-02 00:53:30.187260 klym-telemetry-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3148 2023-05-01 21:12:52.000000 klym-telemetry-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-02 00:53:30.157261 klym-telemetry-0.1.2/klym_telemetry/
+-rw-rw-rw-   0        0        0        0 2023-04-22 00:00:44.000000 klym-telemetry-0.1.2/klym_telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2612 2023-04-23 22:09:56.000000 klym-telemetry-0.1.2/klym_telemetry/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:53:30.183267 klym-telemetry-0.1.2/klym_telemetry/instrumenters/
+-rw-rw-rw-   0        0        0      647 2023-05-01 21:12:52.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-25 19:42:07.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/base.py
+-rw-rw-rw-   0        0        0      625 2023-04-27 14:15:23.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/celery.py
+-rw-rw-rw-   0        0        0      625 2023-04-25 20:14:35.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/django.py
+-rw-rw-rw-   0        0        0      992 2023-04-25 20:10:43.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/fastapi.py
+-rw-rw-rw-   0        0        0      515 2023-05-01 21:09:25.000000 klym-telemetry-0.1.2/klym_telemetry/instrumenters/postgres.py
+-rw-rw-rw-   0        0        0     5693 2023-04-23 22:09:56.000000 klym-telemetry-0.1.2/klym_telemetry/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 00:53:30.171265 klym-telemetry-0.1.2/klym_telemetry.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-05-02 00:53:30.000000 klym-telemetry-0.1.2/klym_telemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-05-02 00:53:30.000000 klym-telemetry-0.1.2/klym_telemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 00:53:30.000000 klym-telemetry-0.1.2/klym_telemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      406 2023-05-02 00:53:30.000000 klym-telemetry-0.1.2/klym_telemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-02 00:53:30.000000 klym-telemetry-0.1.2/klym_telemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-02 00:53:30.188262 klym-telemetry-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1684 2023-05-02 00:41:07.000000 klym-telemetry-0.1.2/setup.py
```

### Comparing `klym-telemetry-0.1.1/PKG-INFO` & `klym-telemetry-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.1/README.md` & `klym-telemetry-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/helpers.py` & `klym-telemetry-0.1.2/klym_telemetry/helpers.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/__init__.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/__init__.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/base.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/base.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/celery.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/celery.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/django.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/django.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/fastapi.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/fastapi.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/instrumenters/postgres.py` & `klym-telemetry-0.1.2/klym_telemetry/instrumenters/postgres.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry/utils.py` & `klym-telemetry-0.1.2/klym_telemetry/utils.py`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/klym_telemetry.egg-info/PKG-INFO` & `klym-telemetry-0.1.2/klym_telemetry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klym-telemetry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Scaffold library
 Home-page: https://dummy.readthedocs.io/
 Author: Klym Telemetry
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klym-telemetry-0.1.1/klym_telemetry.egg-info/SOURCES.txt` & `klym-telemetry-0.1.2/klym_telemetry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klym-telemetry-0.1.1/setup.py` & `klym-telemetry-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="klym-telemetry",
-    version="0.1.1",
+    version="0.1.2",
     description="Scaffold library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dummy.readthedocs.io/",
     author="Klym Telemetry",
     author_email="example@email.com",
     license="MIT",
```

