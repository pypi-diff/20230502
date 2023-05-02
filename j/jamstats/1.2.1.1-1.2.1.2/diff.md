# Comparing `tmp/jamstats-nogui-1.2.1.1.tar.gz` & `tmp/jamstats-1.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jamstats-1.2.1.1.tar", last modified: Tue May  2 15:29:00 2023, max compression
+gzip compressed data, was "dist/jamstats-1.2.1.2.tar", last modified: Tue May  2 15:32:05 2023, max compression
```

## Comparing `jamstats-nogui-1.2.1.1.tar` & `jamstats-1.2.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/
--rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/README.md
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/bin/
--rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.2.1.1/bin/jamstats
--rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-05-02 00:48:27.000000 jamstats-1.2.1.1/bin/jamstats-nogui
--rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/setup.cfg
--rw-r--r--   0 damonmay   (501) staff       (20)      865 2023-05-02 02:30:12.000000 jamstats-1.2.1.1/setup.py
--rw-r--r--   0 damonmay   (501) staff       (20)      833 2023-05-02 15:25:08.000000 jamstats-1.2.1.1/setup_nogui.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/data/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/data/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-1.2.1.1/src/jamstats/data/game_data.py
--rw-r--r--   0 damonmay   (501) staff       (20)    36908 2023-04-30 05:44:55.000000 jamstats-1.2.1.1/src/jamstats/data/json_to_pandas.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/io/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/io/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/src/jamstats/io/scoreboard_json_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/src/jamstats/io/scoreboard_server_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/io/tsv_io.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/plots/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/plots/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/src/jamstats/plots/jamplots.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.2.1.1/src/jamstats/plots/plot_together.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.2.1.1/src/jamstats/plots/plot_util.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/src/jamstats/plots/skaterplots.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/resources/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/resources/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/util/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/util/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/util/resources.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats/web/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.1/src/jamstats/web/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-1.2.1.1/src/jamstats/web/statserver.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/
--rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)      818 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/SOURCES.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/dependency_links.txt
--rw-r--r--   0 damonmay   (501) staff       (20)      169 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/requires.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-05-02 15:29:00.000000 jamstats-1.2.1.1/src/jamstats.egg-info/top_level.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/
+-rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/README.md
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/bin/
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    11127 2023-04-01 22:28:27.000000 jamstats-1.2.1.2/bin/jamstats
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-05-02 00:48:27.000000 jamstats-1.2.1.2/bin/jamstats-nogui
+-rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/setup.cfg
+-rw-r--r--   0 damonmay   (501) staff       (20)      867 2023-05-02 15:31:35.000000 jamstats-1.2.1.2/setup.py
+-rw-r--r--   0 damonmay   (501) staff       (20)      833 2023-05-02 15:25:08.000000 jamstats-1.2.1.2/setup_nogui.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/data/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/data/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-1.2.1.2/src/jamstats/data/game_data.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    36908 2023-04-30 05:44:55.000000 jamstats-1.2.1.2/src/jamstats/data/json_to_pandas.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/io/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/io/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/io/scoreboard_json_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/io/scoreboard_server_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/io/tsv_io.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/plots/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/plots/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/plots/jamplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-1.2.1.2/src/jamstats/plots/plot_together.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-1.2.1.2/src/jamstats/plots/plot_util.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/plots/skaterplots.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/resources/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/util/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/util/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/util/resources.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats/web/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-1.2.1.2/src/jamstats/web/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-1.2.1.2/src/jamstats/web/statserver.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/
+-rw-r--r--   0 damonmay   (501) staff       (20)      424 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)      818 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/SOURCES.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/dependency_links.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)      184 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/requires.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-05-02 15:32:05.000000 jamstats-1.2.1.2/src/jamstats.egg-info/top_level.txt
```

### Comparing `jamstats-1.2.1.1/README.md` & `jamstats-1.2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/bin/jamstats` & `jamstats-1.2.1.2/bin/jamstats`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/bin/jamstats-nogui` & `jamstats-1.2.1.2/bin/jamstats-nogui`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/setup.py` & `jamstats-1.2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats',
-    version='1.2.1',
+    version='1.2.1.2',
     description='Data processing, stats and plots on roller derby scoreboard JSON files',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=find_packages('src', exclude=['test']),
     scripts=['bin/jamstats', 'bin/jamstats-nogui'],
     install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'gooey>=1.0.8.1', 'websocket-client>=1.2.1',
```

### Comparing `jamstats-1.2.1.1/setup_nogui.py` & `jamstats-1.2.1.2/setup_nogui.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/data/game_data.py` & `jamstats-1.2.1.2/src/jamstats/data/game_data.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/data/json_to_pandas.py` & `jamstats-1.2.1.2/src/jamstats/data/json_to_pandas.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/io/scoreboard_json_io.py` & `jamstats-1.2.1.2/src/jamstats/io/scoreboard_json_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/io/scoreboard_server_io.py` & `jamstats-1.2.1.2/src/jamstats/io/scoreboard_server_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/io/tsv_io.py` & `jamstats-1.2.1.2/src/jamstats/io/tsv_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/plots/jamplots.py` & `jamstats-1.2.1.2/src/jamstats/plots/jamplots.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/plots/plot_together.py` & `jamstats-1.2.1.2/src/jamstats/plots/plot_together.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/plots/plot_util.py` & `jamstats-1.2.1.2/src/jamstats/plots/plot_util.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/plots/skaterplots.py` & `jamstats-1.2.1.2/src/jamstats/plots/skaterplots.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/util/resources.py` & `jamstats-1.2.1.2/src/jamstats/util/resources.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats/web/statserver.py` & `jamstats-1.2.1.2/src/jamstats/web/statserver.py`

 * *Files identical despite different names*

### Comparing `jamstats-1.2.1.1/src/jamstats.egg-info/SOURCES.txt` & `jamstats-1.2.1.2/src/jamstats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

