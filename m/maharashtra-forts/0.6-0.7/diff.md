# Comparing `tmp/maharashtra-forts-0.6.tar.gz` & `tmp/maharashtra-forts-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharashtra-forts-0.6.tar", last modified: Tue May  2 12:25:37 2023, max compression
+gzip compressed data, was "maharashtra-forts-0.7.tar", last modified: Tue May  2 12:37:32 2023, max compression
```

## Comparing `maharashtra-forts-0.6.tar` & `maharashtra-forts-0.7.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:25:37.963846 maharashtra-forts-0.6/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      189 2023-05-02 12:25:37.963616 maharashtra-forts-0.6/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1552 2023-05-02 07:47:39.000000 maharashtra-forts-0.6/README.md
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:25:37.960584 maharashtra-forts-0.6/maharashtra_forts/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 maharashtra-forts-0.6/maharashtra_forts/__init__.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:25:37.963410 maharashtra-forts-0.6/maharashtra_forts/forts/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 06:48:51.000000 maharashtra-forts-0.6/maharashtra_forts/forts/__init__.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/harishchandragad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/lohagad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/pratapgad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/purandar_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/raigad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/rajgad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/shivneri_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/sinhagad_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/tikona_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.6/maharashtra_forts/forts/torna_fort.py
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 maharashtra-forts-0.6/maharashtra_forts/get_forts.py
-drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:25:37.961928 maharashtra-forts-0.6/maharashtra_forts.egg-info/
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      189 2023-05-02 12:25:37.000000 maharashtra-forts-0.6/maharashtra_forts.egg-info/PKG-INFO
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      732 2023-05-02 12:25:37.000000 maharashtra-forts-0.6/maharashtra_forts.egg-info/SOURCES.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:25:37.000000 maharashtra-forts-0.6/maharashtra_forts.egg-info/dependency_links.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       20 2023-05-02 12:25:37.000000 maharashtra-forts-0.6/maharashtra_forts.egg-info/entry_points.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:25:37.000000 maharashtra-forts-0.6/maharashtra_forts.egg-info/top_level.txt
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-05-02 12:25:37.963900 maharashtra-forts-0.6/setup.cfg
--rw-r--r--   0 rahulbhoyar   (501) staff       (20)      320 2023-05-02 12:24:14.000000 maharashtra-forts-0.6/setup.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.143425 maharashtra-forts-0.7/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:37:32.143264 maharashtra-forts-0.7/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1552 2023-05-02 07:47:39.000000 maharashtra-forts-0.7/README.md
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.140838 maharashtra-forts-0.7/maharashtra_forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-04-18 18:22:46.000000 maharashtra-forts-0.7/maharashtra_forts/__init__.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.143042 maharashtra-forts-0.7/maharashtra_forts/forts/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 06:48:51.000000 maharashtra-forts-0.7/maharashtra_forts/forts/__init__.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/harishchandragad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/lohagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/pratapgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/purandar_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/raigad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/rajgad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/shivneri_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/sinhagad_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/tikona_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 07:39:43.000000 maharashtra-forts-0.7/maharashtra_forts/forts/torna_fort.py
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      487 2023-05-02 07:41:41.000000 maharashtra-forts-0.7/maharashtra_forts/maharashtra_forts.py
+drwxr-xr-x   0 rahulbhoyar   (501) staff       (20)        0 2023-05-02 12:37:32.141665 maharashtra-forts-0.7/maharashtra_forts.egg-info/
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     2367 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/PKG-INFO
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)      696 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)        1 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       18 2023-05-02 12:37:32.000000 maharashtra-forts-0.7/maharashtra_forts.egg-info/top_level.txt
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)       38 2023-05-02 12:37:32.143485 maharashtra-forts-0.7/setup.cfg
+-rw-r--r--   0 rahulbhoyar   (501) staff       (20)     1072 2023-05-02 12:35:48.000000 maharashtra-forts-0.7/setup.py
```

### Comparing `maharashtra-forts-0.6/README.md` & `maharashtra-forts-0.7/README.md`

 * *Files identical despite different names*

### Comparing `maharashtra-forts-0.6/maharashtra_forts.egg-info/SOURCES.txt` & `maharashtra-forts-0.7/maharashtra_forts.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 README.md
 setup.py
 maharashtra_forts/__init__.py
-maharashtra_forts/get_forts.py
+maharashtra_forts/maharashtra_forts.py
 maharashtra_forts.egg-info/PKG-INFO
 maharashtra_forts.egg-info/SOURCES.txt
 maharashtra_forts.egg-info/dependency_links.txt
-maharashtra_forts.egg-info/entry_points.txt
 maharashtra_forts.egg-info/top_level.txt
 maharashtra_forts/forts/__init__.py
 maharashtra_forts/forts/harishchandragad_fort.py
 maharashtra_forts/forts/lohagad_fort.py
 maharashtra_forts/forts/pratapgad_fort.py
 maharashtra_forts/forts/purandar_fort.py
 maharashtra_forts/forts/raigad_fort.py
```

