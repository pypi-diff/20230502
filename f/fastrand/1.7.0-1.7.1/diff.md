# Comparing `tmp/fastrand-1.7.0.tar.gz` & `tmp/fastrand-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastrand-1.7.0.tar", last modified: Fri Feb  3 16:00:04 2023, max compression
+gzip compressed data, was "fastrand-1.7.1.tar", last modified: Tue May  2 18:31:43 2023, max compression
```

## Comparing `fastrand-1.7.0.tar` & `fastrand-1.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:00:04.964443 fastrand-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-03 15:59:52.000000 fastrand-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-03 16:00:04.964443 fastrand-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-03 15:59:52.000000 fastrand-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 16:00:04.964443 fastrand-1.7.0/fastrand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-03 16:00:04.000000 fastrand-1.7.0/fastrand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-03 16:00:04.000000 fastrand-1.7.0/fastrand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 16:00:04.000000 fastrand-1.7.0/fastrand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-03 16:00:04.000000 fastrand-1.7.0/fastrand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-02-03 15:59:52.000000 fastrand-1.7.0/fastrandmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 16:00:04.964443 fastrand-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-03 15:59:52.000000 fastrand-1.7.0/setup.py
+drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 18:31:43.529010 fastrand-1.7.1/
+-rw-r--r--   0 dlemire    (502) staff       (20)    11357 2023-02-03 15:08:51.000000 fastrand-1.7.1/LICENSE
+-rw-r--r--   0 dlemire    (502) staff       (20)     2671 2023-05-02 18:31:43.528872 fastrand-1.7.1/PKG-INFO
+-rw-r--r--   0 dlemire    (502) staff       (20)     2454 2023-05-02 18:22:32.000000 fastrand-1.7.1/README.md
+drwxr-xr-x   0 dlemire    (502) staff       (20)        0 2023-05-02 18:31:43.528708 fastrand-1.7.1/fastrand.egg-info/
+-rw-r--r--   0 dlemire    (502) staff       (20)     2671 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/PKG-INFO
+-rw-r--r--   0 dlemire    (502) staff       (20)      171 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/SOURCES.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)        1 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/dependency_links.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)        9 2023-05-02 18:31:43.000000 fastrand-1.7.1/fastrand.egg-info/top_level.txt
+-rw-r--r--   0 dlemire    (502) staff       (20)     4762 2023-02-03 15:08:51.000000 fastrand-1.7.1/fastrandmodule.c
+-rw-r--r--   0 dlemire    (502) staff       (20)       38 2023-05-02 18:31:43.529042 fastrand-1.7.1/setup.cfg
+-rw-r--r--   0 dlemire    (502) staff       (20)      463 2023-05-02 18:31:04.000000 fastrand-1.7.1/setup.py
```

### Comparing `fastrand-1.7.0/LICENSE` & `fastrand-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastrand-1.7.0/PKG-INFO` & `fastrand-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastrand
-Version: 1.7.0
+Version: 1.7.1
 Summary: Fast random number generation in Python
 Author: Daniel Lemire
 Author-email: daniel@lemire.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastrand
```

### Comparing `fastrand-1.7.0/README.md` & `fastrand-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fastrand-1.7.0/fastrand.egg-info/PKG-INFO` & `fastrand-1.7.1/fastrand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastrand
-Version: 1.7.0
+Version: 1.7.1
 Summary: Fast random number generation in Python
 Author: Daniel Lemire
 Author-email: daniel@lemire.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastrand
```

### Comparing `fastrand-1.7.0/fastrandmodule.c` & `fastrand-1.7.1/fastrandmodule.c`

 * *Files identical despite different names*

