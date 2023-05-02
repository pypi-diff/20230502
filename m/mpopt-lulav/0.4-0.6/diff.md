# Comparing `tmp/mpopt_lulav-0.4.tar.gz` & `tmp/mpopt_lulav-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpopt_lulav-0.4.tar", last modified: Tue May  2 11:27:34 2023, max compression
+gzip compressed data, was "mpopt_lulav-0.6.tar", last modified: Tue May  2 12:44:25 2023, max compression
```

## Comparing `mpopt_lulav-0.4.tar` & `mpopt_lulav-0.6.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:27:34.673573 mpopt_lulav-0.4/
--rw-r--r--   0 glebteplov   (501) staff       (20)      757 2023-05-02 11:27:34.673782 mpopt_lulav-0.4/PKG-INFO
-drwxr-xr-x   0 glebteplov   (501) staff       (20)        0 2023-05-02 11:27:34.673489 mpopt_lulav-0.4/mpopt_lulav/
--rw-r--r--   0 glebteplov   (501) staff       (20)      383 2023-05-02 11:26:51.659193 mpopt_lulav-0.4/mpopt_lulav/__init__.py
--rw-r--r--   0 glebteplov   (501) staff       (20)   130904 2023-04-25 08:47:09.109647 mpopt_lulav-0.4/mpopt_lulav/mpopt_lulav.py
--rw-r--r--   0 glebteplov   (501) staff       (20)       39 2023-05-02 09:29:09.632076 mpopt_lulav-0.4/setup.cfg
--rw-r--r--   0 glebteplov   (501) staff       (20)      938 2023-05-02 11:27:25.883268 mpopt_lulav-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:44:25.666926 mpopt_lulav-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-02 12:44:07.000000 mpopt_lulav-0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-02 12:44:25.666926 mpopt_lulav-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-02 12:44:07.000000 mpopt_lulav-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:44:25.666926 mpopt_lulav-0.6/mpopt_lulav/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-02 12:44:07.000000 mpopt_lulav-0.6/mpopt_lulav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130904 2023-05-02 12:44:07.000000 mpopt_lulav-0.6/mpopt_lulav/mpopt_lulav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:44:25.666926 mpopt_lulav-0.6/mpopt_lulav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-02 12:44:25.000000 mpopt_lulav-0.6/mpopt_lulav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-02 12:44:25.000000 mpopt_lulav-0.6/mpopt_lulav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:44:25.000000 mpopt_lulav-0.6/mpopt_lulav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 12:44:25.000000 mpopt_lulav-0.6/mpopt_lulav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 12:44:25.000000 mpopt_lulav-0.6/mpopt_lulav.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 12:44:25.666926 mpopt_lulav-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 12:44:07.000000 mpopt_lulav-0.6/setup.py
```

### Comparing `mpopt_lulav-0.4/mpopt_lulav/mpopt_lulav.py` & `mpopt_lulav-0.6/mpopt_lulav/mpopt_lulav.py`

 * *Files identical despite different names*

