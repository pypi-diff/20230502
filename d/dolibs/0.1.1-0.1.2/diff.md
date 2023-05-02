# Comparing `tmp/dolibs-0.1.1.tar.gz` & `tmp/dolibs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibs-0.1.1.tar", last modified: Tue May  2 15:08:00 2023, max compression
+gzip compressed data, was "dolibs-0.1.2.tar", last modified: Tue May  2 16:20:27 2023, max compression
```

## Comparing `dolibs-0.1.1.tar` & `dolibs-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 15:08:00.012314 dolibs-0.1.1/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 15:08:00.012182 dolibs-0.1.1/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      628 2023-05-02 14:40:08.000000 dolibs-0.1.1/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 15:08:00.011223 dolibs-0.1.1/dolibs/
--rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.1/dolibs/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4602 2023-04-27 15:31:17.000000 dolibs-0.1.1/dolibs/skintemp.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 15:08:00.011978 dolibs-0.1.1/dolibs.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 15:07:59.000000 dolibs-0.1.1/dolibs.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      220 2023-05-02 15:07:59.000000 dolibs-0.1.1/dolibs.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-02 15:07:59.000000 dolibs-0.1.1/dolibs.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       47 2023-05-02 15:07:59.000000 dolibs-0.1.1/dolibs.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)        7 2023-05-02 15:07:59.000000 dolibs-0.1.1/dolibs.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)      611 2023-05-02 15:07:39.000000 dolibs-0.1.1/pyproject.toml
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-02 15:08:00.012363 dolibs-0.1.1/setup.cfg
--rw-r--r--   0 leandro    (501) staff       (20)      569 2023-05-02 15:07:49.000000 dolibs-0.1.1/setup.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.421991 dolibs-0.1.2/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 16:20:27.421847 dolibs-0.1.2/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      628 2023-05-02 14:40:08.000000 dolibs-0.1.2/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.420807 dolibs-0.1.2/dolibs/
+-rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.2/dolibs/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4602 2023-05-02 15:47:01.000000 dolibs-0.1.2/dolibs/skintemp.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-05-02 16:20:27.421628 dolibs-0.1.2/dolibs.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      205 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       47 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        7 2023-05-02 16:20:27.000000 dolibs-0.1.2/dolibs.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-05-02 16:20:27.422044 dolibs-0.1.2/setup.cfg
+-rw-r--r--   0 leandro    (501) staff       (20)      569 2023-05-02 16:20:02.000000 dolibs-0.1.2/setup.py
```

### Comparing `dolibs-0.1.1/README.md` & `dolibs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.1/dolibs/skintemp.py` & `dolibs-0.1.2/dolibs/skintemp.py`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.1/setup.py` & `dolibs-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 setup(
     name='dolibs',
     packages=find_packages(include=['dolibs']),
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/n3tmaster/ERA5_procedures',
     description='Library for importing ERA5 Copernicus data into Drought Observatory platform',
     author='Leandro Rocchi - CNR',
     author_email='leandro.rocchi@cnr.it',
     license='MIT',
-    install_requires=['cdsapi','numpy','xarray','SQLAlchemy','psycopg2-binary'],
+    install_requires=['cdsapi','numpy','xarray','sqlalchemy','psycopg2-binary'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest==4.4.1'],
     test_suite='tests',
 )
```

