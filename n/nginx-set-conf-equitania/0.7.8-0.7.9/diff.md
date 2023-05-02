# Comparing `tmp/nginx-set-conf-equitania-0.7.8.tar.gz` & `tmp/nginx-set-conf-equitania-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.7.8.tar", last modified: Tue May  2 12:53:20 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.7.9.tar", last modified: Tue May  2 13:20:28 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.7.8.tar` & `nginx-set-conf-equitania-0.7.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.184376 nginx-set-conf-equitania-0.7.8/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.7.8/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 12:53:20.184199 nginx-set-conf-equitania-0.7.8/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.7.8/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.182392 nginx-set-conf-equitania-0.7.8/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21510 2023-05-02 12:47:22.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4005 2023-05-02 12:42:36.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7077 2023-05-02 12:43:15.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 12:53:20.183931 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-02 12:53:20.000000 nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-02 12:53:20.184426 nginx-set-conf-equitania-0.7.8/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-02 12:43:01.000000 nginx-set-conf-equitania-0.7.8/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:20:28.126573 nginx-set-conf-equitania-0.7.9/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.7.9/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 13:20:28.126358 nginx-set-conf-equitania-0.7.9/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.7.9/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:20:28.111834 nginx-set-conf-equitania-0.7.9/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    21510 2023-05-02 12:47:22.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4019 2023-05-02 13:19:03.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-02 13:20:28.125828 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-02 13:20:28.000000 nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-02 13:20:28.126615 nginx-set-conf-equitania-0.7.9/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-02 13:19:14.000000 nginx-set-conf-equitania-0.7.9/setup.py
```

### Comparing `nginx-set-conf-equitania-0.7.8/LICENSE.txt` & `nginx-set-conf-equitania-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.7.8/PKG-INFO` & `nginx-set-conf-equitania-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.7.8/README.md` & `nginx-set-conf-equitania-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.7.8/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.7.9/nginx_set_conf/config_templates.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.7.8/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.7.9/nginx_set_conf/nginx_set_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # Copyright 2014-now Equitania Software GmbH - Pforzheim - Germany
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
-from utils import parse_yaml_folder, retrieve_valid_input, execute_commands
+from .utils import parse_yaml_folder, retrieve_valid_input, execute_commands
 import click
 import os
 
 def welcome():
-    click.echo("Welcome to the nginx_set_conf!")
+    click.echo("Welcome to the nginx_set_conf version 0.7.9")
 
 
 # Help text conf
 eq_config_support = """
 Insert the conf-template.
 \f
 We support:\f
```

### Comparing `nginx-set-conf-equitania-0.7.8/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.7.9/nginx_set_conf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # Copyright 2014-now Equitania Software GmbH - Pforzheim - Germany
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 import yaml
 import os
-from config_templates import get_config_template
+from .config_templates import get_config_template
 
 def fire_all_functions(function_list: list):
     """
         Execute each function in a list
         :param function_list: List of functions
     """
     for func in function_list:
```

### Comparing `nginx-set-conf-equitania-0.7.8/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.7.9/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.7.8/setup.py` & `nginx-set-conf-equitania-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.7.8",
+    version="0.7.9",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx with/without pagespeed for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

