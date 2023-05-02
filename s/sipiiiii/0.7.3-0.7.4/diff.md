# Comparing `tmp/sipiiiii-0.7.3.tar.gz` & `tmp/sipiiiii-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipiiiii-0.7.3.tar", last modified: Tue May  2 13:23:57 2023, max compression
+gzip compressed data, was "sipiiiii-0.7.4.tar", last modified: Tue May  2 13:33:31 2023, max compression
```

## Comparing `sipiiiii-0.7.3.tar` & `sipiiiii-0.7.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.978587 sipiiiii-0.7.3/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:23:57.977884 sipiiiii-0.7.3/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.3/README.md
--rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-02 13:21:07.000000 sipiiiii-0.7.3/pyproject.toml
--rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-02 13:23:57.978727 sipiiiii-0.7.3/setup.cfg
--rw-r--r--   0 j0hn       (501) staff       (20)     1587 2023-05-02 13:22:18.000000 sipiiiii-0.7.3/setup.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.950703 sipiiiii-0.7.3/sipiiiii/
--rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.3/sipiiiii/__init__.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.960635 sipiiiii-0.7.3/sipiiiii/app/
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.3/sipiiiii/app/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)    10610 2023-04-27 14:53:07.000000 sipiiiii-0.7.3/sipiiiii/app/core.py
--rw-r--r--   0 j0hn       (501) staff       (20)    22091 2023-05-02 13:15:16.000000 sipiiiii-0.7.3/sipiiiii/app/new_app.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.969340 sipiiiii-0.7.3/sipiiiii/app/utils/
--rw-r--r--   0 j0hn       (501) staff       (20)     7849 2023-04-28 03:07:59.000000 sipiiiii-0.7.3/sipiiiii/app/utils/HttpSDK.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.977055 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/
--rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/__init__.py
--rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/generator_factory.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/prog_class.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/progbar.py
--rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.3/sipiiiii/app/utils/PPI/progpercent.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1653 2023-05-01 16:40:26.000000 sipiiiii-0.7.3/sipiiiii/app/utils/Tools.py
--rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.3/sipiiiii/app/utils/ZipFileTool.py
--rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.3/sipiiiii/app/utils/__init__.py
--rw-r--r--   0 j0hn       (501) staff       (20)      137 2023-04-18 09:35:22.000000 sipiiiii-0.7.3/sipiiiii/app/utils/config.py
--rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.3/sipiiiii/app/utils/formatConversion.py
--rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-02 13:20:15.000000 sipiiiii-0.7.3/sipiiiii/app/version.py
--rw-r--r--   0 j0hn       (501) staff       (20)     8367 2023-05-01 16:20:14.000000 sipiiiii-0.7.3/sipiiiii/main.py
-drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:23:57.954866 sipiiiii-0.7.3/sipiiiii.egg-info/
--rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:23:57.000000 sipiiiii-0.7.3/sipiiiii.egg-info/PKG-INFO
--rw-r--r--   0 j0hn       (501) staff       (20)      707 2023-05-02 13:23:57.000000 sipiiiii-0.7.3/sipiiiii.egg-info/SOURCES.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-02 13:23:57.000000 sipiiiii-0.7.3/sipiiiii.egg-info/dependency_links.txt
--rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-02 13:23:57.000000 sipiiiii-0.7.3/sipiiiii.egg-info/entry_points.txt
--rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-02 13:23:57.000000 sipiiiii-0.7.3/sipiiiii.egg-info/top_level.txt
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.615801 sipiiiii-0.7.4/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:33:31.615073 sipiiiii-0.7.4/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)     3326 2023-05-02 13:20:44.000000 sipiiiii-0.7.4/README.md
+-rw-r--r--   0 j0hn       (501) staff       (20)      468 2023-05-02 13:32:45.000000 sipiiiii-0.7.4/pyproject.toml
+-rw-r--r--   0 j0hn       (501) staff       (20)       38 2023-05-02 13:33:31.616112 sipiiiii-0.7.4/setup.cfg
+-rw-r--r--   0 j0hn       (501) staff       (20)     1587 2023-05-02 13:22:18.000000 sipiiiii-0.7.4/setup.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.587492 sipiiiii-0.7.4/sipiiiii/
+-rw-r--r--   0 j0hn       (501) staff       (20)       22 2023-03-28 16:40:14.000000 sipiiiii-0.7.4/sipiiiii/__init__.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.597095 sipiiiii-0.7.4/sipiiiii/app/
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-28 03:21:50.000000 sipiiiii-0.7.4/sipiiiii/app/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    10610 2023-04-27 14:53:07.000000 sipiiiii-0.7.4/sipiiiii/app/core.py
+-rw-r--r--   0 j0hn       (501) staff       (20)    22091 2023-05-02 13:33:08.000000 sipiiiii-0.7.4/sipiiiii/app/new_app.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.604911 sipiiiii-0.7.4/sipiiiii/app/utils/
+-rw-r--r--   0 j0hn       (501) staff       (20)     7849 2023-04-28 03:07:59.000000 sipiiiii-0.7.4/sipiiiii/app/utils/HttpSDK.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.614102 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/
+-rw-rw-r--   0 j0hn       (501) staff       (20)      174 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/__init__.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)      524 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/generator_factory.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     6829 2023-04-10 15:58:16.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/prog_class.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     3470 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progbar.py
+-rw-rw-r--   0 j0hn       (501) staff       (20)     2460 2018-04-19 14:27:03.000000 sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progpercent.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1653 2023-05-01 16:40:26.000000 sipiiiii-0.7.4/sipiiiii/app/utils/Tools.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      735 2023-03-30 02:41:50.000000 sipiiiii-0.7.4/sipiiiii/app/utils/ZipFileTool.py
+-rw-r--r--   0 j0hn       (501) staff       (20)        0 2023-03-30 02:41:28.000000 sipiiiii-0.7.4/sipiiiii/app/utils/__init__.py
+-rw-r--r--   0 j0hn       (501) staff       (20)      138 2023-05-02 13:32:29.000000 sipiiiii-0.7.4/sipiiiii/app/utils/config.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     1325 2023-01-05 06:18:13.000000 sipiiiii-0.7.4/sipiiiii/app/utils/formatConversion.py
+-rw-r--r--   0 j0hn       (501) staff       (20)       15 2023-05-02 13:32:52.000000 sipiiiii-0.7.4/sipiiiii/app/version.py
+-rw-r--r--   0 j0hn       (501) staff       (20)     8367 2023-05-01 16:20:14.000000 sipiiiii-0.7.4/sipiiiii/main.py
+drwxr-xr-x   0 j0hn       (501) staff       (20)        0 2023-05-02 13:33:31.592540 sipiiiii-0.7.4/sipiiiii.egg-info/
+-rw-r--r--   0 j0hn       (501) staff       (20)     3843 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/PKG-INFO
+-rw-r--r--   0 j0hn       (501) staff       (20)      707 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/SOURCES.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        1 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/dependency_links.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)       48 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/entry_points.txt
+-rw-r--r--   0 j0hn       (501) staff       (20)        9 2023-05-02 13:33:31.000000 sipiiiii-0.7.4/sipiiiii.egg-info/top_level.txt
```

### Comparing `sipiiiii-0.7.3/PKG-INFO` & `sipiiiii-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.3
+Version: 0.7.4
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.3/README.md` & `sipiiiii-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/setup.py` & `sipiiiii-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/core.py` & `sipiiiii-0.7.4/sipiiiii/app/core.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/new_app.py` & `sipiiiii-0.7.4/sipiiiii/app/new_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         table.add_row((app['AppName'], app['AppCnName'], app['Domain'],
                       app['ServerStatus'], app['AppStast'], app['CreateTime']))
 
     return True, table
 
 
 def get_cli_server_version():
-    return "0.7.3"
+    return "0.7.4"
 
 
 def update_template():
     pass
 
 
 def activate_account():
```

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/HttpSDK.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/HttpSDK.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/PPI/generator_factory.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/generator_factory.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/PPI/prog_class.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/prog_class.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/PPI/progbar.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progbar.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/PPI/progpercent.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/PPI/progpercent.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/Tools.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/Tools.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/ZipFileTool.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/ZipFileTool.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/app/utils/formatConversion.py` & `sipiiiii-0.7.4/sipiiiii/app/utils/formatConversion.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii/main.py` & `sipiiiii-0.7.4/sipiiiii/main.py`

 * *Files identical despite different names*

### Comparing `sipiiiii-0.7.3/sipiiiii.egg-info/PKG-INFO` & `sipiiiii-0.7.4/sipiiiii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipiiiii
-Version: 0.7.3
+Version: 0.7.4
 Summary: sipiiiii定位为简单易用的云应用托管平台
 Home-page: http://www.depl.run/
 Author: sipiiiii@admin
 Author-email: DeplRun <sipiiiii@example.com>
 Project-URL: Homepage, http://www.depl.run/
 Project-URL: Bug Tracker, http://www.depl.run/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sipiiiii-0.7.3/sipiiiii.egg-info/SOURCES.txt` & `sipiiiii-0.7.4/sipiiiii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

