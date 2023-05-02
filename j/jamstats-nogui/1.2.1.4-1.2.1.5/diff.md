# Comparing `tmp/jamstats-nogui-1.2.1.4.tar.gz` & `tmp/jamstats-nogui-1.2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jamstats-nogui-1.2.1.4.tar", last modified: Tue May  2 19:58:32 2023, max compression
+gzip compressed data, was "dist/jamstats-nogui-1.2.1.5.tar", last modified: Tue May  2 20:08:31 2023, max compression
```

## Comparing `jamstats-nogui-1.2.1.4.tar` & `jamstats-nogui-1.2.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/
--rw-r--r--   0 damonmay   (501) staff       (20)      447 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/README.md
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/bin/
--rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-05-02 00:48:27.000000 jamstats-nogui-1.2.1.4/bin/jamstats-nogui
--rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/setup.cfg
--rw-r--r--   0 damonmay   (501) staff       (20)      865 2023-05-02 15:33:19.000000 jamstats-nogui-1.2.1.4/setup.py
--rw-r--r--   0 damonmay   (501) staff       (20)      830 2023-05-02 19:58:22.000000 jamstats-nogui-1.2.1.4/setup_nogui.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/data/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/data/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-nogui-1.2.1.4/src/jamstats/data/game_data.py
--rw-r--r--   0 damonmay   (501) staff       (20)    36908 2023-04-30 05:44:55.000000 jamstats-nogui-1.2.1.4/src/jamstats/data/json_to_pandas.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/io/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/io/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/src/jamstats/io/scoreboard_json_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/src/jamstats/io/scoreboard_server_io.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/io/tsv_io.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/jamplots.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/plot_together.py
--rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/plot_util.py
--rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/src/jamstats/plots/skaterplots.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/resources/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/resources/__init__.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/util/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/util/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/util/resources.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats/web/
--rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.4/src/jamstats/web/__init__.py
--rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.4/src/jamstats/web/statserver.py
-drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/
--rw-r--r--   0 damonmay   (501) staff       (20)      447 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/PKG-INFO
--rw-r--r--   0 damonmay   (501) staff       (20)      835 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/SOURCES.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/dependency_links.txt
--rw-r--r--   0 damonmay   (501) staff       (20)      169 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/requires.txt
--rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-05-02 19:58:32.000000 jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/top_level.txt
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/
+-rw-r--r--   0 damonmay   (501) staff       (20)      447 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)     8788 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/README.md
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/bin/
+-rwxr-xr-x   0 damonmay   (501) staff       (20)    10659 2023-05-02 00:48:27.000000 jamstats-nogui-1.2.1.5/bin/jamstats-nogui
+-rw-r--r--   0 damonmay   (501) staff       (20)       38 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/setup.cfg
+-rw-r--r--   0 damonmay   (501) staff       (20)      830 2023-05-02 20:08:27.000000 jamstats-nogui-1.2.1.5/setup.py
+-rw-r--r--   0 damonmay   (501) staff       (20)      830 2023-05-02 19:58:22.000000 jamstats-nogui-1.2.1.5/setup_nogui.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/data/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/data/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9916 2023-04-02 05:53:22.000000 jamstats-nogui-1.2.1.5/src/jamstats/data/game_data.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    36908 2023-04-30 05:44:55.000000 jamstats-nogui-1.2.1.5/src/jamstats/data/json_to_pandas.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/io/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/io/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2564 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/src/jamstats/io/scoreboard_json_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    10201 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/src/jamstats/io/scoreboard_server_io.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2216 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/io/tsv_io.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    43584 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/jamplots.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4566 2023-03-18 01:38:05.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/plot_together.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     4012 2023-02-24 16:00:04.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/plot_util.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     9703 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/src/jamstats/plots/skaterplots.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/resources/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/resources/__init__.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/util/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/util/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)     2597 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/util/resources.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats/web/
+-rw-r--r--   0 damonmay   (501) staff       (20)        0 2023-02-20 06:19:34.000000 jamstats-nogui-1.2.1.5/src/jamstats/web/__init__.py
+-rw-r--r--   0 damonmay   (501) staff       (20)    15262 2023-04-25 03:00:12.000000 jamstats-nogui-1.2.1.5/src/jamstats/web/statserver.py
+drwxr-xr-x   0 damonmay   (501) staff       (20)        0 2023-05-02 20:08:31.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/
+-rw-r--r--   0 damonmay   (501) staff       (20)      447 2023-05-02 20:08:30.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/PKG-INFO
+-rw-r--r--   0 damonmay   (501) staff       (20)      835 2023-05-02 20:08:30.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/SOURCES.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        1 2023-05-02 20:08:30.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/dependency_links.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)      169 2023-05-02 20:08:30.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/requires.txt
+-rw-r--r--   0 damonmay   (501) staff       (20)        9 2023-05-02 20:08:30.000000 jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/top_level.txt
```

### Comparing `jamstats-nogui-1.2.1.4/README.md` & `jamstats-nogui-1.2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/bin/jamstats-nogui` & `jamstats-nogui-1.2.1.5/bin/jamstats-nogui`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/setup.py` & `jamstats-nogui-1.2.1.5/setup_nogui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
-    name='jamstats',
-    version='1.2.1',
-    description='Data processing, stats and plots on roller derby scoreboard JSON files',
+    name='jamstats-nogui',
+    version='1.2.1.4',
+    description='Data processing, stats and plots on roller derby scoreboard JSON files. No-GUI version.',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
-    packages=find_packages('src', exclude=['test']),
-    scripts=['bin/jamstats', 'bin/jamstats-nogui'],
-    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'gooey>=1.0.8.1', 'websocket-client>=1.2.1',
+    packages=['jamstats'],
+    scripts=['bin/jamstats-nogui'],
+    install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'websocket-client>=1.2.1',
 		      'Flask-SocketIO>=5.3.2', 'python-engineio>=4.3.4', 'gevent>=22.10.2', 'gevent-websocket>=0.10.1'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
     project_urls={
```

### Comparing `jamstats-nogui-1.2.1.4/setup_nogui.py` & `jamstats-nogui-1.2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jamstats-nogui',
-    version='1.2.1.4',
+    version='1.2.1.5',
     description='Data processing, stats and plots on roller derby scoreboard JSON files. No-GUI version.',
     author='Damon May',
     package_dir={"":"src"},
     include_package_data=True,
     packages=['jamstats'],
     scripts=['bin/jamstats-nogui'],
     install_requires=['pandas>=1.3.4', 'seaborn>=0.11.2', 'flask>=2.2.2', 'attrdict>=2.0.1', 'websocket-client>=1.2.1',
```

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/data/game_data.py` & `jamstats-nogui-1.2.1.5/src/jamstats/data/game_data.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/data/json_to_pandas.py` & `jamstats-nogui-1.2.1.5/src/jamstats/data/json_to_pandas.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/io/scoreboard_json_io.py` & `jamstats-nogui-1.2.1.5/src/jamstats/io/scoreboard_json_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/io/scoreboard_server_io.py` & `jamstats-nogui-1.2.1.5/src/jamstats/io/scoreboard_server_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/io/tsv_io.py` & `jamstats-nogui-1.2.1.5/src/jamstats/io/tsv_io.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/plots/jamplots.py` & `jamstats-nogui-1.2.1.5/src/jamstats/plots/jamplots.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/plots/plot_together.py` & `jamstats-nogui-1.2.1.5/src/jamstats/plots/plot_together.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/plots/plot_util.py` & `jamstats-nogui-1.2.1.5/src/jamstats/plots/plot_util.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/plots/skaterplots.py` & `jamstats-nogui-1.2.1.5/src/jamstats/plots/skaterplots.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/util/resources.py` & `jamstats-nogui-1.2.1.5/src/jamstats/util/resources.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats/web/statserver.py` & `jamstats-nogui-1.2.1.5/src/jamstats/web/statserver.py`

 * *Files identical despite different names*

### Comparing `jamstats-nogui-1.2.1.4/src/jamstats_nogui.egg-info/SOURCES.txt` & `jamstats-nogui-1.2.1.5/src/jamstats_nogui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

