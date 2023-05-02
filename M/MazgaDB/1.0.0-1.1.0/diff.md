# Comparing `tmp/MazgaDB-1.0.0.tar.gz` & `tmp/MazgaDB-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MazgaDB-1.0.0.tar", last modified: Tue May  2 12:55:41 2023, max compression
+gzip compressed data, was "MazgaDB-1.1.0.tar", last modified: Tue May  2 13:03:54 2023, max compression
```

## Comparing `MazgaDB-1.0.0.tar` & `MazgaDB-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 12:55:41.027441 MazgaDB-1.0.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 12:55:41.011441 MazgaDB-1.0.0/MazgaDB.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 12:55:40.000000 MazgaDB-1.0.0/MazgaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      513 2023-05-02 12:55:40.000000 MazgaDB-1.0.0/MazgaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-02 12:55:40.000000 MazgaDB-1.0.0/MazgaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2023-05-02 12:55:40.000000 MazgaDB-1.0.0/MazgaDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2023-05-02 12:55:40.000000 MazgaDB-1.0.0/MazgaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 12:55:41.027441 MazgaDB-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     5551 2023-05-02 12:24:10.000000 MazgaDB-1.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 12:55:41.015441 MazgaDB-1.0.0/bot_func/
--rw-r--r--   0 runner    (1000) runner    (1000)       54 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/bot_func/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/bot_func/class_people.py
--rw-r--r--   0 runner    (1000) runner    (1000)      177 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/bot_func/new_people.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 12:55:41.015441 MazgaDB-1.0.0/package/
--rw-r--r--   0 runner    (1000) runner    (1000)     3880 2023-05-02 12:18:43.000000 MazgaDB-1.0.0/package/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-04-26 09:07:23.000000 MazgaDB-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-02 12:55:41.031441 MazgaDB-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      782 2023-05-02 12:54:40.000000 MazgaDB-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 12:55:41.027441 MazgaDB-1.0.0/sql_func/
--rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-01 12:09:34.000000 MazgaDB-1.0.0/sql_func/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/append.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-02 10:42:39.000000 MazgaDB-1.0.0/sql_func/class_db.py
--rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/delete.py
--rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/delete_column.py
--rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/is_there.py
--rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/new_table.py
--rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/read_all.py
--rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/select.py
--rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-01 07:50:45.000000 MazgaDB-1.0.0/sql_func/update.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/MazgaDB.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      483 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2023-05-02 13:03:54.000000 MazgaDB-1.1.0/MazgaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     8396 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     5551 2023-05-02 12:24:10.000000 MazgaDB-1.1.0/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/bot_func/
+-rw-r--r--   0 runner    (1000) runner    (1000)       54 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      327 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/class_people.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      177 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/bot_func/new_people.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.754739 MazgaDB-1.1.0/package/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3880 2023-05-02 12:18:43.000000 MazgaDB-1.1.0/package/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-04-26 09:07:23.000000 MazgaDB-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      753 2023-05-02 13:03:36.000000 MazgaDB-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-02 13:03:54.758739 MazgaDB-1.1.0/sql_func/
+-rw-r--r--   0 runner    (1000) runner    (1000)      236 2023-05-01 12:09:34.000000 MazgaDB-1.1.0/sql_func/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/append.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3802 2023-05-02 10:42:39.000000 MazgaDB-1.1.0/sql_func/class_db.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      211 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      154 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/delete.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      467 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/delete_column.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      187 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/is_there.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      400 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/new_table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      459 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/read_all.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      251 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/select.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      235 2023-05-01 07:50:45.000000 MazgaDB-1.1.0/sql_func/update.py
```

### Comparing `MazgaDB-1.0.0/MazgaDB.egg-info/PKG-INFO` & `MazgaDB-1.1.0/MazgaDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 1.0.0
+Version: 1.1.0
 Summary: ОРМ для базы данных SQlite3
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
```

### Comparing `MazgaDB-1.0.0/PKG-INFO` & `MazgaDB-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MazgaDB
-Version: 1.0.0
+Version: 1.1.0
 Summary: ОРМ для базы данных SQlite3
 Home-page: https://github.com/Mazgagzam/MazgaDB
 Author: Mazga
 Author-email: agzamikail@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/Mazgagzam/MazgaDB
 Description: # Documentation MazgaDB
```

### Comparing `MazgaDB-1.0.0/README.md` & `MazgaDB-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `MazgaDB-1.0.0/package/__init__.py` & `MazgaDB-1.1.0/package/__init__.py`

 * *Files identical despite different names*

### Comparing `MazgaDB-1.0.0/setup.py` & `MazgaDB-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='MazgaDB',
-  version='1.0.0',
+  version='1.1.0',
   author='Mazga',
   author_email='agzamikail@gmail.com',
   description='ОРМ для базы данных SQlite3',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Mazgagzam/MazgaDB',
   packages=find_packages(),
-  install_requires=['sqlite3>=3.25','prettytable'],
+  install_requires=[],
   classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
   keywords='example python orm sql',
   project_urls={
```

### Comparing `MazgaDB-1.0.0/sql_func/class_db.py` & `MazgaDB-1.1.0/sql_func/class_db.py`

 * *Files identical despite different names*

