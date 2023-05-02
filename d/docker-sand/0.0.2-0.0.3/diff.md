# Comparing `tmp/docker-sand-0.0.2.tar.gz` & `tmp/docker-sand-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-sand-0.0.2.tar", last modified: Tue May  2 07:03:45 2023, max compression
+gzip compressed data, was "docker-sand-0.0.3.tar", last modified: Tue May  2 16:02:17 2023, max compression
```

## Comparing `docker-sand-0.0.2.tar` & `docker-sand-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 guyk       (501) staff       (20)        0 2023-05-02 07:03:45.868101 docker-sand-0.0.2/
--rw-r--r--   0 guyk       (501) staff       (20)     3033 2023-05-02 07:03:45.867953 docker-sand-0.0.2/PKG-INFO
--rw-r--r--   0 guyk       (501) staff       (20)     2701 2023-05-01 19:12:23.000000 docker-sand-0.0.2/README.md
-drwxr-xr-x   0 guyk       (501) staff       (20)        0 2023-05-02 07:03:45.864671 docker-sand-0.0.2/docker_sand.egg-info/
--rw-r--r--   0 guyk       (501) staff       (20)     3033 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/PKG-INFO
--rw-r--r--   0 guyk       (501) staff       (20)      513 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/SOURCES.txt
--rw-r--r--   0 guyk       (501) staff       (20)        1 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/dependency_links.txt
--rw-r--r--   0 guyk       (501) staff       (20)       49 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/entry_points.txt
--rw-r--r--   0 guyk       (501) staff       (20)        9 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/requires.txt
--rw-r--r--   0 guyk       (501) staff       (20)        5 2023-05-02 07:03:45.000000 docker-sand-0.0.2/docker_sand.egg-info/top_level.txt
-drwxr-xr-x   0 guyk       (501) staff       (20)        0 2023-05-02 07:03:45.865290 docker-sand-0.0.2/sand/
--rw-r--r--   0 guyk       (501) staff       (20)       19 2023-04-29 20:11:45.000000 docker-sand-0.0.2/sand/__init__.py
-drwxr-xr-x   0 guyk       (501) staff       (20)        0 2023-05-02 07:03:45.866714 docker-sand-0.0.2/sand/internal/
--rw-r--r--   0 guyk       (501) staff       (20)        0 2023-04-10 08:45:56.000000 docker-sand-0.0.2/sand/internal/__init__.py
--rw-r--r--   0 guyk       (501) staff       (20)      734 2023-04-08 13:53:03.000000 docker-sand-0.0.2/sand/internal/docker_image.py
--rw-r--r--   0 guyk       (501) staff       (20)     4807 2023-04-30 19:48:39.000000 docker-sand-0.0.2/sand/internal/main.py
-drwxr-xr-x   0 guyk       (501) staff       (20)        0 2023-05-02 07:03:45.867617 docker-sand-0.0.2/sand/internal/sandfile_executor/
--rw-r--r--   0 guyk       (501) staff       (20)        0 2023-04-08 09:38:45.000000 docker-sand-0.0.2/sand/internal/sandfile_executor/__init__.py
--rw-r--r--   0 guyk       (501) staff       (20)     1419 2023-04-10 08:51:42.000000 docker-sand-0.0.2/sand/internal/sandfile_executor/commands.py
--rw-r--r--   0 guyk       (501) staff       (20)     2213 2023-04-30 19:47:50.000000 docker-sand-0.0.2/sand/internal/sandfile_executor/sandfile_executor.py
--rw-r--r--   0 guyk       (501) staff       (20)      773 2023-04-30 19:37:30.000000 docker-sand-0.0.2/sand/internal/sandfile_watcher.py
--rw-r--r--   0 guyk       (501) staff       (20)     2260 2023-04-30 19:17:22.000000 docker-sand-0.0.2/sand/sand.py
--rw-r--r--   0 guyk       (501) staff       (20)       38 2023-05-02 07:03:45.868152 docker-sand-0.0.2/setup.cfg
--rw-r--r--   0 guyk       (501) staff       (20)      835 2023-05-02 07:02:18.000000 docker-sand-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 16:02:17.551635 docker-sand-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-02 16:02:14.000000 docker-sand-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/docker_sand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 16:02:17.000000 docker-sand-0.0.3/docker_sand.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:17.551635 docker-sand-0.0.3/sand/internal/sandfile_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_executor/sandfile_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/internal/sandfile_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-02 16:02:14.000000 docker-sand-0.0.3/sand/sand.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 16:02:17.551635 docker-sand-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-02 16:02:14.000000 docker-sand-0.0.3/setup.py
```

### Comparing `docker-sand-0.0.2/PKG-INFO` & `docker-sand-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: docker-sand
-Version: 0.0.2
-Summary: Sand is a Dockerfile generator based on python that allows you to write your Dockerfile in a more convenient way.
-Home-page: https://github.com/gkpln3/Sand
-Author: Guy Kaplan
-License: MIT
-Keywords: sand docker dockerfile build
-Description-Content-Type: text/markdown
-
 # Sand 🏝
 Sand is a Dockerfile generator.
 
 It allows you to write cleaner, shorter and more configurable Dockerfiles.
 
 ## Developers ❤️ Sand
 Sand is built by developers, for developers. It's built to be as simple as possible, while still being super useful.
```

### Comparing `docker-sand-0.0.2/docker_sand.egg-info/SOURCES.txt` & `docker-sand-0.0.3/docker_sand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/internal/docker_image.py` & `docker-sand-0.0.3/sand/internal/docker_image.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/internal/main.py` & `docker-sand-0.0.3/sand/internal/main.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/internal/sandfile_executor/commands.py` & `docker-sand-0.0.3/sand/internal/sandfile_executor/commands.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/internal/sandfile_executor/sandfile_executor.py` & `docker-sand-0.0.3/sand/internal/sandfile_executor/sandfile_executor.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/internal/sandfile_watcher.py` & `docker-sand-0.0.3/sand/internal/sandfile_watcher.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/sand/sand.py` & `docker-sand-0.0.3/sand/sand.py`

 * *Files identical despite different names*

### Comparing `docker-sand-0.0.2/setup.py` & `docker-sand-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='docker-sand',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'sand = sand.internal.main:main'
         ]
     },
     install_requires=[
```

