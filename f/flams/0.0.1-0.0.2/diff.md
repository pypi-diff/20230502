# Comparing `tmp/flams-0.0.1.tar.gz` & `tmp/flams-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-0.0.1.tar", last modified: Tue May  2 14:10:51 2023, max compression
+gzip compressed data, was "flams-0.0.2.tar", last modified: Tue May  2 14:42:56 2023, max compression
```

## Comparing `flams-0.0.1.tar` & `flams-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:10:51.757273 flams-0.0.1/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       73 2023-05-02 14:10:51.753273 flams-0.0.1/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-02 06:30:11.000000 flams-0.0.1/README.md
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:10:51.753273 flams-0.0.1/flams/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.1/flams/__init__.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:10:51.753273 flams-0.0.1/flams/databases/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.1/flams/databases/__init__.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-04-07 09:12:53.000000 flams-0.0.1/flams/databases/cplmv4.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-02 11:49:48.000000 flams-0.0.1/flams/databases/setup.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-02 06:30:11.000000 flams-0.0.1/flams/display.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-02 12:00:55.000000 flams-0.0.1/flams/flams.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12066 2023-05-02 14:01:51.000000 flams-0.0.1/flams/input.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-02 11:49:04.000000 flams-0.0.1/flams/run_blast.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      768 2023-04-07 09:12:53.000000 flams-0.0.1/flams/utils.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:10:51.753273 flams-0.0.1/flams.egg-info/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       73 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      372 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/SOURCES.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/dependency_links.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/entry_points.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       27 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/requires.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-02 14:10:51.000000 flams-0.0.1/flams.egg-info/top_level.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-02 14:10:51.757273 flams-0.0.1/setup.cfg
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      380 2023-05-02 13:20:45.000000 flams-0.0.1/setup.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:42:56.977412 flams-0.0.2/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-02 14:42:26.000000 flams-0.0.2/LICENCE
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      153 2023-05-02 14:42:56.977412 flams-0.0.2/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-02 06:30:11.000000 flams-0.0.2/README.md
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:42:56.977412 flams-0.0.2/flams/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.2/flams/__init__.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:42:56.977412 flams-0.0.2/flams/databases/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-04-07 09:12:53.000000 flams-0.0.2/flams/databases/__init__.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-04-07 09:12:53.000000 flams-0.0.2/flams/databases/cplmv4.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-02 11:49:48.000000 flams-0.0.2/flams/databases/setup.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-02 06:30:11.000000 flams-0.0.2/flams/display.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-02 12:00:55.000000 flams-0.0.2/flams/flams.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12083 2023-05-02 14:35:57.000000 flams-0.0.2/flams/input.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-02 11:49:04.000000 flams-0.0.2/flams/run_blast.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      768 2023-04-07 09:12:53.000000 flams-0.0.2/flams/utils.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-02 14:42:56.977412 flams-0.0.2/flams.egg-info/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      153 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      380 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/entry_points.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       27 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/requires.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-02 14:42:56.000000 flams-0.0.2/flams.egg-info/top_level.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-02 14:42:56.977412 flams-0.0.2/setup.cfg
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      471 2023-05-02 14:39:40.000000 flams-0.0.2/setup.py
```

### Comparing `flams-0.0.1/README.md` & `flams-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/databases/cplmv4.py` & `flams-0.0.2/flams/databases/cplmv4.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/databases/setup.py` & `flams-0.0.2/flams/databases/setup.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/display.py` & `flams-0.0.2/flams/display.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/flams.py` & `flams-0.0.2/flams/flams.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/input.py` & `flams-0.0.2/flams/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     if (args.id is not None) & (not args.data_dir.is_dir()):
         if args.data_dir.parent.is_dir():
             os.mkdir(args.data_dir)
             logging.info(f"Data directory created: {args.data_dir}")
         else:
             logging.error(f"Provided path is not an existing " +
-                        "path. Please make sure the provided path " +
+                        "path: {args.data_dir}. Please make sure the provided path " +
                         "is correct. Exiting FLAMS...")
             sys.exit()
 
 
 def is_valid_fasta_file(path: Path):
     """
     This function checks whether the provided input FASTA file is a valid FASTA file.
```

### Comparing `flams-0.0.1/flams/run_blast.py` & `flams-0.0.2/flams/run_blast.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.1/flams/utils.py` & `flams-0.0.2/flams/utils.py`

 * *Files identical despite different names*

